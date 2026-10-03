<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>New Garden Hotel & Restaurant | Delicious Food & Comfortable Stay</title>

  <meta name="description"
    content="Welcome to New Garden Hotel & Restaurant. Enjoy delicious food, comfortable hospitality and a friendly atmosphere. Call 9849590871.">

  <meta name="keywords"
    content="New Garden Hotel, New Garden Restaurant, hotel Nepal, restaurant Nepal, food, hotel and restaurant">

  <meta name="author" content="New Garden Hotel & Restaurant">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #f8f8f8;
      color: #222;
      line-height: 1.6;
    }

    /* NAVBAR */
    header {
      position: sticky;
      top: 0;
      z-index: 999;
      background: rgba(255,255,255,0.97);
      box-shadow: 0 2px 15px rgba(0,0,0,0.1);
    }

    nav {
      max-width: 1200px;
      margin: auto;
      min-height: 75px;
      padding: 10px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 24px;
      font-weight: 800;
      color: #16833c;
    }

    .logo span {
      color: #e49a00;
    }

    .nav-links {
      display: flex;
      gap: 25px;
      list-style: none;
    }

    .nav-links a {
      text-decoration: none;
      color: #222;
      font-weight: 600;
      transition: .3s;
    }

    .nav-links a:hover {
      color: #16833c;
    }

    .menu-btn {
      display: none;
      font-size: 30px;
      cursor: pointer;
    }

    /* HERO */
    .hero {
      min-height: 88vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 40px 20px;
      color: white;

      background:
        linear-gradient(rgba(0,0,0,.48),rgba(0,0,0,.48)),
        url("hotel.jpg");

      background-size: cover;
      background-position: center;
    }

    .hero-content {
      max-width: 900px;
    }

    .hero h1 {
      font-size: clamp(42px, 7vw, 78px);
      margin-bottom: 15px;
      text-shadow: 2px 4px 15px #000;
    }

    .hero p {
      font-size: 22px;
      margin-bottom: 30px;
    }

    .btn {
      display: inline-block;
      padding: 14px 28px;
      margin: 5px;
      border-radius: 50px;
      text-decoration: none;
      font-weight: bold;
      transition: .3s;
      cursor: pointer;
      border: none;
      font-size: 16px;
    }

    .btn-primary {
      background: #16833c;
      color: white;
    }

    .btn-primary:hover {
      background: #0d632c;
      transform: translateY(-3px);
    }

    .btn-secondary {
      background: #e49a00;
      color: white;
    }

    .btn-secondary:hover {
      background: #c98200;
      transform: translateY(-3px);
    }

    /* GENERAL */
    section {
      padding: 80px 20px;
    }

    .container {
      max-width: 1150px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 42px;
      color: #16833c;
      margin-bottom: 10px;
    }

    .section-title p {
      color: #666;
    }

    /* ABOUT */
    .about {
      background: white;
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
      align-items: center;
    }

    .about-img img {
      width: 100%;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,.15);
    }

    .about-text h3 {
      font-size: 32px;
      margin-bottom: 15px;
      color: #222;
    }

    .about-text p {
      color: #666;
      margin-bottom: 15px;
    }

    /* FEATURES */
    .features {
      background: #f1f8f3;
    }

    .feature-grid {
      display: grid;
      grid-template-columns: repeat(4,1fr);
      gap: 20px;
    }

    .feature {
      background: white;
      padding: 30px 20px;
      text-align: center;
      border-radius: 15px;
      box-shadow: 0 5px 20px rgba(0,0,0,.07);
      transition: .3s;
    }

    .feature:hover {
      transform: translateY(-7px);
    }

    .feature-icon {
      font-size: 42px;
      margin-bottom: 10px;
    }

    .feature h3 {
      margin-bottom: 8px;
    }

    /* MENU */
    .menu-section {
      background: white;
    }

    .menu-grid {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 25px;
    }

    .food-card {
      background: white;
      border-radius: 18px;
      overflow: hidden;
      box-shadow: 0 6px 25px rgba(0,0,0,.1);
      transition: .3s;
    }

    .food-card:hover {
      transform: translateY(-8px);
    }

    .food-card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }

    .food-info {
      padding: 20px;
    }

    .food-info h3 {
      margin-bottom: 8px;
    }

    .food-info p {
      color: #777;
      font-size: 14px;
      margin-bottom: 12px;
    }

    .price {
      color: #16833c;
      font-size: 22px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    /* ORDER */
    .order-section {
      background: #f1f8f3;
    }

    .order-box {
      max-width: 800px;
      margin: auto;
      background: white;
      padding: 35px;
      border-radius: 20px;
      box-shadow: 0 8px 30px rgba(0,0,0,.1);
    }

    .cart-item {
      display: flex;
      justify-content: space-between;
      padding: 12px 0;
      border-bottom: 1px solid #ddd;
    }

    .cart-total {
      text-align: right;
      font-size: 24px;
      font-weight: bold;
      margin: 25px 0;
      color: #16833c;
    }

    input, textarea, select {
      width: 100%;
      padding: 14px;
      border: 1px solid #ddd;
      border-radius: 10px;
      margin-bottom: 15px;
      font-size: 16px;
    }

    textarea {
      height: 100px;
      resize: vertical;
    }

    /* GALLERY */
    .gallery {
      background: white;
    }

    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(2,1fr);
      gap: 25px;
    }

    .gallery-grid img {
      width: 100%;
      height: 350px;
      object-fit: cover;
      border-radius: 20px;
      transition: .3s;
    }

    .gallery-grid img:hover {
      transform: scale(1.02);
    }

    /* REVIEWS */
    .reviews {
      background: #f1f8f3;
    }

    .review-grid {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 25px;
    }

    .review {
      background: white;
      padding: 30px;
      border-radius: 18px;
      box-shadow: 0 5px 20px rgba(0,0,0,.07);
    }

    .stars {
      color: #f3a600;
      font-size: 22px;
      margin-bottom: 10px;
    }

    .review p {
      color: #666;
      margin-bottom: 15px;
    }

    /* CONTACT */
    .contact {
      background: white;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
    }

    .contact-card {
      padding: 30px;
      border-radius: 18px;
      background: #f1f8f3;
    }

    .contact-card h3 {
      margin-bottom: 15px;
      color: #16833c;
    }

    .contact-line {
      margin: 15px 0;
      font-size: 18px;
    }

    /* FOOTER */
    footer {
      background: #102117;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    footer h2 {
      color: #e49a00;
      margin-bottom: 10px;
    }

    footer p {
      color: #ccc;
      margin: 7px 0;
    }

    .social {
      margin: 20px 0;
    }

    .social a {
      color: white;
      text-decoration: none;
      margin: 0 10px;
      font-size: 18px;
    }

    /* STAFF */
    .staff {
      background: #f1f8f3;
    }

    .staff-box {
      max-width: 700px;
      margin: auto;
      background: white;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 5px 25px rgba(0,0,0,.1);
    }

    .orders {
      margin-top: 30px;
    }

    .order-card {
      border: 1px solid #ddd;
      padding: 20px;
      border-radius: 12px;
      margin-bottom: 15px;
    }

    .order-card h4 {
      color: #16833c;
      margin-bottom: 8px;
    }

    .danger {
      background: #d33;
      color: white;
    }

    /* MOBILE */
    @media(max-width: 900px) {

      .feature-grid {
        grid-template-columns: repeat(2,1fr);
      }

      .menu-grid {
        grid-template-columns: repeat(2,1fr);
      }

      .review-grid {
        grid-template-columns: 1fr;
      }

      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }
    }

    @media(max-width: 650px) {

      .menu-btn {
        display: block;
      }

      .nav-links {
        position: absolute;
        top: 75px;
        left: 0;
        width: 100%;
        background: white;
        display: none;
        flex-direction: column;
        padding: 20px;
        text-align: center;
        box-shadow: 0 5px 15px rgba(0,0,0,.1);
      }

      .nav-links.active {
        display: flex;
      }

      .feature-grid,
      .menu-grid,
      .gallery-grid {
        grid-template-columns: 1fr;
      }

      .gallery-grid img {
        height: 280px;
      }

      section {
        padding: 60px 15px;
      }

      .hero {
        min-height: 80vh;
      }

      .hero p {
        font-size: 18px;
      }

      .order-box,
      .staff-box {
        padding: 20px;
      }
    }
  </style>
</head>

<body>

<!-- NAVIGATION -->
<header>
  <nav>

    <div class="logo">
      New Garden <span>Hotel</span>
    </div>

    <div class="menu-btn" onclick="toggleMenu()">☰</div>

    <ul class="nav-links" id="navLinks">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#menu">Menu</a></li>
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#reviews">Reviews</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="#staff">Staff</a></li>
    </ul>

  </nav>
</header>


<!-- HERO -->
<section class="hero" id="home">

  <div class="hero-content">

    <h1>New Garden Hotel & Restaurant</h1>

    <p>
      Delicious Food • Friendly Service • Comfortable Hospitality
    </p>

    <a href="#menu" class="btn btn-primary">
      Explore Menu
    </a>

    <a href="#contact" class="btn btn-secondary">
      Contact Us
    </a>

  </div>

</section>


<!-- ABOUT -->
<section class="about" id="about">

  <div class="container">

    <div class="section-title">
      <h2>About Us</h2>
      <p>Welcome to New Garden Hotel & Restaurant</p>
    </div>

    <div class="about-grid">

      <div class="about-img">
        <img src="hotel.jpg" alt="New Garden Hotel and Restaurant">
      </div>

      <div class="about-text">

        <h3>A Place to Eat, Relax & Enjoy</h3>

        <p>
          Welcome to New Garden Hotel & Restaurant.
          We aim to provide delicious food, friendly service
          and a comfortable environment for our guests.
        </p>

        <p>
          Whether you are visiting with family, friends or
          colleagues, we are happy to serve you.
        </p>

        <a href="#menu" class="btn btn-primary">
          View Our Food
        </a>

      </div>

    </div>

  </div>

</section>


<!-- FEATURES -->
<section class="features">

  <div class="container">

    <div class="section-title">
      <h2>Why Choose Us?</h2>
      <p>Enjoy a friendly and comfortable experience</p>
    </div>

    <div class="feature-grid">

      <div class="feature">
        <div class="feature-icon">🍛</div>
        <h3>Delicious Food</h3>
        <p>Fresh and tasty meals for our guests.</p>
      </div>

      <div class="feature">
        <div class="feature-icon">🏨</div>
        <h3>Comfortable</h3>
        <p>A relaxing environment for visitors.</p>
      </div>

      <div class="feature">
        <div class="feature-icon">😊</div>
        <h3>Friendly Service</h3>
        <p>We care about our customers.</p>
      </div>

      <div class="feature">
        <div class="feature-icon">📞</div>
        <h3>Easy Contact</h3>
        <p>Call us whenever you need us.</p>
      </div>

    </div>

  </div>

</section>


<!-- MENU -->
<section class="menu-section" id="menu">

  <div class="container">

    <div class="section-title">
      <h2>Our Menu</h2>
      <p>Sample menu — edit the names and prices with your real menu</p>
    </div>

    <div class="menu-grid">

      <!-- FOOD 1 -->
      <div class="food-card">

        <img src="food.jpg" alt="Restaurant food">

        <div class="food-info">

          <h3>Special Fried Dish</h3>

          <p>
            Deliciously prepared special dish.
          </p>

          <div class="price">Rs. 250</div>

          <button class="btn btn-primary"
            onclick="addToCart('Special Fried Dish',250)">
            Add to Order
          </button>

        </div>

      </div>


      <!-- FOOD 2 -->
      <div class="food-card">

        <img src="food.jpg" alt="Restaurant food">

        <div class="food-info">

          <h3>Special Meal</h3>

          <p>
            A tasty meal prepared fresh.
          </p>

          <div class="price">Rs. 300</div>

          <button class="btn btn-primary"
            onclick="addToCart('Special Meal',300)">
            Add to Order
          </button>

        </div>

      </div>


      <!-- FOOD 3 -->
      <div class="food-card">

        <img src="food.jpg" alt="Restaurant food">

        <div class="food-info">

          <h3>Chef Special</h3>

          <p>
            One of our special sample dishes.
          </p>

          <div class="price">Rs. 350</div>

          <button class="btn btn-primary"
            onclick="addToCart('Chef Special',350)">
            Add to Order
          </button>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- ONLINE ORDER -->
<section class="order-section" id="order">

  <div class="container">

    <div class="section-title">
      <h2>Your Order</h2>
      <p>Add food to your cart and send your order</p>
    </div>

    <div class="order-box">

      <div id="cartItems">
        <p>Your cart is empty.</p>
      </div>

      <div class="cart-total">
        Total: Rs. <span id="cartTotal">0</span>
      </div>

      <h3>Customer Information</h3>

      <br>

      <input
        type="text"
        id="customerName"
        placeholder="Your Name"
      >

      <input
        type="tel"
        id="customerPhone"
        placeholder="Your Phone Number"
      >

      <textarea
        id="customerAddress"
        placeholder="Delivery address / additional message"
      ></textarea>

      <button
        class="btn btn-primary"
        onclick="placeOrder()">
        📲 Send Order on WhatsApp
      </button>

    </div>

  </div>

</section>


<!-- GALLERY -->
<section class="gallery" id="gallery">

  <div class="container">

    <div class="section-title">

      <h2>Our Gallery</h2>

      <p>
        A look at New Garden Hotel & Restaurant
      </p>

    </div>

    <div class="gallery-grid">

      <img
        src="hotel.jpg"
        alt="New Garden Hotel exterior"
      >

      <img
        src="food.jpg"
        alt="Food at New Garden Restaurant"
      >

    </div>

  </div>

</section>


<!-- REVIEWS -->
<section class="reviews" id="reviews">

  <div class="container">

    <div class="section-title">

      <h2>Customer Reviews</h2>

      <p>
        What our customers say
      </p>

    </div>

    <div class="review-grid">

      <div class="review">

        <div class="stars">
          ★★★★★
        </div>

        <p>
          "The food was delicious and the service was friendly."
        </p>

        <strong>Happy Customer</strong>

      </div>


      <div class="review">

        <div class="stars">
          ★★★★★
        </div>

        <p>
          "A nice place to stop, eat and relax."
        </p>

        <strong>Local Customer</strong>

      </div>


      <div class="review">

        <div class="stars">
          ★★★★★
        </div>

        <p>
          "Good atmosphere and tasty food."
        </p>

        <strong>Guest</strong>

      </div>

    </div>

  </div>

</section>


<!-- CONTACT -->
<section class="contact" id="contact">

  <div class="container">

    <div class="section-title">

      <h2>Contact Us</h2>

      <p>
        Get in touch with New Garden Hotel & Restaurant
      </p>

    </div>

    <div class="contact-grid">

      <div class="contact-card">

        <h3>Contact Information</h3>

        <div class="contact-line">
          📞 <strong>9849590871</strong>
        </div>

        <div class="contact-line">
          💬 WhatsApp Available
        </div>

        <div class="contact-line">
          📍 Nepal
        </div>

        <a
          href="tel:9849590871"
          class="btn btn-primary">
          Call Now
        </a>

        <a
          href="https://wa.me/9779849590871"
          target="_blank"
          class="btn btn-secondary">
          WhatsApp
        </a>

      </div>


      <div class="contact-card">

        <h3>Send Us a Message</h3>

        <input
          type="text"
          id="messageName"
          placeholder="Your Name"
        >

        <input
          type="tel"
          id="messagePhone"
          placeholder="Your Phone"
        >

        <textarea
          id="messageText"
          placeholder="Your message">
        </textarea>

        <button
          class="btn btn-primary"
          onclick="sendMessage()">
          Send Message
        </button>

      </div>

    </div>

  </div>

</section>


<!-- STAFF -->
<section class="staff" id="staff">

  <div class="container">

    <div class="section-title">

      <h2>Staff Dashboard</h2>

      <p>
        Staff can view orders saved on this device.
      </p>

    </div>

    <div class="staff-box">

      <input
        type="password"
        id="staffPin"
        placeholder="Enter staff PIN"
      >

      <button
        class="btn btn-primary"
        onclick="loginStaff()">
        Staff Login
      </button>

      <div id="staffDashboard" style="display:none">

        <h3>Orders</h3>

        <div id="staffOrders" class="orders"></div>

      </div>

    </div>

  </div>

</section>


<!-- FOOTER -->
<footer>

  <h2>New Garden Hotel & Restaurant</h2>

  <p>
    Delicious Food • Friendly Service • Comfortable Hospitality
  </p>

  <div class="social">

    <a href="tel:9849590871">
      📞 Call
    </a>

    <a
      href="https://wa.me/9779849590871"
      target="_blank">
      💬 WhatsApp
    </a>

  </div>

  <p>
    © 2026 New Garden Hotel & Restaurant. All Rights Reserved.
  </p>

</footer>


<script>

  /* =========================
     MOBILE MENU
  ========================= */

  function toggleMenu() {

    document
      .getElementById("navLinks")
      .classList.toggle("active");

  }


  /* =========================
     CART
  ========================= */

  let cart = [];


  function addToCart(name, price) {

    cart.push({
      name: name,
      price: price
    });

    updateCart();

    document
      .getElementById("order")
      .scrollIntoView({
        behavior: "smooth"
      });

  }


  function updateCart() {

    const cartItems =
      document.getElementById("cartItems");

    const cartTotal =
      document.getElementById("cartTotal");


    if (cart.length === 0) {

      cartItems.innerHTML =
        "<p>Your cart is empty.</p>";

      cartTotal.innerText = "0";

      return;

    }


    let total = 0;

    let html = "";


    cart.forEach((item, index) => {

      total += item.price;

      html += `

        <div class="cart-item">

          <span>
            ${item.name}
          </span>

          <span>
            Rs. ${item.price}

            <button
              onclick="removeFromCart(${index})"
              style="
                margin-left:10px;
                border:none;
                background:#d33;
                color:white;
                padding:5px 9px;
                border-radius:5px;
                cursor:pointer;">
              X
            </button>

          </span>

        </div>

      `;

    });


    cartItems.innerHTML = html;

    cartTotal.innerText = total;

  }


  function removeFromCart(index) {

    cart.splice(index, 1);

    updateCart();

  }


  /* =========================
     PLACE ORDER
  ========================= */

  function placeOrder() {

    if (cart.length === 0) {

      alert("Please add food to your order first.");

      return;

    }


    const name =
      document.getElementById("customerName").value.trim();

    const phone =
      document.getElementById("customerPhone").value.trim();

    const address =
      document.getElementById("customerAddress").value.trim();


    if (!name || !phone) {

      alert("Please enter your name and phone number.");

      return;

    }


    let total = 0;

    let orderText =
      "NEW GARDEN HOTEL & RESTAURANT ORDER\n\n";


    orderText +=
      "Customer: " + name + "\n";

    orderText +=
      "Phone: " + phone + "\n";

    orderText +=
      "Address/Message: " +
      (address || "Not provided") +
      "\n\n";

    orderText += "ORDER:\n";


    cart.forEach(item => {

      orderText +=
        "• " +
        item.name +
        " - Rs. " +
        item.price +
        "\n";

      total += item.price;

    });


    orderText +=
      "\nTOTAL: Rs. " +
      total;


    /* SAVE ORDER */

    let orders =
      JSON.parse(
        localStorage.getItem("newGardenOrders")
      ) || [];


    orders.push({

      id: Date.now(),

      customer: name,

      phone: phone,

      address: address,

      items: [...cart],

      total: total,

      status: "New",

      date: new Date().toLocaleString()

    });


    localStorage.setItem(
      "newGardenOrders",
      JSON.stringify(orders)
    );


    /* OPEN WHATSAPP */

    const whatsappURL =
      "https://wa.me/9779849590871?text=" +
      encodeURIComponent(orderText);


    window.open(
      whatsappURL,
      "_blank"
    );


    alert(
      "Order saved! WhatsApp will open now."
    );


    cart = [];

    updateCart();

  }


  /* =========================
     SEND MESSAGE
  ========================= */

  function sendMessage() {

    const name =
      document.getElementById("messageName").value.trim();

    const phone =
      document.getElementById("messagePhone").value.trim();

    const message =
      document.getElementById("messageText").value.trim();


    if (!name || !message) {

      alert(
        "Please enter your name and message."
      );

      return;

    }


    const text =
      "Hello New Garden Hotel & Restaurant!\n\n" +

      "Name: " + name + "\n" +

      "Phone: " +
      (phone || "Not provided") +
      "\n\n" +

      "Message:\n" +
      message;


    window.open(

      "https://wa.me/9779849590871?text=" +
      encodeURIComponent(text),

      "_blank"

    );

  }


  /* =========================
     STAFF LOGIN
  ========================= */

  /*
     DEMO PIN ONLY.
     This is NOT secure authentication.
  */

  const STAFF_PIN = "2468";


  function loginStaff() {

    const pin =
      document.getElementById("staffPin").value;


    if (pin !== STAFF_PIN) {

      alert("Incorrect staff PIN.");

      return;

    }


    document
      .getElementById("staffDashboard")
      .style.display = "block";


    loadOrders();

  }


  /* =========================
     LOAD STAFF ORDERS
  ========================= */

  function loadOrders() {

    const container =
      document.getElementById("staffOrders");


    const orders =
      JSON.parse(
        localStorage.getItem("newGardenOrders")
      ) || [];


    if (orders.length === 0) {

      container.innerHTML =
        "<p>No orders yet.</p>";

      return;

    }


    container.innerHTML = "";


    orders
      .slice()
      .reverse()
      .forEach(order => {

        let items = "";

        order.items.forEach(item => {

          items +=
            "<li>" +
            item.name +
            " - Rs. " +
            item.price +
            "</li>";

        });


        container.innerHTML += `

          <div class="order-card">

            <h4>
              Order #${order.id}
            </h4>

            <p>
              <strong>Customer:</strong>
              ${order.customer}
            </p>

            <p>
              <strong>Phone:</strong>
              ${order.phone}
            </p>

            <p>
              <strong>Address:</strong>
              ${order.address || "Not provided"}
            </p>

            <p>
              <strong>Date:</strong>
              ${order.date}
            </p>

            <p>
              <strong>Status:</strong>
              ${order.status}
            </p>

            <br>

            <strong>Items:</strong>

            <ul>
              ${items}
            </ul>

            <br>

            <strong>
              Total: Rs. ${order.total}
            </strong>

            <br><br>

            <button
              class="btn btn-primary"
              onclick="completeOrder(${order.id})">
              Mark Completed
            </button>

            <button
              class="btn danger"
              onclick="deleteOrder(${order.id})">
              Delete
            </button>

          </div>

        `;

      });

  }


  /* =========================
     COMPLETE ORDER
  ========================= */

  function completeOrder(id) {

    let orders =
      JSON.parse(
        localStorage.getItem("newGardenOrders")
      ) || [];


    orders =
      orders.map(order => {

        if (order.id === id) {

          order.status = "Completed";

        }

        return order;

      });


    localStorage.setItem(
      "newGardenOrders",
      JSON.stringify(orders)
    );


    loadOrders();

  }


  /* =========================
     DELETE ORDER
  ========================= */

  function deleteOrder(id) {

    if (
      !confirm(
        "Delete this order?"
      )
    ) {

      return;

    }


    let orders =
      JSON.parse(
        localStorage.getItem("newGardenOrders")
      ) || [];


    orders =
      orders.filter(
        order => order.id !== id
      );


    localStorage.setItem(
      "newGardenOrders",
      JSON.stringify(orders)
    );


    loadOrders();

  }


  /* =========================
     CLOSE MOBILE MENU
  ========================= */

  document
    .querySelectorAll(".nav-links a")
    .forEach(link => {

      link.addEventListener(
        "click",
        () => {

          document
            .getElementById("navLinks")
            .classList.remove("active");

        }
      );

    });

</script>

</body>
</html>
