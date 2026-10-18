 
<!DOCTYPE html>
<html lang="ur" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>میری پرفیوم شاپ</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff;
      color: #222;
    }

    header {
      background: #171717;
      color: white;
      text-align: center;
      padding: 22px;
    }

    nav {
      background: #c5a46d;
      padding: 12px;
      text-align: center;
    }

    nav a {
      color: #111;
      text-decoration: none;
      margin: 10px;
    }

    .hero {
      text-align: center;
      padding: 45px 15px;
      background: #f6f0e6;
    }

    .products {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      padding: 25px;
    }

    .product {
      width: 230px;
      padding: 15px;
      text-align: center;
      border: 1px solid #ddd;
      border-radius: 8px;
    }

    .product img {
      width: 100%;
      height: 200px;
      object-fit: contain;
    }

    button {
      background: #171717;
      color: white;
      border: none;
      padding: 12px 20px;
      cursor: pointer;
    }

    footer {
      background: #171717;
      color: white;
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>

  <header>
    <h1>میری پرفیوم شاپ</h1>
    <p>خوشبوئی جو آپ کی پہچان بنے</p>
  </header>

  <nav>
    <a href="#">ہوم</a>
    <a href="#products">پرفیومز</a>
    <a href="#contact">رابطہ</a>
    <a href="#cart">کارٹ: <span id="count">0</span></a>
  </nav>

  <section class="hero">
    <h2>اپنی پسند کی خوشبو منتخب کریں</h2>
    <p>معیاری پرفیومز مناسب قیمت پر</p>
    <a href="#products">
      <button>ابھی خریدیں</button>
    </a>
  </section>

  <section id="products">
    <h2 style="text-align:center">ہمارے پرفیومز</h2>

    <div class="products">
      <div class="product">
        <img src="https://placehold.co/300x300?text=Perfume+1"
             alt="پرفیوم نمبر ایک">
        <h3>پریمیم پرفیوم</h3>
        <p>قیمت: 2500 روپے</p>
        <button onclick="addToCart()">کارٹ میں شامل کریں</button>
      </div>

      <div class="product">
        <img src="https://placehold.co/300x300?text=Perfume+2"
             alt="پرفیوم نمبر دو">
        <h3>لگژری پرفیوم</h3>
        <p>قیمت: 3500 روپے</p>
        <button onclick="addToCart()">کارٹ میں شامل کریں</button>
      </div>
    </div>
  </section>

  <section id="cart" style="text-align:center;padding:20px">
    <h2>آپ کی شاپنگ کارٹ</h2>
    <p>منتخب پروڈکٹس: <span id="cartCount">0</span></p>
  </section>

  <footer id="contact">
    <p>رابطہ کریں: اپنا فون نمبر یہاں لکھیں</p>
    <p>© 2026 میری پرفیوم شاپ</p>
  </footer>

  <script>
    let count = 0;

    function addToCart() {
      count++;
      document.getElementById("count").textContent = count;
      document.getElementById("cartCount").textContent = count;
    }
  </script>

</body>
</html>
