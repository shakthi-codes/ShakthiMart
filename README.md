import java.util.*;

class SkillMart {
    static Scanner sc = new Scanner(System.in);

    static ArrayList<String> skills = new ArrayList<>();
    static ArrayList<Integer> prices = new ArrayList<>();

    static void addSkill() {
        System.out.print("Enter skill/service: ");
        String skill = sc.nextLine();

        System.out.print("Enter price: ");
        int price = sc.nextInt();
        sc.nextLine();

        skills.add(skill);
        prices.add(price);

        System.out.println("Skill added successfully!");
    }

    static void viewSkills() {
        if (skills.isEmpty()) {
            System.out.println("No services available.");
            return;
        }

        System.out.println("\nAvailable Services:");

        for (int i = 0; i < skills.size(); i++) {
            System.out.println((i + 1) + ". " + skills.get(i)
                    + " - Rs." + prices.get(i));
        }
    }

    static void requestSkill() {
        viewSkills();

        if (skills.isEmpty())
            return;

        System.out.print("Select service number: ");
        int choice = sc.nextInt();
        sc.nextLine();

        if (choice >= 1 && choice <= skills.size()) {
            System.out.println(
                "Service requested: " + skills.get(choice - 1)
            );
        } else {
            System.out.println("Invalid choice.");
        }
    }

    public static void main(String[] args) {

        while (true) {
            System.out.println("\n===== SKILLMART =====");
            System.out.println("1. Add Skill/Service");
            System.out.println("2. View Services");
            System.out.println("3. Request Service");
            System.out.println("4. Exit");

            System.out.print("Enter choice: ");
            int choice = sc.nextInt();
            sc.nextLine();

            switch (choice) {
                case 1:
                    addSkill();
                    break;

                case 2:
                    viewSkills();
                    break;

                case 3:
                    requestSkill();
                    break;

                case 4:
                    System.out.println("Thank you for using SkillMart!");
                    return;

                default:
                    System.out.println("Invalid choice.");
            }
        }
    }
}

