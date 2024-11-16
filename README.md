<!DOCTYPE html>
<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta
      name="viewport"
      content="width=400px, height=820px, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0, user-scalable=no"
    />
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
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-image: url("https://i.pinimg.com/474x/bf/58/e7/bf58e7025454d9e51a005147f3225668.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        background-color: #f0f0f0;
        color: #000000;
      }

      /* Phần logo */
      .header,
      .header1 {
        text-align: center;
        width: 100%;
      }
      .header2 {
        text-align: center;
        width: 100%;
      }
      .header img {
        width: 75px;
        height: auto;
        border-radius: 50%;
        object-fit: cover;
      }

      .header img:hover {
        transform: scale(1.1);
        transition: transform 0.5s ease;
        box-shadow: 0px 3px 5px #000000;
      }

      /* Phần chứa sản phẩm */
      .container {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
        padding: 10px;
        justify-content: center;
      }

      /* Phần hiển thị sản phẩm */
      .product-row {
        width: 160px; /* Chiều rộng cố định */
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(208, 241, 239);
        padding: 5px;
        border-radius: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }

      .product-row:hover {
        border: 0.5px solid black;
        transition: transform 0.5s ease;
        width: 159px;
      }

      .product-left img {
        width: 150px;
        height: 120px;
        object-fit: cover;
        border-radius: 5px;
      }

      .product-left h3 {
        margin: 2px 0;
        font-size: 0.9em;
      }

      .product-left .price {
        color: #ff0000c4;
        margin: 2px 0;
        font-size: 0.8em;
      }

      /* Nút */
      .product-actions a,
      .product-actions button {
        font-size: 0.6em;
        color: white;
        font-size: 12px;
        padding: 5px 5px;
        border-radius: 5px;
        text-decoration: none;
      }
      .OUT {
        right: 2px;
        top: 2px;
      }
      .delete {
        background-color: #ff342d;
      }
      .delete:hover {
        background-color: #e20800;
      }
      .save {
        background-color: #007bff;
      }
      .save:hover {
        background-color: #0056b3;
      }

      /* Phần floating icons */
      .shopping,
      .chatting,
      .ADS,
      .contact-logo {
        position: fixed;
        width: 60px;
        height: auto;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: transform 0.5s ease;
        border: 2px solid black;
      }
      .shopping {
        bottom: 20px;
        left: 32.5%;
      }
      .chatting {
        bottom: 20px;
        right: 32.5%;
      }
      .ADS {
        bottom: 20px;
        right: 10%;
      }
      .shopping:hover,
      .chatting:hover,
      .ADS:hover,
      .contact-logo:hover {
        transform: scale(1.2);
        box-shadow: 0 3px 5px #000000;
      }
      .shopping img,
      .chatting img,
      .ADS img,
      .contact-logo img {
        width: 60px;
        height: 60px;
        object-fit: cover;
        border-radius: 50%;
      }
      /* Thông tin liên hệ*/
      /* Kiểu dáng cho logo, khi nhấn vào logo sẽ hiển thị nội dung liên hệ */
      .contact-logo {
        cursor: pointer;
        width: 60px;
        height: 60px;
        position: fixed;
        bottom: 20px; /* Đặt logo ở dưới cùng */
        left: 10%; /* Đặt logo ở lề trái */
        border-radius: 50%;
        justify-content: center;
      }
      /* Kiểu dáng cho hộp thông tin liên hệ, nằm ở lề phải và ẩn ban đầu */
      .contact-content,
      .contact-ADS,
      .contact-Shopping,
      .contact-Chatting {
        display: none; /* Ẩn hộp liên hệ khi chưa nhấn vào logo */
        position: fixed;
        background-color: #e3e3e3;
        border: 1px solid #000000;
        border-radius: 8px;
        padding: 15px;
        width: 25em;
        top: 50%;
        left: 50%;
        transform: translate(
          -50%,
          -50%
        ); /* Dịch chuyển để căn giữa chính xác */
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        transition: transform 2s ease;
        border: 0.5px solid black;
      }
      .contact-content,
      .contact-ADS,
      .contact-Shopping,
      .contact-Chatting h2 {
        margin-top: 0;
        font-size: 18px;
        color: #333;
        text-align: auto;
      }
      .contact-content,
      .contact-ADS,
      .contact-Shopping,
      .contact-Chatting,
      .contact-LuuY p {
        margin: 5px 0;
        font-size: 12px;
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
    </div>
    <div class="header1">
      <h2>Welcome To OTISShop</h2>
    </div>

    <!-- Sản phẩm -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
          <h3>Sản phẩm 1</h3>
          <div class="price">Giá: 100,000 VND</div>
          <div class="product-actions">
            <button class="delete" onclick="copyProductInfo('-SP1')">
              Xóa
            </button>
            <button class="save" onclick="copyProductInfo('+SP1')">Thêm</button>
          </div>
        </div>
      </div>

      <!-- Thêm các sản phẩm khác tương tự ở đây -->
    </div>
    <br /><br /><br />
    <!-- Logo để mở/ẩn phần nội dung liên hệ -->
    <div class="contact-logo" onclick="toggleContact('contactContent')">
      <img
        src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
        alt="contact-logo"
      />
    </div>
    <!-- Nội dung liên hệ (ẩn mặc định) -->
    <div class="contact-content" id="contactContent">
      <h2>
        Chi tiết
        <button class="OUT" onclick="toggleContact('contactContent')" ;>
          X
        </button>
      </h2>

      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
      </p>
      <p>Điện Thoại: <a href="tel:0329022431">0329022431</a></p>
      <p>
        Địa Chỉ:
        <a href="https://maps.app.goo.gl/pyLNvcmZvLtHrBtT7"
          >2252/22/12.Tổ 2, Kp1, Tân Chánh Hiệp, Q.12, TP.HCM, Việt Nam</a
        >
      </p>
    </div>
    <!-- Floating Buttons -->
    <div class="shopping" onclick="toggleContact('contactShopping')">
      <img
        src="https://i.pinimg.com/474x/f7/22/3e/f7223e8daaee44645802955532e1c372.jpg"
        alt="Shopping"
      />
    </div>
    <div class="contact-Shopping" id="contactShopping">
      <h2>
        Giỏ hàng
        <button class="OUT" onclick="toggleContact('contactShopping')">
          X
        </button>
        <button
          class="Oder"
          herf="https://www.messenger.com/t/460099260527241?"
        >
          Đặt
        </button>
      </h2>
      <p>OTISShop chỉ hổ trợ tư vấn cho sản phẩm liên kết Shopee!</p>
    </div>
    <!-- Nội dung Chatting (ẩn mặc định) -->
    <div class="chatting" onclick="toggleContact('contactChatting')">
      <img
        src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
        alt="Chatting"
      />
    </div>
    <div class="contact-Chatting" id="contactChatting">
      <h2>
        Hổ trợ khách hàng
        <button class="OUT" onclick="toggleContact('contactChatting')" ;>
          X
        </button>
      </h2>
      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
      </p>
      <p>Điện Thoại: <a href="tel:0329022431">0329022431</a></p>
      <p>Địa Chỉ: <a>1234 Example Street, City</a></p>
    </div>

    <!-- Nội dung ADS (ẩn mặc định) -->
    <div class="ADS" onclick="toggleContact('contactADS')">
      <img
        src="https://i.pinimg.com/474x/38/ea/d6/38ead648ede5fb91f29b086f22396613.jpg"
        alt="ADS"
      />
    </div>
    <div class="contact-ADS" id="contactADS">
      <h2>
        Liên hệ quảng cáo
        <button class="OUT" onclick="toggleContact('contactADS') " ;>X</button>
      </h2>
      <p>
        Email:
        <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
      </p>
      <p>Điện Thoại: <a href="tel:0329022431">0329022431</a></p>
      <p>Địa Chỉ: <a>1234 Example Street, City</a></p>
    </div>
    <script>
      function copyProductInfo(name) {
        // Lấy văn bản hiện tại từ clipboard (nếu có)
        navigator.clipboard
          .readText()
          .then((existingText) => {
            // Cộng dồn nội dung mới vào nội dung cũ
            const newText = existingText + ", " + name; // Ghép nội dung cũ với nội dung mới
            // Sao chép văn bản mới vào clipboard
            navigator.clipboard.writeText(newText).then(
              function () {
                alert("Sao chép thành công!");
              },
              function (err) {
                alert("Không thể sao chép!");
              }
            );
          })
          .catch((err) => {
            alert("Không thể lấy dữ liệu từ clipboard: " + err);
          });
      }

      // Hàm để chuyển đổi trạng thái ẩn/hiện của phần nội dung liên hệ
      function toggleContact(contentID) {
        var content = document.getElementById(contentID);

        if (content) {
          // Kiểm tra xem phần tử có tồn tại không
          if (
            content.style.display === "none" ||
            content.style.display === ""
          ) {
            // Ẩn tất cả các phần tử có lớp "contentID" trước khi hiển thị phần tử mới
            var allContents = document.querySelectorAll(contentID);
            allContents.forEach(function (item) {
              item.style.display = "none";
            });

            // Hiển thị phần tử đã chọn
            content.style.display = "block";
          } else {
            // Nếu phần tử đang hiển thị, ẩn nó đi
            content.style.display = "none";
          }
        }
      }
    </script>
  </body>
</html>
