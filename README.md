
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
        margin: 0 1 0 1;
        padding: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-image: url("https://i.pinimg.com/474x/bf/58/e7/bf58e7025454d9e51a005147f3225668.jpg");
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
        transform: scale(1.05);
        transition: transform 0.3s ease;
        box-shadow: 0px 2px 5px #000000;
      }
      .font_container {
        position: fixed;
        width: 100%;
        top: 130px;
        bottom: 90px;
        overflow-y: auto;
        scroll-behavior: smooth;
      }

      /* Phần chứa sản phẩm với cuộn ngang */
      .container {
        display: flex;
        gap: 10px;
        padding: 10px;
        width: 100%;
        overflow-x: auto;
        scroll-behavior: smooth;
      }

      /* Phần hiển thị sản phẩm */
      .product-row {
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(208, 241, 239);
        padding: 5px 5px 5px 5px;
        border-radius: 5px;
        width: 160px;
        text-align: center;
        flex: 0 0 auto; /* Đảm bảo sản phẩm có kích thước cố định để cuộn ngang */
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
        font-size: 0.75em;
      }

      .product-left .price {
        color: #ff0000c4;
        margin: 2px 0;
        font-size: 0.7em;
      }

      /* Nút Đặt và Lưu */
      .product-actions a,
      .product-actions button {
        font-size: 0.6em;
        color: white;
        padding: 5px 5px;
        border-radius: 5px;
        text-decoration: none;
      }

      .link {
        background-color: #f489d7;
      }

      .link:hover {
        background-color: #ff3fc5;
      }
      .order {
        background-color: #28a745;
      }

      .order:hover {
        background-color: #218838;
      }

      .save {
        background-color: #007bff;
      }

      .save:hover {
        background-color: #0056b3;
      }

      /* Phần footer */
      .footer_top,
      .footer_bottom {
        background-color: #ffffff;
        color: rgb(0, 0, 0);
        padding: 0.5px;
        text-align: center;
        width: 100%;
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
        /*z-index: 1000;
        */
        transition: transform 0.5s ease;
        border: 2px solid black;
      }

      .shopping {
        bottom: 20px;
        right: 32%;
      }
      .chatting {
        bottom: 20px;
        right: 10%;
      }
      .ADS {
        bottom: 20px;
        left: 32%;
      }

      .shopping:hover,
      .chatting:hover,
      .ADS:hover,
      .contact-logo:hover {
        transform: scale(1.2);
        box-shadow: 0 2px 2px #000000;
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
        /*z-index: 1000;*/
        justify-content: center;
      }

      /* Kiểu dáng cho hộp thông tin liên hệ, nằm ở lề phải và ẩn ban đầu */
      .contact-content {
        display: none; /* Ẩn hộp liên hệ khi chưa nhấn vào logo */
        position: fixed;
        background-color: #e3e3e3;
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 15px;
        width: Auto;
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

      .contact-content h2 {
        margin-top: 0;
        font-size: 14px;
        color: #333;
        text-align: center;
      }

      .contact-content p {
        margin: 5px 0;
        font-size: 10px;
        color: #000000;
      }
      .contact-content a {
        color: rgb(2, 57, 255);
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

    <!-- Logo để mở/ẩn phần nội dung liên hệ -->
    <div class="contact-logo" onclick="toggleContact()">
      <img
        src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
        alt="contact-log"
      />
    </div>

    <!-- Nội dung liên hệ (ẩn mặc định) -->
    <div class="contact-content" id="contactContent">
      <h2>Liên Hệ</h2>
      <p>Email: <a>contact@example.com</a></p>
      <p>Điện Thoại: <a>+123 456 789</a></p>
      <p>Địa Chỉ: <a>1234 Example Street, City</a></p>
    </div>

    <div class="font_container">
      <!-- Shopee -->
      <div class="container">
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>

        <!-- Thêm các sản phẩm khác tương tự ở đây -->
      </div>
      <div class="container">
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>

        <!-- Thêm các sản phẩm khác tương tự ở đây -->
      </div>
      <div class="container">
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>

        <!-- Thêm các sản phẩm khác tương tự ở đây -->
      </div>

      <!-- OTISShop -->
      <div class="container">
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>
        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>

        <!-- Sản phẩm 1 -->
        <div class="product-row">
          <div class="product-left">
            <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
            <h3>Sản phẩm 1</h3>
            <div class="price">Giá: 100,000 VND</div>
            <div class="product-actions">
              <button class="save" onclick="copyProductInfo('SP1')">
                Lưu mã sản phẩm
              </button>
            </div>
          </div>
        </div>

        <!-- Thêm các sản phẩm khác tương tự ở đây -->
      </div>
    </div>
    <!-- Floating Buttons -->
    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20muốn%20mua%20sản%20phẩm?"
      target="_blank"
      class="shopping"
    >
      <img
        src="https://i.pinimg.com/474x/f7/22/3e/f7223e8daaee44645802955532e1c372.jpg"
        alt="Shopping"
      />
    </a>

    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20có%20một%20vài%20vấn%20đề?"
      target="_blank"
      class="chatting"
    >
      <img
        src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
        alt="Chatting"
      />
    </a>

    <a
      href="https://www.messenger.com/t/460099260527241?message=Tôi%20muốn%20hợp%20tác%20quảng%20cáo?"
      target="_blank"
      class="ADS"
    >
      <img
        src="https://i.pinimg.com/474x/38/ea/d6/38ead648ede5fb91f29b086f22396613.jpg"
        alt="ADS"
      />
    </a>

    <script>
      /*
      let clipboardContent = "";

      function saveToClipboard(name) {
        // Nội dung mới cần thêm vào clipboard
        const newText = name; // Thay đổi nội dung này theo nhu cầu

        // Cộng dồn đoạn văn bản mới vào nội dung cũ
        clipboardContent += newText;

        // Sao chép nội dung đã cập nhật vào clipboard
        navigator.clipboard
          .writeText(clipboardContent)
          .then(() => {
            alert("Đã thêm mã sản phẩm, chọn 'Giỏ hàng' để đặt!");
          })
          .catch((err) => {
            console.error("Không thể thêm mã sản phẩm, vui lòng thử lại!", err);
          });
      } */
      function copyProductInfo(name) {
        // Lấy văn bản hiện tại từ clipboard (nếu có)
        navigator.clipboard
          .readText()
          .then((existingText) => {
            // Cộng dồn nội dung mới vào nội dung cũ
            const newText = existingText + " " + name; // Ghép nội dung cũ với nội dung mới

            // Sao chép văn bản mới vào clipboard
            navigator.clipboard.writeText(newText).then(
              function () {
                alert("Đã lưu mã sản phẩm, vui lòng chọn 'Giỏ hàng'!");
              },
              function (err) {
                alert("Có lỗi xảy ra, không thể lưu mã sản phẩm!");
              }
            );
          })
          .catch((err) => {
            alert("Không thể lấy dữ liệu từ clipboard: " + err);
          });
      }

      // Hàm để chuyển đổi trạng thái ẩn/hiện của phần nội dung liên hệ
      function toggleContact() {
        var content = document.getElementById("contactContent");
        if (content.style.display === "none" || content.style.display === "") {
          content.style.display = "block"; // Hiển thị nội dung
        } else {
          content.style.display = "none"; // Ẩn nội dung
        }
      }
    </script>
  </body>
</html>
