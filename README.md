<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trang Web Bán Hàng</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Thanh điều hướng -->
  <nav>
    <div class="logo">Shop của tôi</div>
    <div class="cart" onclick="toggleCart()">
      <span>Giỏ hàng (0)</span>
    </div>
  </nav>
  <!-- Danh sách sản phẩm -->
  <section class="product-list">
    <div class="product">
      <div class="product-image">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 1">
      </div>
      <div class="product-details">
        <h3>Sản phẩm 1</h3>
        <p class="price">Giá: 100.000 VND</p>
        <p class="description">Đây là mô tả chi tiết của sản phẩm 1. Đây là sản phẩm tuyệt vời với chất lượng cao.</p>
        <button onclick="addToCart('Sản phẩm 1', 100000)">Thêm vào giỏ</button>
      </div>
    </div>
    <div class="product">
      <div class="product-image">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 2">
      </div>
      <div class="product-details">
        <h3>Sản phẩm 2</h3>
        <p class="price">Giá: 200.000 VND</p>
        <p class="description">Đây là mô tả chi tiết của sản phẩm 2. Một sản phẩm cao cấp với tính năng tuyệt vời.</p>
        <button onclick="addToCart('Sản phẩm 2', 200000)">Thêm vào giỏ</button>
      </div>
    </div>
    <div class="product">
      <div class="product-image">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 3">
      </div>
      <div class="product-details">
        <h3>Sản phẩm 3</h3>
        <p class="price">Giá: 300.000 VND</p>
        <p class="description">Đây là mô tả chi tiết của sản phẩm 3. Với thiết kế hiện đại và tính năng vượt trội.</p>
        <button onclick="addToCart('Sản phẩm 3', 300000)">Thêm vào giỏ</button>
      </div>
    </div>
  </section>
  <!-- Giỏ hàng -->
  <div class="cart-popup" id="cart-popup">
    <h2>Giỏ hàng</h2>
    <ul id="cart-items">
      <!-- Các sản phẩm sẽ được thêm vào đây -->
    </ul>
    <p id="total-price">Tổng: 0 VND</p>
    <button onclick="checkout()">Thanh toán</button>
    <button onclick="closeCart()">Đóng</button>
  </div>
  <script src="script.js"></script>
</body>
</html>
