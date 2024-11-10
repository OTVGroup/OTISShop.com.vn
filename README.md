<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>OTISShop</title>
    <link rel="stylesheet" href="style.css" />
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f4f4f4; /* Màu nền chính */
        color: #333; /* Màu chữ chính */
      }
      /* Phần logo và giới thiệu website */
      .header {
        background-color: #0044cc; /* Nền màu xanh dương */
        color: white;
        padding: 20px;
        text-align: center;
      }
      .header img {
        width: 150px; /* Đặt kích thước của logo */
        height: 150px; /* Đảm bảo chiều cao logo bằng chiều rộng */
        border-radius: 50%; /* Biến logo thành hình tròn */
        object-fit: cover; /* Giữ tỷ lệ ảnh khi cắt */
      }
      .header h1 {
        margin: 10px 0;
        font-size: 3em; /* Tăng kích thước chữ */
      }
      .header p {
        font-size: 1.2em; /* Tăng kích thước chữ mô tả */
        color: #ffd700; /* Màu vàng cho mô tả */
      }
      /* Phần chứa sản phẩm */
.container {
  display: grid;
  grid-template-columns: repeat(4, 1fr); /* Mặc định hiển thị 4 cột */
  gap: 20px;
  padding: 10px;
  padding-bottom: 20px;
  justify-items: center; /* Căn giữa các sản phẩm */
}

@media (max-width: 1200px) {
  .container {
    grid-template-columns: repeat(3, 1fr); /* Hiển thị 3 cột khi màn hình nhỏ hơn 1200px */
  }
}

@media (max-width: 900px) {
  .container {
    grid-template-columns: repeat(2, 1fr); /* Hiển thị 2 cột khi màn hình nhỏ hơn 900px */
  }
}
      .product {
        background-color: white;
        padding: 20px;
        margin: 10px;
        width: 200px;
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
        text-align: center;
        border-radius: 8px;
        transition: transform 0.3s ease;
      }
      .product:hover {
        transform: translateY(-10px); /* Hiệu ứng hover cho sản phẩm */
      }
      .product img {
        width: 200px;
        height: auto;
        border-radius: 8px;
      }
      .product h3 {
        font-size: 1.3em;
        color: #0044cc; /* Màu tiêu đề sản phẩm */
      }
      .product p {
        font-size: 1em;
        color: #555;
      }
      .product .price {
        font-size: 1.2em;
        color: #e60000; /* Màu đỏ cho giá sản phẩm */
        margin: 10px 0;
      }
      .order-btn {
        display: inline-block;
        background-color: #28a745; /* Nút đặt hàng màu xanh lá */
        color: white;
        padding: 10px 20px;
        text-decoration: none;
        border-radius: 5px;
        transition: background-color 0.3s ease;
      }
      .order-btn:hover {
        background-color: #218838; /* Hiệu ứng hover cho nút đặt hàng */
      }
      .copy-btn {
        display: inline-block;
        background-color: #007bff; /* Nút sao chép màu xanh dương */
        color: white;
        padding: 5px 10px;
        text-decoration: none;
        border-radius: 5px;
        margin-top: 10px;
        transition: background-color 0.3s ease;
      }
      .copy-btn:hover {
        background-color: #0056b3; /* Hiệu ứng hover cho nút sao chép */
      }
      /* Phần footer */
      .footer {
        background-color: #333; /* Nền footer màu xám đen */
        color: white;
        padding: 20px;
        text-align: center;
        position: relative;
        width: 100%;
        bottom: 0;
      }
      .footer a {
        color: #ffea00; /* Liên kết màu vàng */
        text-decoration: none;
      }
      .footer a:hover {
        text-decoration: underline;
      }
    </style>
  </head>
  <body>
    <!-- Phần logo và giới thiệu website -->
    <div class="header">
      <img
        src="https://i.pinimg.com/474x/df/2f/de/df2fdeef83868e15085ae4c7e4b9d396.jpg"
        alt="Logo OTISShop"
      />
      <h1>Chào mừng bạn đến với OTISShop</h1>
      <p>
        Khám phá các sản phẩm chất lượng và giá cả phải chăng tại cửa hàng của
        chúng tôi.
      </p>
    </div>
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 1" />
        <h3>Sản phẩm 1</h3>
        <p>Mô tả sản phẩm.</p>
        <p class="price">Giá: 100,000 VND</p>
        <a href="https://m.me/460099260527241" target="_blank" class="order-btn"
          >Đặt hàng</a
        >
        <a
          href="#"
          class="copy-btn"
          onclick="copyProductInfo('Sản phẩm 1', '100,000 VND', 'Mô tả chi tiết sản phẩm 1.')"
          >Sao chép thông tin</a
        >
      </div>
      <!-- Sản phẩm 2 -->
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 2" />
        <h3>Sản phẩm 2</h3>
        <p>Mô tả sản phẩm.</p>
        <p class="price">Giá: 150,000 VND</p>
        <a href="https://m.me/460099260527241" target="_blank" class="order-btn"
          >Đặt hàng</a
        >
        <a
          href="#"
          class="copy-btn"
          onclick="copyProductInfo('Sản phẩm 2', '150,000 VND', 'Mô tả chi tiết sản phẩm 2.')"
          >Sao chép thông tin</a
        >
      </div>
      <!-- Sản phẩm 3 -->
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 3" />
        <h3>Sản phẩm 3</h3>
        <p>Mô tả sản phẩm.</p>
        <p class="price">Giá: 200,000 VND</p>
        <a href="https://m.me/460099260527241" target="_blank" class="order-btn"
          >Đặt hàng</a
        >
        <a
          href="#"
          class="copy-btn"
          onclick="copyProductInfo('Sản phẩm 3', '200,000 VND', 'Mô tả chi tiết sản phẩm 3.')"
          >Sao chép thông tin</a
        >
      </div>
      <!-- Sản phẩm 4 -->
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 4" />
        <h3>Sản phẩm 4</h3>
        <p>Mô tả sản phẩm.</p>
        <p class="price">Giá: 250,000 VND</p>
        <a href="https://m.me/460099260527241" target="_blank" class="order-btn"
          >Đặt hàng</a
        >
        <a
          href="#"
          class="copy-btn"
          onclick="copyProductInfo('Sản phẩm 4', '250,000 VND', 'Mô tả chi tiết sản phẩm 4.')"
          >Sao chép thông tin</a
        >
      </div>
      <!-- Sản phẩm 5 -->
      <div class="product">
        <img src="https://via.placeholder.com/200" alt="Sản phẩm 5" />
        <h3>Sản phẩm 5</h3>
        <p>Mô tả sản phẩm.</p>
        <p class="price">Giá: 120,000 VND</p>
        <a href="https://m.me/460099260527241" target="_blank" class="order-btn"
          >Đặt hàng</a
        >
        <a
          href="#"
          class="copy-btn"
          onclick="copyProductInfo('Sản phẩm 5', '120,000 VND', 'Mô tả chi tiết sản phẩm 5.')"
          >Sao chép thông tin</a
        >
      </div>
    </div>
    <div class="footer">
      <p>
        <a href="https://www.facebook.com/OtisSeller" target="_blank">Fanpage</a
        >,
        <a href="https://www.instagram.com/otisvo586" target="_blank"
          >Instagram</a
        >,
        <a href="https://www.tiktok.com/@o2v_586" target="_blank">Threads</a>,
        <a href="https://www.threads.net/@otisvo586" target="_blank">TikTok</a>
      </p>
      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>,
        Điện thoại:
        <a href="tel:0329022431">0329022431</a>
      </p>
      <p>
        Địa chỉ:
        <a href="https://maps.app.goo.gl/hjFTnBm2Her5mJyd7" target="_blank"
          >2252/22/12.Tổ2, Kp1, Tân Chánh Hiệp, Q12, TP.HCM, Việt Nam</a
        >
      </p>
    </div>
    <script>
      function copyProductInfo(name, price, description) {
        const productInfo = `Sản phẩm: ${name}\nGiá: ${price}\nMô tả: ${description}`;
        navigator.clipboard.writeText(productInfo).then(
          function () {
            alert("Thông tin sản phẩm đã được sao chép!");
          },
          function (err) {
            alert("Có lỗi xảy ra, không sao chép được!");
          }
        );
      }
    </script>
  </body>
</html>
