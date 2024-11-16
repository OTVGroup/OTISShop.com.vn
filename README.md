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
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-image: url("https://i.pinimg.com/474x/bf/58/e7/bf58e7025454d9e51a005147f3225668.jpg");
        background-size: cover;
        background-repeat: repeat;

        background-position: center;
        background-color: #f0f0f0;
        color: #000000;
        width: 100%;

        margin: 0 auto;
      }

      /* Phần logo */
      .header {
        text-align: center;
        width: 100%;
        margin: 40px 0 0 0;
        font-size: 24px;
      }
      .header img {
        width: 300px;
        height: auto;
        border-radius: 50%;
        object-fit: cover;
      }

      .header img:hover {
        transform: scale(1.1);
        transition: transform 0.5s ease;
        box-shadow: 0px 6px 10px #000000;
      }

      /* Phần chứa sản phẩm */
      .container {
        display: flex;
        flex-direction: column; /* Sắp xếp các phần tử con theo chiều dọc */
        gap: 10px; /* Khoảng cách giữa các phần tử */
        padding: 10px; /* Khoảng cách bên trong container */
        align-items: center; /* Căn giữa các phần tử con theo chiều ngang */
        justify-content: flex-start; /* Căn các phần tử con theo chiều dọc (mặc định là từ trên xuống) */
      }

      /* Phần hiển thị sản phẩm */
      .product-row {
        width: 450px; /* Chiều rộng cố định */
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(208, 241, 239);
        padding: 10px;
        border-radius: 10px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
        border: 4px solid black;
      }
      .product-left img {
        width: 400px;
        height: 320px;
        object-fit: cover;
        border-radius: 10px;
      }

      .product-left h3 {
        margin: 4px 0;
        font-size: 1.8em;
      }
      .product-left .price {
        color: #ff0000c4;
        margin: 4px 0;
        font-size: 1.5em;
      }
      /* Nút điều hướng */
      .product-actions {
        display: flex; /* Thiết lập container làm flexbox */
        justify-content: center; /* Căn giữa các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều dọc (nếu cần) */
      }
      .product-actions img {
        width: 50px;
        height: 50px;
        border: 2px solid #000000;
        border-radius: 50%;
        margin: 0 20px 0 20px;
      }
      .OUT {
        margin: 4px 4px 4px 4px;
        border-radius: 8px;
        background-color: #fb513bae;
      }
      .OUT:hover {
        background-color: #c7140ecd;
      }
      .oder {
        margin: 4px 4px 4px 4px;
        height: 50px;
        width: auto;
        border-radius: 8px;
        background-color: #58e139;
      }
      .oder:hover {
        background-color: #04a504;
      }
      .save {
        margin: 4px 4px 4px 4px;
        height: 50px;
        width: auto;
        border-radius: 8px;
        background-color: #4989ff;
      }
      .save:hover {
        background-color: #1653cdc4;
      }
      .link {
        margin: 4px 4px 4px 4px;
        height: 50px;
        width: auto;
        border-radius: 8px;
        background-color: #e75ef6;
      }
      .link:hover {
        background-color: #c40ec4;
      }
      .OUT,
      .oder,
      .save,
      .link a {
        font-size: 22px;
      }
      /* Phần floating icons */
      .shopping,
      .chatting,
      .voucher,
      .content {
        position: fixed;
        width: 100px;
        height: auto;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: transform 0.5s ease;
        border: 4px solid black;
      }
      .shopping {
        bottom: 380px;
        right: 20px;
      }
      .voucher {
        bottom: 260px;
        right: 20px;
      }
      .chatting {
        bottom: 140px;
        right: 20px;
      }
      .content {
        bottom: 20px;
        right: 20px;
      }
      .shopping:hover,
      .chatting:hover,
      .voucher:hover,
      .content:hover {
        transform: scale(1.2);
        box-shadow: 0 3px 10px #000000;
      }
      .shopping img,
      .chatting img,
      .voucher img,
      .content img {
        width: 100px;
        height: auto;
        object-fit: cover;
        border-radius: 50%;
      }
      /* Hộp thông tin, ẩn ban đầu */
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting {
        display: none; /* Ẩn khi chưa nhấn vào logo */
        position: fixed;
        background-color: #e3e3e3;
        border: 4px solid #000000;
        border-radius: 16px;
        padding: 20px;
        width: 480px;
        top: 50%;
        left: 50%;
        transform: translate(
          -50%,
          -50%
        ); /* Dịch chuyển để căn giữa chính xác */
        box-shadow: 0 8px 12px rgba(0, 0, 0, 0.1);
        transition: transform 2s ease;
        border: 0.5px solid black;
        z-index: 999;
      }
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting h2 {
        margin: 10px 0;
        font-size: 36px;
        color: #000000;
        text-align: left;
      }
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting p {
        margin: 10px 0;
        font-size: 24px;
        color: #000000;
        text-align: left;
      }
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting li {
        margin: 10px 0;
        font-size: 24px;
        color: #000000;
        text-align: left;
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
      <h2>Welcome To OTISShop</h2>
    </div>
    <hr />

    <!-- Sản phẩm OTISShop -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
          <h3>Sản phẩm 1</h3>
          <div class="price">Giá: 100,000 VND</div>
          <div class="product-actions">
            <button
              class="oder"
              onclick="window.open('https://www.messenger.com/t/460099260527241?', '_blank')"
            >
              <a>Đặt</a></button
            ><img
              src="https://i.pinimg.com/474x/df/2f/de/df2fdeef83868e15085ae4c7e4b9d396.jpg"
              alt="Shopee"
            />
            <button class="save" onclick="copyProductInfo('OS-0101')">
              <a>Lưu</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Thêm các sản phẩm khác tương tự ở đây -->
    </div>
    <hr />

    <!-- Sản phẩm Liên Kết Shopee -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
          <h3>Sản phẩm 1</h3>
          <div class="price">Giá: 100,000 VND</div>
          <div class="product-actions">
            <button
              class="link"
              onclick="window.open('  /* Link sản phẩm */', '_blank')"
            >
              <a>Link</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button class="save" onclick="copyProductInfo('SP-0101')">
              <a>Lưu</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Thêm các sản phẩm khác tương tự ở đây -->
    </div>
    <br />
    <!-- Logo để mở/ẩn phần Thông Tin -->
    <div class="content" onclick="toggleContact('contactContent')">
      <img
        src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
        alt="content"
      />
    </div>
    <!-- Nội dung Thông Tin -->
    <div class="contact-Content" id="contactContent">
      <h2>
        Chi tiết!
        <button class="OUT" onclick="toggleContact('contactContent')">
          <a>X</a>
        </button>
      </h2>
      <p>Hotline: <a href="tel:0329022431">0329022431</a></p>
      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
      </p>
      <p>
        Fanpage:
        <a href="https://www.messenger.com/t/460099260527241?" target="_blank"
          >https://.../OtisSeller</a
        >.
      </p>
      <p>
        Địa Chỉ:
        <a href="https://maps.app.goo.gl/pyLNvcmZvLtHrBtT7"
          >2252/22/12.Tổ 2, Kp1, Tân Chánh Hiệp, Q.12, TP.HCM, Việt Nam</a
        >.
      </p>
    </div>
    <!-- Logo để mở/ẩn phần Shopping-->
    <div class="shopping" onclick="toggleContact('contactShopping')">
      <img
        src="https://i.pinimg.com/474x/f7/22/3e/f7223e8daaee44645802955532e1c372.jpg"
        alt="shopping"
      />
    </div>
    <!-- Nội dung Shopping-->
    <div class="contact-Shopping" id="contactShopping">
      <h2>
        Giỏ hàng!
        <button class="OUT" onclick="toggleContact('contactShopping')">
          <a>X</a>
        </button>
        <button
          class="oder"
          onclick="window.open('https://www.messenger.com/t/460099260527241?', '_blank')"
        >
          <a>Đặt</a>
        </button>
      </h2>
      <p>
        <li>
          Bấm 'Lưu' để lưu mã sản phẩm vào 'Clipboard' trước khi bấm 'Đặt'!
        </li>
        <li>
          Bấm 'Đặt' và gửi mã sản phẩm cho chúng tôi thông qua Fanpage của
          OTISShop!
        </li>
        <li>Chỉ hổ trợ tư vấn chứ không bán sản phẩm liên kết Shopee!</li>
        <br />
        <a>- - - Chân Thành Cảm Ơn Quý Khách! - - -</a>
      </p>
    </div>
    <!-- Logo để mở/ẩn phần Chatting -->
    <div class="chatting" onclick="toggleContact('contactChatting')">
      <img
        src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
        alt="chatting"
      />
    </div>
    <!-- Nội dung Chatting -->
    <div class="contact-Chatting" id="contactChatting">
      <h2>
        Hổ trợ!
        <button class="OUT" onclick="toggleContact('contactChatting')">
          <a>X</a>
        </button>
      </h2>
      <p>
        <li>Hổ trợ tư vấn sản phẩm.</li>
        <li>Liên kết bán hàng - Tư vấn sản phẩm.</li>
        <li>Hổ trợ quảng cáo - Tiếp thị sản phẩm.</li>
      </p>
      <hr />
      <p>Hotline: <a href="tel:0329022431" target="_blank">0329022431</a>.</p>
      <p>
        Fanpage:
        <a href="https://www.messenger.com/t/460099260527241?" target="_blank"
          >https://.../OtisSeller</a
        >.
      </p>
      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>.
      </p>
    </div>

    <!-- Logo để mở/ẩn phần Voucher -->
    <div class="voucher" onclick="toggleContact('contactVoucher')">
      <img
        src="https://i.pinimg.com/474x/38/ea/d6/38ead648ede5fb91f29b086f22396613.jpg"
        alt="voucher"
      />
    </div>
    <!-- Nội dung Voucher (ẩn mặc định) -->
    <div class="contact-Voucher" id="contactVoucher">
      <h2>
        OTISShop Voucher!
        <button class="OUT" onclick="toggleContact('contactVoucher')">
          <a>X</a>
        </button>
      </h2>
      <p>
        <li>Hiện tại chưa có Voucher, vui lòng quay lại sau!</li>
      </p>
    </div>

    <script>
      // Biến toàn cục để lưu các mã sản phẩm đã được chọn
      let selectedProductCodes = [];

      // Hàm để sao chép mã sản phẩm
      function copyProductInfo(name) {
        // Kiểm tra xem mã sản phẩm đã tồn tại trong danh sách chưa
        if (selectedProductCodes.includes(name)) {
          alert("Mã sản phẩm đã tồn tại!");
        } else {
          // Thêm mã sản phẩm vào danh sách đã chọn
          selectedProductCodes.push(name);

          // Tạo chuỗi các mã sản phẩm cách nhau bằng dấu phẩy
          const newText = selectedProductCodes.join(", "); // Join mảng thành một chuỗi, cách nhau bằng dấu phẩy

          // Sao chép chuỗi vào clipboard
          navigator.clipboard.writeText(newText).then(
            function () {
              alert("Lưu mã sản phẩm thành công! Vui lòng chọn 'Giỏ Hàng'!");
            },
            function (err) {
              alert("Không thể lưu mã sản phẩm! Vui lòng thử lại!");
            }
          );
        }
      }

      function toggleContact(contentID) {
        var content = document.getElementById(contentID);
        var content1 = document.getElementById("contactContent");
        var content2 = document.getElementById("contactChatting");
        var content3 = document.getElementById("contactVoucher");
        var content4 = document.getElementById("contactShopping");

        // Ẩn tất cả các phần tử khác trước khi hiển thị phần tử mới
        if (contentID === "contactContent") {
          content2.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
        }
        if (contentID === "contactChatting") {
          content1.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
        }
        if (contentID === "contactVoucher") {
          content1.style.display = "none";
          content2.style.display = "none";
          content4.style.display = "none";
        }
        if (contentID === "contactShopping") {
          content1.style.display = "none";
          content2.style.display = "none";
          content3.style.display = "none";
        }
        // Chuyển đổi trạng thái hiển thị của phần tử được chọn
        if (content.style.display !== "block") {
          content.style.display = "block";
        } else {
          content.style.display = "none";
        }
      }
    </script>
  </body>
</html>
