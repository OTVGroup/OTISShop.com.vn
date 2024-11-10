<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta
      name="description"
      content="OTISShop - Cửa hàng trực tuyến với các sản phẩm chất lượng và giá cả phải chăng."
    />
    <meta name="author" content="OTISShop" />
    <title>OTISShop</title>
    <link rel="stylesheet" href="style.css" />
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-color: #f4f4f4;
        color: #333;
      }

      /* Phần logo và giới thiệu website */
      .header {
        background-color: #0044cc;
        color: white;
        padding: 20px;
        text-align: center;
      }

      .header img {
        width: 150px;
        height: 150px;
        border-radius: 50%;
        object-fit: cover;
      }

      .header h1 {
        margin: 10px 0;
        font-size: 2.5em;
      }

      .header p {
        font-size: 1.2em;
        color: #ffd700;
      }

      /* Phần chứa sản phẩm */
      .container {
        display: flex;
        flex-direction: column;
        gap: 40px;
        padding: 10px;
      }

      .product-row {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        background-color: white;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
        margin: 10px 0;
      }

      /* Khung bên trái (Ảnh, Tên, Giá, Nút) */
      .product-left {
        flex: 0 0 160px;
        display: flex;
        flex-direction: column;
        gap: 10px;
        align-items: center;
      }

      .product-left img {
        width: 160px;
        height: 90px;
        object-fit: cover;
        border-radius: 8px;
      }

      .product-left h3 {
        font-size: 1.3em;
        color: #0044cc;
        margin: 0;
      }

      .product-left .price {
        font-size: 1.2em;
        color: #e60000;
        margin: 0;
      }

      .product-actions {
        display: flex;
        gap: 10px;
        margin-top: 10px;
      }

      .order-btn,
      .save-btn {
        display: inline-block;
        padding: 10px 20px;
        text-decoration: none;
        border-radius: 5px;
        transition: background-color 0.3s ease;
      }

      .order-btn {
        background-color: #28a745;
        color: white;
      }

      .order-btn:hover {
        background-color: #218838;
      }

      .save-btn {
        background-color: #007bff;
        color: white;
      }

      .save-btn:hover {
        background-color: #0056b3;
      }

      /* Khung bên phải (Mô tả sản phẩm) */
      .product-right {
        flex: 1;
        padding-left: 20px;
        width: 60%;
        display: flex;
        align-items: flex-start;
        justify-content: flex-start;
        overflow: hidden;
        /* Xóa vạch phân cách */
        /* border-left: 2px solid #cccccc; */
      }

      .product-description {
        font-size: 1em;
        color: #555;
        line-height: 1.6;
      }

      /* Phần footer */
      .footer {
        background-color: #333;
        color: white;
        padding: 20px;
        text-align: center;
        position: relative;
        width: 100%;
        bottom: 0;
      }

      .footer a {
        color: #ffea00;
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

    <!-- Phần sản phẩm -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/160x90" alt="Sản phẩm 1" />
          <h3 class="name">Sản phẩm 1</h3>
          <p class="price">Giá: 100,000 VND</p>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a
              href="#"
              class="save-btn"
              onclick="copyProductInfo('Sản phẩm 1', '100,000 VND', 'Mô tả chi tiết sản phẩm 1.')"
              >Lưu</a
            >
          </div>
        </div>
        <div class="product-right">
          <div class="product-description">
            <p>
              Thông tin chi tiết về sản phẩm 1 sẽ được cung cấp ở đây. Bạn có
              thể mô tả thêm về đặc điểm, công dụng, hoặc hướng dẫn sử dụng của
              sản phẩm này.
            </p>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 2 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/160x90" alt="Sản phẩm 2" />
          <h3 class="name">Sản phẩm 2</h3>
          <p class="price">Giá: 150,000 VND</p>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a
              href="#"
              class="save-btn"
              onclick="copyProductInfo('Sản phẩm 2', '150,000 VND', 'Mô tả chi tiết sản phẩm 2.')"
              >Lưu</a
            >
          </div>
        </div>
        <div class="product-right">
          <div class="product-description">
            <p>
              Thông tin chi tiết về sản phẩm 2 sẽ được cung cấp ở đây. Bạn có
              thể mô tả thêm về đặc điểm, công dụng, hoặc hướng dẫn sử dụng của
              sản phẩm này.
            </p>
          </div>
        </div>
      </div>

      <!-- Thêm các sản phẩm khác vào đây theo mẫu -->
    </div>

    <!-- Phần footer -->
    <div class="footer">
      <p>&copy; 2024 OTISShop. Tất cả quyền lợi được bảo lưu.</p>
      <p>
        <a href="https://www.facebook.com/otus.shop" target="_blank"
          >Facebook</a
        >
        | <a href="mailto:info@otisshop.com">Email</a>
      </p>
    </div>

    <script>
      function copyProductInfo(name, price, description) {
        const text = `Tên sản phẩm: ${name}\nGiá: ${price}\nMô tả: ${description}`;
        navigator.clipboard.writeText(text).then(() => {
          alert("Đã lưu thông tin sản phẩm!");
        });
      }
    </script>
  </body>
</html>
