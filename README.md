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
        /* Thiết lập phông chữ mặc định cho toàn bộ trang */
        font-family: Arial, sans-serif;

        /* Dùng flexbox để căn chỉnh các phần tử trong body */
        display: flex;
        flex-direction: column; /* Căn các phần tử theo chiều dọc */
        align-items: center; /* Căn giữa theo trục ngang */
        justify-content: center; /* Căn giữa theo trục dọc */

        /* Thiết lập nền bằng hình ảnh */
        background-image: url("https://i.pinimg.com/474x/bf/58/e7/bf58e7025454d9e51a005147f3225668.jpg");
        background-repeat: repeat; /* Lặp hình nền theo cả chiều ngang và dọc */
        background-size: auto; /* Giữ nguyên kích thước gốc của hình ảnh */

        /* Màu nền thay thế (hiển thị khi hình ảnh không tải được) */
        background-color: #f0f0f0;

        /* Màu văn bản mặc định cho body */
        color: #000000;

        /* Giới hạn chiều rộng của body */
        max-width: 100%;
        width: 380px; /* Cố định chiều rộng */

        /* Loại bỏ khoảng cách mặc định của body */
        margin: 0 auto; /* Căn giữa body theo chiều ngang trong viewport */
      }
      /* Phần chứa logo */
      .header {
        text-align: center;
        width: 100%;
        margin: 70px 0 0 0;
        font-size: 32px;
      }
      /* Ảnh logo */
      .header img {
        width: 225px;
        height: auto;
        border-radius: 50%;
        object-fit: cover;
      }
      /* hiệu ứng Logo */
      .header img:hover {
        transform: scale(1.1);
        transition: transform 0.5s ease;
        box-shadow: 0px 8px 12px #000000;
      }
      /* Phần chứa sản phẩm */
      .container {
        display: flex;
        width: 330px;
        flex-direction: column; /* Sắp xếp các phần tử con theo chiều dọc */
        gap: 10px; /* Khoảng cách giữa các phần tử */
        padding: 10px; /* Khoảng cách bên trong container */
        align-items: center; /* Căn giữa các phần tử con theo chiều ngang */
        justify-content: center; /* Căn các phần tử con theo chiều dọc (mặc định là từ trên xuống) */
      }
      /* Phần hiển thị sản phẩm */
      .product-row {
        width: 90%;
        max-width: 330px; /* Chiều rộng tối đa */
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: rgb(211, 240, 255);
        padding: 5px;
        border-radius: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
        border: 2.5px solid black;
      }
      /* Ảnh sản phẩm */
      .product-left img {
        width: 290px;
        height: auto;
        object-fit: cover;
        border-radius: 10px;
      }
      /* Tên sản phẩm */
      .product-left h3 {
        margin: 0;
        font-size: 1em;
      }
      /* Giá */
      .product-left .price {
        color: #d30808;
        margin: 5px 0;
        font-size: 0.9em;
        font-weight: 520;
      }
      /* Nút điều hướng */
      .product-actions {
        display: flex; /* Thiết lập container làm flexbox */
        justify-content: center; /* Căn giữa các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều dọc (nếu cần) */
      }
      .product-actions img {
        width: 30px;
        height: 30px;
        border: 2px solid #000000;
        border-radius: 50%;
        margin: 0 10px 0 10px;
      }
      .OUT,
      .oder,
      .save,
      .link {
        margin: 0px 5px 0px 5px;
        height: 35px;
        width: auto;
        border-radius: 6px;
      }
      .OUT {
        background-color: #f63d3d;
      }
      .OUT:hover {
        background-color: #d30808;
      }
      .oder {
        background-color: #58e139;
      }
      .oder:hover {
        background-color: #04a504;
      }
      .save {
        background-color: #4989ff;
      }
      .save:hover {
        background-color: #1653cdc4;
      }
      .link {
        background-color: #e75ef6;
      }
      .link:hover {
        background-color: #c40ec4;
      }
      .OUT a,
      .oder a,
      .save a,
      .link a {
        font-size: 18px;
        font-weight: 540;
      }
      /* Phần floating icons */
      .shopping,
      .chatting,
      .voucher,
      .content {
        position: fixed;
        right: 10px;
        width: 50px;
        height: auto;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: transform 0.5s ease;
        border: 2px solid black;
      }
      .shopping {
        bottom: 190px;
      }
      .voucher {
        bottom: 130px;
      }
      .chatting {
        bottom: 70px;
      }
      .content {
        bottom: 10px;
      }
      .shopping:hover,
      .chatting:hover,
      .voucher:hover,
      .content:hover {
        transform: scale(1.1);
        box-shadow: 0 5px 10px #000000;
      }
      .shopping img,
      .chatting img,
      .voucher img,
      .content img {
        width: 50px;
        height: auto;
        object-fit: cover;
        border-radius: 50%;
      }
      /* Hộp thông tin */
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting,
      .contact-VD {
        position: fixed;
        background-color: #ffffff;
        border: 6px solid #000000;
        border-radius: 24px;
        padding: 15px;
        width: 90%;
        max-width: 360px;
        top: 50%;
        left: 50%;
        transform: translate(
          -50%,
          -50%
        ); /* Dịch chuyển để căn giữa chính xác */
        box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1);
        transition: transform 2s ease;
        border: 2px solid black;
        z-index: 999;
      }
      /* Ẩn ban đầu */
      .contact-Content,
      .contact-Voucher,
      .contact-Shopping,
      .contact-Chatting {
        display: none;
      }
      /* Hiện ban đầu */
      .contact-VD {
        display: block;
      }
      .contact-Content h3,
      .contact-Voucher h3,
      .contact-Shopping h3,
      .contact-Chatting h3,
      .contact-VD h3 {
        margin: 8px 0;
        font-size: 24px;
        color: #000000;
        text-align: left;
        font-weight: 750;
      }
      .contact-Content p,
      .contact-Voucher p,
      .contact-Shopping p,
      .contact-Chatting p,
      .contact-VD p {
        margin: 4px 0;
        font-size: 14px;
        color: #000000;
        text-align: left;
        font-weight: 450;
      }
      .contact-Content li,
      .contact-Voucher li,
      .contact-Shopping li,
      .contact-Chatting li,
      .contact-VD li {
        margin: 4px 0;
        font-size: 14px;
        color: #000000;
        text-align: left;
        font-weight: 450;
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
    <hr />

    <!-- Sản phẩm Liên Kết Shopee -->
    <div class="container">
      <!-- Sản phẩm 1 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/bc/ec/25/bcec2542f761d93fd3191855e5bec86a.jpg"
            alt="Sản phẩm 1"
          />
          <h3>Nước Hoa - BODYMISS</h3>
          <div class="price">Giá: 136.800 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1101')">
              <a>SP1101</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/8pUdQpfLsu', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 2 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/00/4a/9a/004a9aaeb3d695e0593b62f7b5570144.jpg"
            alt="Sản phẩm 2"
          />
          <h3>Sữa tắm gội 3 in 1</h3>
          <div class="price">Giá: 159.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP0102')">
              <a>SP1102</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/8AEwdf7DK3', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 3 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/b2/75/36/b27536f6ad8530a39272e0e33960a9cc.jpg"
            alt="Sản phẩm 3"
          />
          <h3>Quạt mini có LED</h3>
          <div class="price">Giá: 329.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP0103')">
              <a>SP1103</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/5VEBSmY4yy', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 4 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/65/49/e1/6549e19bb9a99b8df321000b55bc740a.jpg"
            alt="Sản phẩm 4"
          />
          <h3>Đồng Hồ Thông Minh</h3>
          <div class="price">Giá: 56.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP0104')">
              <a>SP1104</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/1LOcV91DZv', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 5 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/90/06/ce/9006ceb11e216f95fd258fd833f36276.jpg"
            alt="Sản phẩm 5"
          />
          <h3>Sạc dự phòng 20W</h3>
          <div class="price">Giá: 339.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP0105')">
              <a>SP1105</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/5AbL4DGshp', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 6 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/e5/8d/c2/e58dc2624756e5e8eb9caf9a4e008650.jpg"
            alt="Sản phẩm 6"
          />
          <h3>Điện Thoại Vivo V23 5G</h3>
          <div class="price">Giá: 1.988.950 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1106')">
              <a>SP1106</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/9zgap9wWPX', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 7 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/a4/f5/6c/a4f56c639e16d6cb014b28704f2e26cd.jpg"
            alt="Sản phẩm 7"
          />
          <h3>Áo Len Nam Nữ</h3>
          <div class="price">Giá: 99.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1107')">
              <a>SP1107</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/3AqGgcvk3y', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 8 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/d8/1e/c2/d81ec2de154704240bac0dec046bf1e4.jpg"
            alt="Sản phẩm 8"
          />
          <h3>Quần jean nam</h3>
          <div class="price">Giá: 139.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1108')">
              <a>SP1108</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/30WqUJwNOx', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 9 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/90/cd/7c/90cd7cc76708ab6e8f9d253750b8fdb3.jpg"
            alt="Sản phẩm 9"
          />
          <h3>Áo sơ mi trắng nam</h3>
          <div class="price">Giá: 165.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1109')">
              <a>SP1109</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/4pyUfgpOgK ', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 10 -->
      <div class="product-row">
        <div class="product-left">
          <img
            src="https://i.pinimg.com/474x/34/28/ab/3428abd5ea2217f803f54b920937eb80.jpg"
            alt="Sản phẩm 10"
          />
          <h3>Quần Jean BIGSIZE</h3>
          <div class="price">Giá: 150.000 VNĐ</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('SP1110')">
              <a>SP1110</a></button
            ><img
              src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg"
              alt="Shopee"
            />
            <button
              class="link"
              onclick="window.open('https://s.shopee.vn/4ff4TNq21J', '_blank')"
            >
              <a>Link</a>
            </button>
          </div>
        </div>
      </div>

      <!-- Thêm các sản phẩm khác tương tự ở đây -->
    </div>
    <hr />
    <!--
    <hr />
    <-- Sản phẩm OTISShop --
    <div class="container">
      <-- Sản phẩm 1 --
      <div class="product-row">
        <div class="product-left">
          <img src="https://via.placeholder.com/150x120" alt="Sản phẩm 1" />
          <h3>Sản phẩm 1</h3>
          <div class="price">Giá: 100,000 VND</div>
          <div class="product-actions">
            <button class="save" onclick="copyProductInfo('OS0101')">
              <a>OS1101</a></button
            ><img
              src="https://i.pinimg.com/474x/df/2f/de/df2fdeef83868e15085ae4c7e4b9d396.jpg"
              alt="Shopee"
            />
            <button
              class="oder"
              onclick="window.open('https://www.messenger.com/t/460099260527241?', '_blank')"
            >
              <a>Đặt</a>
            </button>
          </div>
        </div>
      </div>

      <-- Thêm các sản phẩm khác tương tự ở đây --
    </div>-->
    <br />

    <!-- Nội dung Ghi Chú -->
    <div class="contact-VD" id="contactVD">
      <h3 style="text-align: center">
        Hướng dẫn!
        <button class="OUT" onclick="toggleContact('contactVD')">
          <a>X</a>
        </button>
      </h3>
      <p>
        <li>
          - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
        </li>
        <li>
          - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
        </li>
        <li>
          - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
        </li>
        <li>
          - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
        </li>
        <li>
          - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
        </li>
      </p>
    </div>
    <!-- Logo để mở/ẩn phần Thông Tin -->
    <div class="content" onclick="toggleContact('contactContent')">
      <img
        src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
        alt="content"
      />
    </div>
    <!-- Nội dung Thông Tin -->
    <div class="contact-Content" id="contactContent">
      <h3 style="text-align: center">
        Chi tiết!
        <button class="OUT" onclick="toggleContact('contactContent')">
          <a>X</a>
        </button>
      </h3>
      <p>
        <li>Hotline: <a href="tel:0329022431">0329022431</a></li>

        <li>
          Email:
          <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>
        </li>
        <li>
          Fanpage:
          <a href="https://www.messenger.com/t/460099260527241?" target="_blank"
            >https://.../OtisSeller</a
          >.
        </li>
        <li>
          Địa Chỉ:
          <a href="https://maps.app.goo.gl/pyLNvcmZvLtHrBtT7"
            >2252/22/12.Tổ 2, Kp1, Tân Chánh Hiệp, Q.12, TP.HCM, Việt Nam</a
          >.
        </li>
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
      <h3 style="text-align: center">
        Giỏ hàng!
        <button class="OUT" onclick="toggleContact('contactShopping')">
          <a>X</a>
        </button>
        <button
          class="oder"
          onclick="window.open('https://www.messenger.com/t/460099260527241?', '_blank')"
        >
          <a>Đơn</a>
        </button>
      </h3>
      <li>Lưu mã sản phẩm vào 'Clipboard' trước khi bấm 'Đơn'!</li>
      <li>
        Bấm 'Đơn' và gửi mã sản phẩm + thông tin cho chúng tôi thông qua Fanpage
        của OTISShop!
      </li>
      <li>Chỉ hổ trợ tư vấn - không bán sản phẩm liên kết Shopee!</li>

      <p style="text-align: center">- - -Chân Thành Cảm Ơn Quý Khách!- - -</p>
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
      <h3 style="text-align: center">
        Hổ trợ!
        <button class="OUT" onclick="toggleContact('contactChatting')">
          <a>X</a>
        </button>
      </h3>
      <p>
        <li>Hổ trợ tư vấn sản phẩm.</li>
        <li>Liên kết bán hàng - Tư vấn sản phẩm.</li>
        <li>Hổ trợ quảng cáo - Tiếp thị sản phẩm.</li>
        <li>
          Hotline: <a href="tel:0329022431" target="_blank">0329022431</a>.
        </li>
        <li>
          Fanpage:
          <a href="https://www.messenger.com/t/460099260527241?" target="_blank"
            >https://.../OtisSeller</a
          >.
        </li>
        <li>
          Email:
          <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a>.
        </li>
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
      <h3 style="text-align: center">
        Voucher!
        <button class="OUT" onclick="toggleContact('contactVoucher')">
          <a>X</a>
        </button>
      </h3>
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

      // Dọn sạch dữ liệu khi tải trang (sau khi trang được load hoàn toàn)
      window.onload = function () {
        // Reset mảng mã sản phẩm đã chọn
        selectedProductCodes = [];
        console.log("Vui lòng lưu mã sản phẩm vào Clipboard!");
      };

      function toggleContact(contentID) {
        var content = document.getElementById(contentID);
        var content1 = document.getElementById("contactContent");
        var content2 = document.getElementById("contactChatting");
        var content3 = document.getElementById("contactVoucher");
        var content4 = document.getElementById("contactShopping");
        var content5 = document.getElementById("contactVD");

        // Ẩn tất cả các phần tử khác trước khi hiển thị phần tử mới
        if (contentID === "contactContent") {
          content2.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
        }
        if (contentID === "contactChatting") {
          content1.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
        }
        if (contentID === "contactVoucher") {
          content1.style.display = "none";
          content2.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
        }
        if (contentID === "contactShopping") {
          content1.style.display = "none";
          content2.style.display = "none";
          content3.style.display = "none";
          content5.style.display = "none";
        }
        if (contentID === "contactVD") {
          content1.style.display = "none";
          content2.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
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
