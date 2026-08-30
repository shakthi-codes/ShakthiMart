<!DOCTYPE html>  <html lang="en">  
<head>   
<meta charset="UTF-8">   
<meta name="viewport" content="width=device-width, initial-scale=1.0">  <title>Shakthi Mart - Skill Marketplace</title>  <style>  
  
/* ==============================  
   GENERAL  
================================= */  
  
* {  
    margin: 0;  
    padding: 0;  
    box-sizing: border-box;  
    font-family: Arial, "Segoe UI", sans-serif;  
}  
  
body {  
    background: #f5f7ff;  
    color: #202124;  
}  
  
button,  
input,  
select,  
textarea {  
    font: inherit;  
}  
  
button {  
    cursor: pointer;  
}  
  
  
/* ==============================  
   LOGIN PAGE  
================================= */  
  
#loginPage {  
    min-height: 100vh;  
  
    display: flex;  
    align-items: center;  
    justify-content: center;  
  
    padding: 20px;  
  
    background:  
        linear-gradient(  
            135deg,  
            #312e81,  
            #4f46e5 55%,  
            #7c3aed  
        );  
}  
  
.login-card {  
    width: 100%;  
    max-width: 420px;  
  
    background: white;  
  
    border-radius: 22px;  
  
    padding: 35px;  
  
    box-shadow: 0 20px 60px rgba(0,0,0,0.35);  
  
    text-align: center;  
}  
  
.logo {  
    width: 75px;  
    height: 75px;  
  
    border-radius: 22px;  
  
    background: #4f46e5;  
    color: white;  
  
    display: flex;  
    align-items: center;  
    justify-content: center;  
  
    font-size: 35px;  
    font-weight: 800;  
  
    margin: 0 auto 15px;  
}  
  
.login-card h1 {  
    color: #3730a3;  
    font-size: 30px;  
}  
  
.login-card p {  
    color: #6b7280;  
    margin: 8px 0 25px;  
}  
  
  
/* ==============================  
   FORM  
================================= */  
  
.form-group {  
    text-align: left;  
    margin: 15px 0;  
}  
  
.form-group label {  
    display: block;  
  
    font-weight: 700;  
  
    margin-bottom: 7px;  
  
    font-size: 14px;  
}  
  
.form-group input,  
.form-group select,  
.form-group textarea {  
    width: 100%;  
  
    padding: 12px;  
  
    border: 1px solid #d8dbe8;  
  
    border-radius: 9px;  
  
    outline: none;  
}  
  
.form-group input:focus,  
.form-group select:focus,  
.form-group textarea:focus {  
    border-color: #4f46e5;  
}  
  
.primary {  
    width: 100%;  
  
    border: 0;  
  
    border-radius: 9px;  
  
    padding: 13px;  
  
    background: #4f46e5;  
  
    color: white;  
  
    font-weight: 700;  
}  
  
.primary:hover {  
    background: #3730a3;  
}  
  
.demo {  
    font-size: 12px;  
  
    color: #777;  
  
    margin-top: 12px;  
}  
  
  
/* ==============================  
   APPLICATION  
================================= */  
  
#app {  
    display: none;  
}  
  
  
/* ==============================  
   HEADER  
================================= */  
  
header {  
    position: sticky;  
  
    top: 0;  
  
    z-index: 50;  
  
    background: #4f46e5;  
  
    color: white;  
  
    padding: 13px 5%;  
  
    display: flex;  
  
    align-items: center;  
  
    gap: 20px;  
  
    box-shadow: 0 3px 12px rgba(0,0,0,0.15);  
}  
  
.brand {  
    font-size: 24px;  
  
    font-weight: 800;  
  
    white-space: nowrap;  
}  
  
.brand span {  
    font-size: 14px;  
  
    display: block;  
  
    font-weight: 400;  
  
    opacity: 0.85;  
}  
  
.search {  
    flex: 1;  
  
    max-width: 500px;  
}  
  
.search input {  
    width: 100%;  
  
    padding: 11px 18px;  
  
    border: 0;  
  
    border-radius: 25px;  
  
    outline: none;  
}  
  
.header-actions {  
    display: flex;  
  
    gap: 8px;  
}  
  
.header-btn {  
    border: 0;  
  
    background: #312e81;  
  
    color: white;  
  
    padding: 10px 13px;  
  
    border-radius: 8px;  
  
    font-weight: 700;  
}  
  
  
/* ==============================  
   MAIN  
================================= */  
  
main {  
    max-width: 1250px;  
  
    margin: auto;  
  
    padding: 25px 18px 50px;  
}  
  
  
/* ==============================  
   HERO  
================================= */  
  
.hero {  
    background:  
        linear-gradient(  
            135deg,  
            #eef2ff,  
            #ffffff  
        );  
  
    border: 1px solid #dfe3ff;  
  
    border-radius: 18px;  
  
    padding: 28px;  
  
    margin-bottom: 22px;  
}  
  
.hero h2 {  
    color: #3730a3;  
  
    font-size: 28px;  
  
    margin-bottom: 8px;  
}  
  
.hero p {  
    color: #5f6470;  
  
    max-width: 700px;  
}  
  
  
/* ==============================  
   STATISTICS  
================================= */  
  
.stats {  
    display: flex;  
  
    gap: 12px;  
  
    flex-wrap: wrap;  
  
    margin-top: 18px;  
}  
  
.stat {  
    background: white;  
  
    border-radius: 10px;  
  
    padding: 12px 16px;  
  
    box-shadow: 0 3px 12px rgba(0,0,0,0.05);  
}  
  
.stat b {  
    color: #4f46e5;  
}  
  
  
/* ==============================  
   TOOLBAR  
================================= */  
  
.toolbar {  
    display: flex;  
  
    gap: 10px;  
  
    align-items: center;  
  
    justify-content: space-between;  
  
    margin: 22px 0;  
  
    flex-wrap: wrap;  
}  
  
.categories {  
    display: flex;  
  
    gap: 8px;  
  
    flex-wrap: wrap;  
}  
  
.cat {  
    border: 1px solid #cdd2ed;  
  
    background: white;  
  
    color: #3730a3;  
  
    border-radius: 20px;  
  
    padding: 8px 14px;  
}  
  
.cat.active,  
.cat:hover {  
    background: #4f46e5;  
  
    color: white;  
}  
  
  
/* ==============================  
   SECTION TITLE  
================================= */  
  
.section-title {  
    color: #3730a3;  
  
    font-size: 22px;  
  
    margin-bottom: 15px;  
}  
  
  
/* ==============================  
   PRODUCT / SERVICE GRID  
================================= */  
  
.grid {  
    display: grid;  
  
    grid-template-columns:  
        repeat(  
            auto-fill,  
            minmax(250px, 1fr)  
        );  
  
    gap: 18px;  
}  
  
  
/* ==============================  
   SERVICE CARD  
================================= */  
  
.card {  
    background: white;  
  
    border-radius: 14px;  
  
    padding: 20px;  
  
    box-shadow: 0 4px 16px rgba(0,0,0,0.06);  
  
    border: 1px solid #eee;  
  
    transition: 0.2s;  
}  
  
.card:hover {  
    transform: translateY(-3px);  
  
    box-shadow:  
        0 8px 22px rgba(0,0,0,0.1);  
}  
  
.icon {  
    width: 58px;  
    height: 58px;  
  
    border-radius: 14px;  
  
    background: #eef2ff;  
  
    display: flex;  
  
    align-items: center;  
    justify-content: center;  
  
    font-size: 30px;  
  
    margin-bottom: 13px;  
}  
  
.card h3 {  
    margin-bottom: 7px;  
}  
  
.card p {  
    font-size: 14px;  
  
    color: #666;  
  
    line-height: 1.45;  
  
    min-height: 41px;  
}  
  
.provider {  
    font-size: 12px;  
  
    color: #777;  
  
    margin: 10px 0;  
}  
  
.price {  
    font-size: 19px;  
  
    color: #4f46e5;  
  
    font-weight: 800;  
  
    margin: 10px 0;  
}  
  
.actions {  
    display: flex;  
  
    gap: 8px;  
}  
  
.actions button {  
    flex: 1;  
  
    padding: 10px;  
  
    border-radius: 8px;  
  
    font-weight: 700;  
}  
  
.book {  
    background: #4f46e5;  
  
    color: white;  
  
    border: 0;  
}  
  
.book:hover {  
    background: #3730a3;  
}  
  
.cart {  
    background: white;  
  
    color: #4f46e5;  
  
    border: 1px solid #4f46e5;  
}  
  
.cart:hover {  
    background: #eef2ff;  
}  
  
  
/* ==============================  
   EMPTY MESSAGE  
================================= */  
  
.empty {  
    text-align: center;  
  
    background: white;  
  
    padding: 35px;  
  
    border-radius: 12px;  
  
    color: #777;  
}  
  
  
/* ==============================  
   MODAL  
================================= */  
  
.modal {  
    position: fixed;  
  
    inset: 0;  
  
    background: rgba(0,0,0,0.6);  
  
    display: none;  
  
    align-items: center;  
  
    justify-content: center;  
  
    z-index: 100;  
  
    padding: 20px;  
}  
  
.modal-box {  
    background: white;  
  
    width: 100%;  
  
    max-width: 480px;  
  
    max-height: 90vh;  
  
    overflow: auto;  
  
    border-radius: 16px;  
  
    padding: 25px;  
}  
  
.modal-head {  
    display: flex;  
  
    justify-content: space-between;  
  
    align-items: center;  
  
    margin-bottom: 15px;  
}  
  
.modal-box h2 {  
    color: #3730a3;  
}  
  
.close {  
    border: 0;  
  
    background: none;  
  
    font-size: 28px;  
  
    color: #777;  
}  
  
  
/* ==============================  
   CART  
================================= */  
  
.cart-row {  
    display: flex;  
  
    justify-content: space-between;  
  
    gap: 10px;  
  
    padding: 12px 0;  
  
    border-bottom: 1px solid #eee;  
}  
  
.remove {  
    border: 0;  
  
    background: none;  
  
    color: #d32f2f;  
  
    font-size: 12px;  
}  
  
.total {  
    display: flex;  
  
    justify-content: space-between;  
  
    font-size: 20px;  
  
    font-weight: 800;  
  
    margin: 18px 0;  
}  
  
  
/* ==============================  
   TOAST  
================================= */  
  
.toast {  
    position: fixed;  
  
    bottom: 20px;  
  
    left: 50%;  
  
    transform: translateX(-50%);  
  
    background: #222;  
  
    color: white;  
  
    padding: 12px 18px;  
  
    border-radius: 9px;  
  
    display: none;  
  
    z-index: 200;  
}  
  
  
/* ==============================  
   FOOTER  
================================= */  
  
footer {  
    text-align: center;  
  
    padding: 25px;  
  
    color: #777;  
  
    font-size: 13px;  
}  
  
  
/* ==============================  
   MOBILE  
================================= */  
  
@media(max-width:700px) {  
  
    header {  
        flex-wrap: wrap;  
    }  
  
    .brand {  
        width: 100%;  
    }  
  
    .search {  
        order: 3;  
  
        max-width: none;  
  
        width: 100%;  
    }  
  
    .header-actions {  
        margin-left: auto;  
    }  
  
    .hero h2 {  
        font-size: 23px;  
    }  
  
    .grid {  
        grid-template-columns: 1fr;  
    }  
  
}  
  
</style>  </head>  <body>  <!-- ==========================================  
     LOGIN PAGE  
=========================================== -->  <section id="loginPage">  <div class="login-card">  

    <div class="logo">  
        S  
    </div>  

    <h1>  
        Shakthi Mart  
    </h1>  

    <p>  
        Skill Marketplace • Learn, Share & Earn  
    </p>  


    <form id="loginForm">  

        <div class="form-group">  

            <label>  
                Username  
            </label>  

            <input  
                id="username"  
                type="text"  
                placeholder="Enter username"  
                required  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Password  
            </label>  

            <input  
                id="password"  
                type="password"  
                placeholder="Enter password"  
                required  
            >  

        </div>  


        <button  
            class="primary"  
            type="submit"  
        >  
            Login to Shakthi Mart  
        </button>  

    </form>  


    <div class="demo">  
        Demo mode: enter any username and password.  
    </div>  

</div>

</section>  <!-- ==========================================  
     MAIN APPLICATION  
=========================================== -->  <div id="app">  <!-- HEADER -->  <header>  <div class="brand">  

    Shakthi Mart 🛠️  

    <span>  
        Skill Marketplace  
    </span>  

</div>  


<div class="search">  

    <input  
        id="search"  
        placeholder="Search skills, services or categories..."  
    >  

</div>  


<div class="header-actions">  

    <button  
        class="header-btn"  
        id="cartBtn"  
    >  
        🛒 Cart  
        (<span id="cartCount">0</span>)  
    </button>  


    <button  
        class="header-btn"  
        id="logoutBtn"  
    >  
        Logout  
    </button>  

</div>

</header>  <!-- MAIN -->  <main>  <!-- HERO -->  <section class="hero">  <h2>  
    Welcome to Shakthi Mart 👋  
</h2>  

<p>  
    Find trusted student skills and services,  
    book talented people, or offer your own  
    skills to earn.  
</p>  


<div class="stats">  

    <div class="stat">  

        Available Services  

        <b id="serviceCount">  
            0  
        </b>  

    </div>  


    <div class="stat">  

        Categories  

        <b>  
            6  
        </b>  

    </div>  


    <div class="stat">  

        Marketplace  

        <b>  
            Online  
        </b>  

    </div>  

</div>

</section>  <!-- CATEGORY TOOLBAR -->  <div class="toolbar">  <div class="categories">  


    <button  
        class="cat active"  
        data-cat="All"  
    >  
        All  
    </button>  


    <button  
        class="cat"  
        data-cat="Technology"  
    >  
        Technology  
    </button>  


    <button  
        class="cat"  
        data-cat="Design"  
    >  
        Design  
    </button>  


    <button  
        class="cat"  
        data-cat="Education"  
    >  
        Education  
    </button>  


    <button  
        class="cat"  
        data-cat="Media"  
    >  
        Media  
    </button>  


    <button  
        class="cat"  
        data-cat="Writing"  
    >  
        Writing  
    </button>  


    <button  
        class="cat"  
        data-cat="Business"  
    >  
        Business  
    </button>  


</div>  


<button  
    class="cat"  
    id="offerBtn"  
>  
    ＋ Offer Your Skill  
</button>

</div>  <!-- SERVICES -->  <h2 class="section-title">  
    Available Skills & Services  
</h2>  <div  
    class="grid"  
    id="serviceGrid"  
>  
</div>  <footer>  © 2026 Shakthi Mart  
• Learn • Share • Earn

</footer>  </main>  </div>  <!-- ==========================================  
     CART MODAL  
=========================================== -->  <div  
    class="modal"  
    id="cartModal"  
>  <div class="modal-box">  


    <div class="modal-head">  

        <h2>  
            Your Cart 🛒  
        </h2>  

        <button  
            class="close"  
            onclick="closeModal('cartModal')"  
        >  
            ×  
        </button>  

    </div>  


    <div id="cartItems">  
    </div>  


    <div class="total">  

        <span>  
            Total  
        </span>  

        <span id="cartTotal">  
            ₹0  
        </span>  

    </div>  


    <button  
        class="primary"  
        id="checkoutBtn"  
    >  
        Proceed to Checkout  
    </button>  


</div>

</div>  <!-- ==========================================  
     BOOKING MODAL  
=========================================== -->  <div  
    class="modal"  
    id="bookingModal"  
>  <div class="modal-box">  


    <div class="modal-head">  

        <h2>  
            Book Service  
        </h2>  

        <button  
            class="close"  
            onclick="closeModal('bookingModal')"  
        >  
            ×  
        </button>  

    </div>  


    <form id="bookingForm">  


        <div class="form-group">  

            <label>  
                Service  
            </label>  

            <input  
                id="bookService"  
                readonly  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Your Name  
            </label>  

            <input  
                id="bookName"  
                required  
                placeholder="Enter your name"  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Phone Number  
            </label>  

            <input  
                id="bookPhone"  
                required  
                type="tel"  
                placeholder="Enter phone number"  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Preferred Date  
            </label>  

            <input  
                id="bookDate"  
                required  
                type="date"  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Requirements  
            </label>  

            <textarea  
                id="bookReq"  
                rows="3"  
                placeholder="Tell the service provider what you need"  
            ></textarea>  

        </div>  


        <button  
            class="primary"  
        >  
            Confirm Booking  
        </button>  


    </form>  

</div>

</div>  <!-- ==========================================  
     OFFER SKILL MODAL  
=========================================== -->  <div  
    class="modal"  
    id="offerModal"  
>  <div class="modal-box">  


    <div class="modal-head">  

        <h2>  
            Offer Your Skill  
        </h2>  

        <button  
            class="close"  
            onclick="closeModal('offerModal')"  
        >  
            ×  
        </button>  

    </div>  


    <form id="offerForm">  


        <div class="form-group">  

            <label>  
                Skill / Service Name  
            </label>  

            <input  
                id="offerName"  
                required  
                placeholder="e.g. Python Programming"  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Category  
            </label>  

            <select  
                id="offerCategory"  
                required  
            >  

                <option value="">  
                    Select category  
                </option>  

                <option>  
                    Technology  
                </option>  

                <option>  
                    Design  
                </option>  

                <option>  
                    Education  
                </option>  

                <option>  
                    Media  
                </option>  

                <option>  
                    Writing  
                </option>  

                <option>  
                    Business  
                </option>  

            </select>  

        </div>  


        <div class="form-group">  

            <label>  
                Description  
            </label>  

            <textarea  
                id="offerDesc"  
                rows="3"  
                required  
                placeholder="Describe your service"  
            ></textarea>  

        </div>  


        <div class="form-group">  

            <label>  
                Price (₹)  
            </label>  

            <input  
                id="offerPrice"  
                type="number"  
                min="1"  
                required  
                placeholder="500"  
            >  

        </div>  


        <button  
            class="primary"  
        >  
            Publish Service  
        </button>  


    </form>  

</div>

</div>  <!-- ==========================================  
     CHECKOUT MODAL  
=========================================== -->  <div  
    class="modal"  
    id="checkoutModal"  
>  <div class="modal-box">  


    <div class="modal-head">  

        <h2>  
            Checkout  
        </h2>  

        <button  
            class="close"  
            onclick="closeModal('checkoutModal')"  
        >  
            ×  
        </button>  

    </div>  


    <form id="checkoutForm">  


        <div class="form-group">  

            <label>  
                Full Name  
            </label>  

            <input  
                id="custName"  
                required  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Phone Number  
            </label>  

            <input  
                id="custPhone"  
                required  
                type="tel"  
            >  

        </div>  


        <div class="form-group">  

            <label>  
                Payment Method  
            </label>  

            <select  
                id="payment"  
                required  
            >  

                <option value="">  
                    Select payment  
                </option>  

                <option>  
                    Cash on Delivery  
                </option>  

                <option>  
                    UPI  
                </option>  

                <option>  
                    Card  
                </option>  

            </select>  

        </div>  


        <div class="form-group">  

            <label>  
                Address / Meeting Details  
            </label>  

            <textarea  
                id="address"  
                rows="3"  
                required  
            ></textarea>  

        </div>  


        <button  
            class="primary"  
        >  
            Place Order  
        </button>  


    </form>  

</div>

</div>  <!-- TOAST -->  <div  
    class="toast"  
    id="toast"  
>  
</div>  <script>  
  
/* ==========================================  
   SERVICE DATA  
=========================================== */  
  
const services = [  
  
    {  
        id: 1,  
        name: "Web Development",  
        cat: "Technology",  
        icon: "💻",  
        desc: "Responsive websites, portfolio pages and college projects.",  
        price: 500,  
        provider: "Arun • Verified Student"  
    },  
  
    {  
        id: 2,  
        name: "Java Programming",  
        cat: "Technology",  
        icon: "☕",  
        desc: "Java programs, debugging and beginner project support.",  
        price: 400,  
        provider: "Kavin • Java Developer"  
    },  
  
    {  
        id: 3,  
        name: "Graphic Design",  
        cat: "Design",  
        icon: "🎨",  
        desc: "Logos, posters, presentations and social media designs.",  
        price: 300,  
        provider: "Meena • Designer"  
    },  
  
    {  
        id: 4,  
        name: "UI/UX Design",  
        cat: "Design",  
        icon: "🖌️",  
        desc: "Clean app and website interface designs for projects.",  
        price: 600,  
        provider: "Priya • UI Designer"  
    },  
  
    {  
        id: 5,  
        name: "Academic Tutoring",  
        cat: "Education",  
        icon: "📚",  
        desc: "One-to-one help for school and college subjects.",  
        price: 200,  
        provider: "Sanjay • Tutor"  
    },  
  
    {  
        id: 6,  
        name: "Python & Data Science",  
        cat: "Education",  
        icon: "🐍",  
        desc: "Python basics, data analysis and beginner ML guidance.",  
        price: 450,  
        provider: "Naveen • AI & DS Student"  
    },  
  
    {  
        id: 7,  
        name: "Video Editing",  
        cat: "Media",  
        icon: "🎬",  
        desc: "Edit reels, presentations, college videos and short films.",  
        price: 400,  
        provider: "Dharani • Video Editor"  
    },  
  
    {  
        id: 8,  
        name: "Photography",  
        cat: "Media",  
        icon: "📷",  
        desc: "Event, product and project photography services.",  
        price: 600,  
        provider: "Vijay • Photographer"  
    },  
  
    {  
        id: 9,  
        name: "Content Writing",  
        cat: "Writing",  
        icon: "✍️",  
        desc: "Articles, blogs, captions and project documentation.",  
        price: 350,  
        provider: "Aishwarya • Writer"  
    },  
  
    {  
        id: 10,  
        name: "Resume Creation",  
        cat: "Business",  
        icon: "📄",  
        desc: "Professional student resumes and project profiles.",  
        price: 250,  
        provider: "Rahul • Career Support"  
    },  
  
    {  
        id: 11,  
        name: "Digital Marketing",  
        cat: "Business",  
        icon: "📈",  
        desc: "Social media ideas, basic SEO and digital promotion.",  
        price: 500,  
        provider: "Keerthi • Marketing"  
    },  
  
    {  
        id: 12,  
        name: "Presentation Design",  
        cat: "Design",  
        icon: "📊",  
        desc: "Professional PPT layouts for seminars and college projects.",  
        price: 300,  
        provider: "Shakthi • Presentation Designer"  
    }  
  
];  
  
  
/* ==========================================  
   VARIABLES  
=========================================== */  
  
let cart = [];  
  
let activeCategory = "All";  
  
let user = "";  
  
  
/* ==========================================  
   SHORTCUT  
=========================================== */  
  
const $ = id =>  
    document.getElementById(id);  
  
  
/* ==========================================  
   LOGIN  
=========================================== */  
  
$("loginForm").addEventListener(  
    "submit",  
    function(event) {  
  
        event.preventDefault();  
  
        user =  
            $("username")  
            .value  
            .trim();  
  
        const password =  
            $("password")  
            .value  
            .trim();  
  
  
        if (  
            user === "" ||  
            password === ""  
        ) {  
  
            alert(  
                "Please enter username and password."  
            );  
  
            return;  
  
        }  
  
  
        $("loginPage").style.display =  
            "none";  
  
        $("app").style.display =  
            "block";  
  
  
        renderServices();  
  
    }  
);  
  
  
/* ==========================================  
   DISPLAY SERVICES  
=========================================== */  
  
function renderServices() {  
  
    const query =  
        $("search")  
        .value  
        .toLowerCase()  
        .trim();  
  
  
    const filtered =  
        services.filter(  
  
            service =>  
  
                (  
                    activeCategory === "All" ||  
                    service.cat === activeCategory  
                )  
  
                &&  
  
                (  
                    service.name  
                    .toLowerCase()  
                    .includes(query)  
  
                    ||  
  
                    service.cat  
                    .toLowerCase()  
                    .includes(query)  
  
                    ||  
  
                    service.desc  
                    .toLowerCase()  
                    .includes(query)  
                )  
  
        );  
  
  
    $("serviceCount")  
        .textContent =  
        services.length;  
  
  
    if (filtered.length === 0) {  
  
        $("serviceGrid").innerHTML =  
  
            `  
            <div class="empty">  
  
                No services found.  
  
                <br><br>  
  
                Try another search  
                or category.  
  
            </div>  
            `;  
  
        return;  
  
    }  
  
  
    $("serviceGrid").innerHTML =  
  
        filtered  
        .map(service =>  
  
            `  
  
            <div class="card">  
  
                <div class="icon">  
  
                    ${service.icon}  
  
                </div>  
  
  
                <h3>  
  
                    ${service.name}  
  
                </h3>  
  
  
                <p>  
  
                    ${service.desc}  
  
                </p>  
  
  
                <div class="provider">  
  
                    👤 ${service.provider}  
  
                </div>  
  
  
                <div class="price">  
  
                    ₹${service.price}  
                    / service  
  
                </div>  
  
  
                <div class="actions">  
  
                    <button  
                        class="book"  
                        onclick="bookService(${service.id})"  
                    >  
  
                        Book Now  
  
                    </button>  
  
  
                    <button  
                        class="cart"  
                        onclick="addToCart(${service.id})"  
                    >  
  
                        Add to Cart  
  
                    </button>  
  
                </div>  
  
            </div>  
  
            `  
  
        )  
        .join("");  
  
}  
  
  
/* ==========================================  
   SEARCH  
=========================================== */  
  
$("search")  
    .addEventListener(  
        "input",  
        renderServices  
    );  
  
  
/* ==========================================  
   CATEGORY FILTER  
=========================================== */  
  
document  
.querySelectorAll(".cat")  
.forEach(button => {  
  
    button.addEventListener(  
        "click",  
        function() {  
  
            if (!this.dataset.cat) {  
                return;  
            }  
  
  
            activeCategory =  
                this.dataset.cat;  
  
  
            document  
            .querySelectorAll(".cat")  
            .forEach(  
                item =>  
                item.classList.remove("active")  
            );  
  
  
            this.classList.add("active");  
  
  
            renderServices();  
  
        }  
    );  
  
});  
  
  
/* ==========================================  
   ADD TO CART  
=========================================== */  
  
function addToCart(id) {  
  
    const service =  
        services.find(  
            item => item.id === id  
        );  
  
  
    const existing =  
        cart.find(  
            item => item.id === id  
        );  
  
  
    if (existing) {  
  
        existing.qty++;  
  
    } else {  
  
        cart.push({  
  
            ...service,  
  
            qty: 1  
  
        });  
  
    }  
  
  
    updateCart();  
  
  
    showToast(  
        service.name +  
        " added to cart ✓"  
    );  
  
}  
  
  
/* ==========================================  
   UPDATE CART  
=========================================== */  
  
function updateCart() {  
  
    const count =  
        cart.reduce(  
            (total, item) =>  
            total + item.qty,  
            0  
        );  
  
  
    $("cartCount")  
        .textContent =  
        count;  
  
  
    let total = 0;  
  
  
    if (cart.length === 0) {  
  
        $("cartItems").innerHTML =  
  
            `  
            <div class="empty">  
  
                Your cart is empty 🛒  
  
            </div>  
            `;  
  
    } else {  
  
        $("cartItems").innerHTML =  
  
            cart  
            .map(item => {  
  
                total +=  
                    item.price *  
                    item.qty;  
  
  
                return `  
  
                <div class="cart-row">  
  
                    <div>  
  
                        <b>  
                            ${item.name}  
                        </b>  
  
                        <br>  
  
                        <small>  
  
                            ₹${item.price}  
                            ×  
                            ${item.qty}  
  
                        </small>  
  
                    </div>  
  
  
                    <div>  
  
                        ₹${item.price * item.qty}  
  
                        <br>  
  
                        <button  
                            class="remove"  
                            onclick="removeFromCart(${item.id})"  
                        >  
  
                            Remove  
  
                        </button>  
  
                    </div>  
  
                </div>  
  
                `;  
  
            })  
            .join("");  
  
    }  
  
  
    $("cartTotal")  
        .textContent =  
        "₹" + total;  
  
  
    $("checkoutBtn")  
        .disabled =  
        cart.length === 0;  
  
}  
  
  
/* ==========================================  
   REMOVE CART ITEM  
=========================================== */  
  
function removeFromCart(id) {  
  
    cart =  
        cart.filter(  
            item =>  
            item.id !== id  
        );  
  
  
    updateCart();  
  
}  
  
  
/* ==========================================  
   OPEN CART  
=========================================== */  
  
$("cartBtn")  
.addEventListener(  
    "click",  
    function() {  
  
        updateCart();  
  
        $("cartModal")  
            .style.display =  
            "flex";  
  
    }  
);  
  
  
/* ==========================================  
   CHECKOUT  
=========================================== */  
  
$("checkoutBtn")  
.addEventListener(  
    "click",  
    function() {  
  
        if (cart.length === 0) {  
  
            alert(  
                "Your cart is empty."  
            );  
  
            return;  
  
        }  
  
  
        closeModal("cartModal");  
  
  
        $("checkoutModal")  
            .style.display =  
            "flex";  
  
    }  
);  
  
  
/* ==========================================  
   BOOK SERVICE  
=========================================== */  
  
function bookService(id) {  
  
    const service =  
        services.find(  
            item =>  
            item.id === id  
        );  
  
  
    $("bookService")  
        .value =  
        service.name;  
  
  
    $("bookingModal")  
        .style.display =  
        "flex";  
  
}  
  
  
/* ==========================================  
   BOOKING FORM  
=========================================== */  
  
$("bookingForm")  
.addEventListener(  
    "submit",  
    function(event) {  
  
        event.preventDefault();  
  
  
        const service =  
            $("bookService")  
            .value;  
  
  
        closeModal(  
            "bookingModal"  
        );  
  
  
        this.reset();  
  
  
        showToast(  
            "Booking request sent for " +  
            service +  
            " ✓"  
        );  
  
    }  
);  
  
  
/* ==========================================  
   OFFER YOUR SKILL  
=========================================== */  
  
$("offerBtn")  
.addEventListener(  
    "click",  
    function() {  
  
        $("offerModal")  
            .style.display =  
            "flex";  
  
    }  
);  
  
  
/* ==========================================  
   OFFER FORM  
=========================================== */  
  
$("offerForm")  
.addEventListener(  
    "submit",  
    function(event) {  
  
        event.preventDefault();  
  
  
        const newService = {  
  
            id:  
                Date.now(),  
  
            name:  
                $("offerName")  
                .value,  
  
            cat:  
                $("offerCategory")  
                .value,  
  
            icon:  
                "⭐",  
  
            desc:  
                $("offerDesc")  
                .value,  
  
            price:  
                Number(  
                    $("offerPrice")  
                    .value  
                ),  
  
            provider:  
                user +  
                " • New Provider"  
  
        };  
  
  
        services.unshift(  
            newService  
        );  
  
  
        closeModal(  
            "offerModal"  
        );  
  
  
        this.reset();  
  
  
        activeCategory =  
            "All";  
  
  
        document  
        .querySelectorAll(".cat")  
        .forEach(  
            item =>  
            item.classList.remove("active")  
        );  
  
  
        document  
        .querySelector(  
            '[data-cat="All"]'  
        )  
        .classList.add("active");  
  
  
        renderServices();  
  
  
        showToast(  
            "Your service was published ✓"  
        );  
  
    }  
);  
  
  
/* ==========================================  
   CHECKOUT FORM  
=========================================== */  
  
$("checkoutForm")  
.addEventListener(  
    "submit",  
    function(event) {  
  
        event.preventDefault();  
  
  
        const total =  
            cart.reduce(  
                (sum, item) =>  
                sum +  
                item.price *  
                item.qty,  
                0  
            );  
  
  
        cart = [];  
  
  
        updateCart();  
  
  
        closeModal(  
            "checkoutModal"  
        );  
  
  
        this.reset();  
  
  
        showToast(  
            "Order placed successfully! Total ₹" +  
            total +  
            " ✓"  
        );  
  
    }  
);  
  
  
/* ==========================================  
   LOGOUT  
=========================================== */  
  
$("logoutBtn")  
.addEventListener(  
    "click",  
    function() {  
  
        $("app")  
            .style.display =  
            "none";  
  
  
        $("loginPage")  
            .style.display =  
            "flex";  
  
  
        $("loginForm")  
            .reset();  
  
  
        cart = [];  
  
  
        updateCart();  
  
    }  
);  
  
  
/* ==========================================  
   CLOSE MODAL  
=========================================== */  
  
function closeModal(id) {  
  
    $(id)  
        .style.display =  
        "none";  
  
}  
  
  
/* ==========================================  
   TOAST MESSAGE  
=========================================== */  
  
function showToast(message) {  
  
    const toast =  
        $("toast");  
  
  
    toast.textContent =  
        message;  
  
  
    toast.style.display =  
        "block";  
  
  
    setTimeout(  
        function() {  
  
            toast.style.display =  
                "none";  
  
        },  
        2500  
    );  
  
}  
  
  
/* ==========================================  
   INITIAL CART  
=========================================== */  
  
updateCart();  
  
</script>  </body>  
</html>  
