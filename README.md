<!DOCTYPE html>
<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta
      name="description"
      content="OTISShop - Chất Lượng, Uy Tín, Tin Cậy."
    />
    <meta name="author" content="OTISShop" />
    <title>OTISShop</title>
    <style>
      /* Cấu hình chung cho body */
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
        background-image: url("https://i.pinimg.com/474x/bf/58/e7/bf58e7025454d9e51a005147f3225668.jpg");
        color: #000000;
      }

      /* Phần logo */
      .header {
        text-align: center;
        padding: 20px;
      }

      .header img {
        width: 90px;
        height: 90px;
        border-radius: 50%;
        object-fit: cover;
      }

      .header h1 {
        font-size: 1.5em;
        color: #000000;
      }

      .header h3 {
        font-size: 1em;
        color: #000000;
      }

      /* Phần chứa sản phẩm */
      .container {
        display: flex;
        flex-wrap: wrap; /* Cho phép sản phẩm nằm ở nhiều hàng */
        gap: 10px;
        padding: 10px;
        max-width: 100%;
        margin: auto;
        justify-content: center;
      }

      /* Phần hiển thị sản phẩm */
      .product-row {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(208, 241, 239);
        padding: 15px;
        border-radius: 10px;
        width: 120px; /* Đảm bảo mỗi sản phẩm có kích thước cố định */
        text-align: center;
      }

      .product-left img {
        width: 100px;
        height: 100px;
        object-fit: cover;
        border-radius: 10px;
      }

      .product-left h3 {
        font-size: 1em;
        color: #0044cc;
        margin: 10px 0;
      }

      .product-left .category {
        font-size: 0.8em;
        color: #ff00e1;
        margin: 5px 0;
      }

      .product-left .price {
        font-size: 0.8em;
        color: #ff0000c4;
        margin: 10px 0;
      }

      .product-actions {
        display: flex;
        gap: 10px;
        margin-top: 10px;
      }

      .order-btn,
      .save-btn {
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

      /* Phần footer */
      .footer {
        background-color: #333;
        color: white;
        padding: 5px;
        text-align: center;
        width: 100%;
      }

      .footer a {
        color: #ffea00;
        text-decoration: none;
      }

      .footer a:hover {
        text-decoration: underline;
      }
      .shopping-float {
        position: fixed;
        bottom: 175px; /* Căn cách lề dưới 20px */
        right: 10px; /* Căn cách lề phải 20px */
        width: 50px;
        height: 50px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 1000; /* Đảm bảo nút luôn ở trên các thành phần khác */
        transition: transform 0.3s ease;
        border: 2px solid black; /* Thêm viền đen */
      }

      .shopping-float:hover {
        transform: scale(1.1); /* Tăng kích thước khi di chuột */
      }

      .shopping-float img {
        width: 50px;
        height: 50px;
        object-fit: cover;
        border-radius: 50%;
      }

      .chatting-float {
        position: fixed;
        bottom: 235px; /* Căn cách lề dưới 20px */
        right: 10px; /* Căn cách lề phải 20px */
        width: 50px;
        height: 50px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 1000; /* Đảm bảo nút luôn ở trên các thành phần khác */
        transition: transform 0.3s ease;
        border: 2px solid black; /* Thêm viền đen */
      }

      .chatting-float:hover {
        transform: scale(1.1); /* Tăng kích thước khi di chuột */
      }

      .chatting-float img {
        width: 50px;
        height: 50px;
        object-fit: cover;
        border-radius: 50%;
      }
      .ADS-float {
        position: fixed;
        bottom: 295px; /* Căn cách lề dưới 20px */
        right: 10px; /* Căn cách lề phải 20px */
        width: 50px;
        height: 50px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: 1000; /* Đảm bảo nút luôn ở trên các thành phần khác */
        transition: transform 0.3s ease;
        border: 2px solid black; /* Thêm viền đen */
      }

      .ADS-float:hover {
        transform: scale(1.1); /* Tăng kích thước khi di chuột */
      }

      .ADS-float img {
        width: 50px;
        height: 50px;
        object-fit: cover;
        border-radius: 50%;
      }
    </style>
  </head>
  <body>
    <!-- Phần logo -->
    <div class="header">
      <img
        src="https://i.pinimg.com/474x/df/2f/de/df2fdeef83868e15085ae4c7e4b9d396.jpg"
        alt="Logo OTISShop"
      />
      <h1>Welcome to OTISShop</h1>
      <h3>Chất Lượng - Uy Tín - Tin Cậy</h3>
    </div>

    <!-- Phần footer phân loại-->
    <div class="footer">
      <p>Sản phẩm cung cấp bới <a href="https://shopee.vn">Shopee</a>!</p>
    </div>

    <!-- Phần sản phẩm -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
          <h3>Sản phẩm 1</h3>

          <div class="price">Giá: 100,000 VND</div>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a href="#" class="save-btn" onclick="copyProductInfo('OS-####01')"
              >Lưu</a
            >
          </div>
        </div>
      </div>

      <!-- Sản phẩm 2 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 2" />
          <h3>Sản phẩm 2</h3>

          <div class="price">Giá: 150,000 VND</div>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a href="#" class="save-btn" onclick="copyProductInfo('OS-####02')"
              >Lưu</a
            >
          </div>
        </div>
      </div>
    </div>
    <!-- Phần footer phân loại-->
    <div class="footer">
      <p>
        Sản phẩm cung cấp bới
        <a href="https://www.messenger.com/t/460099260527241">OTISShop</a>!
      </p>
    </div>
    <div class="container">
      <!-- Sản phẩm 3 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 3" />
          <h3>Sản phẩm 3</h3>

          <div class="price">Giá: 200,000 VND</div>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241&"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a href="#" class="save-btn" onclick="copyProductInfo('OS-####003')"
              >Lưu</a
            >
          </div>
        </div>
      </div>

      <!-- Sản phẩm 4 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 4" />
          <h3>Sản phẩm 4</h3>

          <div class="price">Giá: 180,000 VND</div>
          <div class="product-actions">
            <a
              href="https://www.messenger.com/t/460099260527241"
              target="_blank"
              class="order-btn"
              >Đặt</a
            >
            <a href="#" class="save-btn" onclick="copyProductInfo('OS-####04')"
              >Lưu</a
            >
          </div>
        </div>
      </div>
    </div>
    <!--Phần Shoping Icon-->
    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20muốn%20mua%20sản%20phẩm?"
      target="_blank"
      class="shopping-float"
    >
      <img
        src="https://i.pinimg.com/474x/f7/22/3e/f7223e8daaee44645802955532e1c372.jpg"
        alt="Shopping"
      />
    </a>
    <!--Phần Chatting Icon-->
    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20có%20một%20vài%20vấn%20đề?"
      target="_blank"
      class="chatting-float"
    >
      <img
        src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
        alt="Chatting"
      />
    </a>
    <!--Phần ADS Icon-->
    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20muốn%20hợp%20tác%20quảng%20cáo?"
      target="_blank"
      class="ADS-float"
    >
      <img
        src="https://i.pinimg.com/474x/38/ea/d6/38ead648ede5fb91f29b086f22396613.jpg"
        alt="ADS"
      />
    </a>
    <!-- Phần footer -->
    <div class="footer">
      <p>&copy; 2024 OTISShop. Tất cả quyền lợi được bảo lưu.</p>
      <p>
        Hotline: <a href="tel:0329022431">0329022431</a> | Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
      </p>
      <p>
        <a href="https://www.facebook.com/OtisSeller" target="_blank"
          >Fanpage</a
        >
        | <a href="https://www.tiktok.com/@o2v_586" target="_blank">TikTok</a> |
        <a href="https://www.instagram.com/otisvo586" target="_blank"
          >Instagram</a
        >
        |
        <a href="https://www.threads.net/@otisvo586" target="_blank">Threads</a>
      </p>
      <p>
        Địa chỉ:
        <a href="2252/22/12. Tổ 2, Kp1, Quận 12, Hồ Chí Minh, Việt Nam"
          >2252/22/12. Tổ 2, Kp1, Q.12, TP.HCM</a
        >
      </p>
    </div>

    <script>
      // Chức năng lưu thông tin sản phẩm vào clipboard
      function copyProductInfo(name) {
        const text = `Mã sản phẩm: ${name}`;
        navigator.clipboard.writeText(text).then(
          function () {
            alert("Đã lưu mã sản phẩm, vui lòng chọn 'Giỏ hàng'!");
          },
          function (err) {
            alert("Có lỗi xảy ra, không thể lưu mã sản phẩm!");
          }
        );
      }
    </script>
  </body>
</html>
