<html lang="vi">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Chất Lượng, Uy Tín, Tin Cậy." />
    <meta name="author" content="OTISShop" />
    <meta
      name="image"
      content="https://i.pinimg.com/474x/ea/24/e1/ea24e1a0ed40857020ab39336b9fc78c.jpg"
    />
    <title>OTISShop</title>
    <link
      rel="icon"
      type="image/jpeg"
      href="https://i.pinimg.com/474x/6d/ed/ac/6dedac7e01c34c37f226b05591ccde2e.jpg"
    />
    <!-- Google tag (gtag.js) -->
    <script
      async
      src="https://www.googletagmanager.com/gtag/js?id=G-RTE1XGS0BK"
    ></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag() {
        dataLayer.push(arguments);
      }
      gtag("js", new Date());

      gtag("config", "G-RTE1XGS0BK");
    </script>
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
        background-repeat: repeat-y; /* Lặp hình nền theo cả chiều dọc */
        background-size: 100% auto; /* Giữ nguyên chiều cao hình ảnh */

        /* Màu nền thay thế (hiển thị khi hình ảnh không tải được) */
        background-color: #f0f0f0;

        /* Màu văn bản mặc định cho body */
        color: #000000;
        user-select: none;
        width: 100%;

        /* Loại bỏ khoảng cách mặc định của body */
        margin: 17.5px auto 22.5px auto; /* Căn giữa body theo chiều ngang trong viewport */
      }

      /* Phần chứa logo */
      .header {
        background-image: url("https://i.pinimg.com/736x/30/b1/9b/30b19b5deca9683e67a3960d44a6df83.jpg");
        background-repeat: repeat-x;
        background-size: auto 100%;
        position: fixed;
        top: 0;
        left: -50%;
        right: -50%; /* Đặt các icon từ dưới lên */
        display: flex;
        flex-direction: row; /* Xếp các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều ngang */
        justify-content: center;
        padding: 10px;
        border: 2px solid black;
        gap: 10px; /* Phân bố đều khoảng cách giữa các phần tử */
        height: auto; /* Chiều cao của container */
      }

      /* Ảnh logo */
      .header img {
        width: 75px;
        height: auto;
        border-radius: 50%;
        object-fit: cover;
      }
      /* hiệu ứng Logo */
      .header img:hover {
        transform: scale(1.05);
        transition: transform 0.5s ease;
        box-shadow: 0px 0px 12px #000000;
      }
      .filter-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: #63e2ffb1;
        border-radius: 7px;
        gap: 2px;
        padding: 2px;
        width: auto;
        height: auto;
      }
      /* Phần hiển thị sản phẩm dọc */
      .SHOPEE,
      .TIKTOK,
      .OTISShop {
        display: flex;
        width: 320px;
        flex-direction: column; /* Sắp xếp các phần tử con theo chiều dọc */
        align-items: center; /* Căn giữa các phần tử con theo chiều ngang */
        justify-content: center; /* Căn các phần tử con theo chiều dọc (mặc định là từ trên xuống) */
      }
      .product-row {
        width: 100%; /* Chiều rộng tối đa */
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: auto;
        gap: 4px;
        padding: 2px 0;
        border-radius: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }
      .product-row2 {
        width: auto;
        display: flex;
        flex-direction: row;
        align-items: center;

        border-radius: 2px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }
      .product-column {
        width: auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-image: url("https://i.pinimg.com/736x/3a/cb/1b/3acb1b0bf256c9cb84cd785018970842.jpg");
        background-repeat: repeat-y; /* Không lặp hình nền */
        background-size: 100% auto; /* Giữ nguyên chiều cao hình ảnh */
        border-radius: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }
      /* Phần sản phẩm */
      .product-column2 {
        width: 210px;
        height: 110px;
        display: flex;
        background-color: #f5f5f5a5;
        flex-direction: column;
        align-items: auto;
        border-radius: 0 5px 5px 0;
        justify-content: center; /* Căn giữa các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều dọc (nếu cần) */
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }
      /* Ảnh sản phẩm */
      .product-row2 img {
        width: 110px;
        height: 110px;
        object-fit: cover;
        border-radius: 5px 0 0 5px;
      }
      .product-description {
        top: calc(50%);
        left: 50%;
        transform: translate(
          -50%,
          -50%
        ); /* Dịch chuyển để căn giữa chính xác */
        position: fixed;
        display: none;
        width: 100%;
        height: 100%;
        color: #000;
        background-color: #616161cd;
        flex-direction: column;
        justify-items: center;
        align-items: center;
        z-index: 999;
      }
      .description-img {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 17%;
        gap: 5px;
      }
      .description-text {
        position: fixed;
        display: flex;
        flex-direction: column;
        text-align: left;
        width: 100%;
        height: 83%;
        background-color: #ffffffe3;
      }

      .description-text p {
        margin: 1.5% 0.5% 1% 2%;
        width: 97.5%;
        font-size: 12px;
        font-weight: 600;
      }
      .description-text a {
        margin: 0.2% 0.5% 0.2% 4.5%;
        width: 95%;
        display: flex;
        flex-wrap: wrap;
        font-size: 11px;
        font-weight: 400;
      }
      .description-text i {
        width: 100%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
      }
      .product-column .name {
        color: #000000;
        margin: 2.5px;
        font-size: 13px;
        font-weight: 600;
      }
      /* Giá */
      .product-column .price {
        color: #d81414;
        margin: 2px;
        font-size: 12px;
        font-weight: 600;
      }
      /* Nút điều hướng */
      .product-actions {
        width: auto;
        height: auto;
        display: flex; /* Thiết lập container làm flexbox */
        justify-content: center; /* Căn giữa các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều dọc (nếu cần) */
      }
      .product-actions img {
        width: 26px;
        height: 26px;
        border-radius: 50%;
        margin: 2px 4px;
      }
      .oder,
      .save,
      .link {
        margin: 2px;
        width: auto;
        min-width: 60px;
        height: 24px;
        font-size: 11px; /* Kích thước chữ */
        font-weight: 550; /* Độ đậm của chữ */
        text-align: center; /* Căn giữa chữ theo chiều ngang */
        justify-content: center; /* Căn giữa ngang */
        align-items: center; /* Căn giữa dọc */
        color: rgb(0, 0, 0); /* Màu chữ */
        border-radius: 5px;
      }
      .div-style {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        margin-top: 5px;
        gap: 50px;
      }
      .div-style2 {
        width: 70px;
        height: 26px;
        border-radius: 3px;
        font-weight: 550;
      }
      .styler {
        width: 100%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        font-size: 11px;
        margin-top: 3px;
        height: 15px;
        color: white;
        background-color: #8787878f;
      }
      .oder {
        background-color: #58e139;
      }
      .oder:hover {
        background-color: #04a504;
      }
      .save {
        background-color: #589eff;
      }
      .save:hover {
        background-color: #2c6bff;
      }
      .link {
        background-color: #e772f4;
      }
      .link:hover {
        background-color: #d62cd6;
      }
      /* Phần floating icons */
      .icon-container {
        position: fixed;
        bottom: 0;
        left: -50%;
        right: -50%; /* Đặt các icon từ dưới lên */
        display: flex;
        background-color: white;
        flex-direction: row; /* Xếp các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều ngang */
        justify-content: center;
        box-shadow: 0 0 5px black;
        padding: 10px;
        gap: 60px; /* Phân bố đều khoảng cách giữa các phần tử */
        height: auto; /* Chiều cao của container (thay đổi tuỳ theo số lượng và kích thước các phần tử) */
      }
      /* Các phần tử icon */
      .icon {
        border-radius: 50%;
        display: flex;
        width: 40px;
        height: 40px;
        align-items: center;
        justify-content: center;
        transition: transform 0.5s ease, box-shadow 0.5s ease;
        box-shadow: 0 0 8px #000000;
      }
      .icon:active {
        transform: scale(1.2); /* Phóng to */
        border-radius: 50%;
      }
      .icon img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        border-radius: 50%;
      }
      /* Hộp thông tin */
      .contact-Content,
      .contact-Chatting {
        position: fixed;
        background-color: #ffffff;
        border-radius: 10px;
        padding: 10px;
        width: 95%;
        max-width: 400px;
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
      .contact-Home {
        position: fixed;
        background-color: #ffffff;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
        padding: 10px;
        width: 95%;
        max-width: 400px;
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
      .contact-Style {
        position: fixed;
        background-color: #ffffff;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
        padding-bottom: 10px;
        gap: 10px;
        width: 95%;
        max-width: 380px;
        top: 50%;
        left: 50%;
        transform: translate(
          -50%,
          -50%
        ); /* Dịch chuyển để căn giữa chính xác */
        border: 0.5px solid black;
        z-index: 999;
      }

      /* Ẩn ban đầu */
      .contact-Chatting,
      .contact-Home,
      .contact-Style {
        display: none;
      }
      /* Hiện ban đầu */
      .contact-Content {
        display: block;
      }
      .contact-Content h3,
      .contact-Chatting h3,
      .contact-Home h3 {
        margin: 0;
        font-size: 16px;
        color: #000000;
        display: flex;
        justify-content: center;
        align-items: center;
        font-weight: 600;
      }
      .contact-Content p,
      .contact-Home p,
      .contact-Chatting p {
        margin: 2.5px 0;
        font-size: 13px;
        color: #000000;
        text-align: left;
      }
      .contact-Content li,
      .contact-Chatting li,
      .contact-Home li {
        margin: 2.5px 0;
        font-size: 13px;
        color: #000000;
        text-align: left;
      }
      .contact-Style h3 {
        font-size: 14px;
        color: #000000;
        text-align: center;
      }
      .header2 {
        width: 100%;
        max-width: 390px;
        padding: 5px;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        height: auto;
        gap: 15px;
        background-color: rgb(255, 255, 255);
      }
      /* HÀM TẠO 4 MÙA */
      #effect-container {
        position: fixed;
        top: 0;
        left: 0;
        z-index: 1001;
        width: 100%;
        height: 100%;
        pointer-events: none;
      }

      .effect {
        position: absolute;
        top: -50px;
        background-size: contain;
        background-repeat: no-repeat;
        opacity: 1;
        pointer-events: none;
        animation: fall linear infinite;
      }

      @keyframes fall {
        0% {
          transform: translateY(-10px) rotate(0deg);
          opacity: 1;
        }
        100% {
          transform: translateY(105vh) rotate(360deg);
          opacity: 0;
        }
      }
    </style>
  </head>

  <body>
    <div id="effect-container"></div>
    <script src="script.js"></script>
    <!-- Phần logo -->
    <div class="header">
      <img
        src="https://i.pinimg.com/474x/ea/24/e1/ea24e1a0ed40857020ab39336b9fc78c.jpg"
        alt="Logo"
      />
      <!-- Thanh điều kiện (Filter) -->
      <div
        style="
          width: auto;
          height: auto;
          padding: 3px;
          background-color: #ffffffa6;
          align-items: center;
          justify-items: center;
          border-radius: 10px;
        "
      >
        <div class="filter-container">
          <div
            style="
              height: auto;
              display: flex;
              flex-direction: row;
              justify-content: center;
              align-items: center;
              gap: 5px;
              margin: 1px;
            "
          >
            <div>
              <label for="shop-select" style="font-size: 14px; width: 45px"
                ><b>Shop: </b></label
              >
              <select
                id="shop-select"
                style="
                  font-size: 13px;
                  border-radius: 3px;
                  width: 100px;
                  border: 1px solid black;
                "
              >
                <option value="all" selected>Tất cả</option>
                <option value="SHOPEE">Shopee</option>
                <option value="TIKTOK">TikTok</option>
                <option value="OTISShop">OTISShop</option>
              </select>
            </div>

            <div
              style="
                font-size: 14px;
                display: flex;
                align-items: center;
                justify-content: center;
                margin: 3px;
              "
            >
              <b style="width: 33px">Còn:</b>

              <div
                id="product-count"
                style="
                  font-size: 13px;
                  display: flex;
                  align-items: center;
                  justify-content: center;
                  background-color: #f0f0f0;
                  border: 1px solid black;
                  border-radius: 3px;
                  width: 35px;
                  height: 16px;
                "
              >
                0
              </div>
            </div>
          </div>

          <div
            style="
              height: auto;
              display: flex;
              align-items: flex-start;
              margin: 2px 0;
            "
          >
            <label for="category-select" style="font-size: 14px; width: 40px"
              ><b>Loại: </b></label
            >
            <select
              id="category-select"
              style="
                font-size: 13px;
                border-radius: 3px;
                width: 176px;
                border: 1px solid black;
              "
            >
              <option value="all" selected>Tất cả</option>
              <option value="A">Thời Trang</option>
              <option value="B">Sức Khỏe & Làm Đẹp</option>
              <option value="C">Thiết Bị Điện Tử</option>
              <option value="D">Nhà Cửa & Đời Sống</option>
              <option value="E">Mẹ & Bé</option>
              <option value="F">Thể Thao & Du Lịch</option>
              <option value="G">Tiêu Dùng & Thực Phẩm</option>
              <option value="H">Văn Phòng & Đồ Chơi</option>
              <option value="I">Xe & Phụ Kiện</option>
              <option value="J">Linh Kiện & Mạch Điện</option>
              <option value="K">Khác</option>
            </select>
          </div>
          <div
            style="
              display: flex;
              flex-direction: row;
              align-items: center;
              margin-bottom: 3px;
            "
          >
            <b style="font-size: 13px">Ngày cập nhật: </b>
            <button
              style="
                display: flex;
                width: 125px;
                margin-left: 3px;
                height: 19px;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                background-color: #ffffff;
                border: 1px solid black;
                border-radius: 3px;
              "
            >
              <a style="font-size: 13px"> 00:00 - 07.01.2025</a>
            </button>
          </div>
        </div>
      </div>
    </div>

    <!-- Sản phẩm SHOPEE -->
    <div class="SHOPEE">
      <div class="product-row"></div>
    </div>
    <!-- Sản phẩm TIKTOK -->
    <div class="TIKTOK">
      <div class="product-row"></div>
    </div>
    <!-- Sản phẩm OTISShop -->
    <div class="OTISShop">
      <div class="product-row"></div>
    </div>

    <!-- List Sản phẩm -->
    <script>
      const products = {
        SHOPEE: [
          /* Quần Jean BIGSIZE*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2m8kpfbnrie79@resize_w450_nl.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lwcl0ymunrvd34.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m23qhtd0yl7i37.webp",
            name: "Quần Jean BIGSIZE",
            price: "150.000",
            code: "SPA01",
            category: "A",
            link: "https://s.shopee.vn/4ff4TNq21J",
            description:
              "<p>THÔNG TIN SẢN PHẨM:</p><a>👖 Quần Jean Nam Wash RETRO</a><a>Chất liệu : Jean co dãn</a><a>Kiểu dáng: Quần suông form rộng</a><a>Màu sắc: Xanh - Đen</a><p>THÔNG SỐ SẢN PHẨM:</p><a>🔥 Size 26 (Từ 38 - 44kg Cao Dưới 1m71)</a><a>🔥 Size 27 (Từ 44 - 49kg Cao Dưới 1m71)</a><a>🔥 Size 28 (Từ 50 - 54kg Cao Dưới 1m75)</a><a>🔥 Size 29 (Từ 55 - 58kg Cao Dưới 1m80)</a><a>🔥 Size 30 (Từ 59 - 62kg Cao Dưới 1m80)</a><a>🔥 Size 31 (Từ 63 - 65kg Cao Dưới 1m80)</a><a>🔥 Size 32 (Từ 66 - 69kg Cao Dưới 1m80)</a><a>🔥 Size 33 (Từ 70 - 73kg Cao Dưới 1m80)</a><a>🔥 Size 34 (Từ 74 - 77kg Cao Dưới 1m80)</a><a>🔥 Size 35 (Từ 78 - 81kg Cao Dưới 1m80)</a><a>🔥 Size 36 (Từ 81 - 87kg Cao Dưới 1m80)</a><p>HƯỚNG DẪN BẢO QUẢN VÀ SỬ DỤNG SẢN PHẨM:</p><a>🌀 Lộn trái quần khi giặt để giữ màu lâu phai.</a><a>💧 Sử dụng nước giặt dịu nhẹ để làm sạch nhanh chóng và hiệu quả.</a><a>☀️ Phơi trong bóng râm thoáng mát, tránh ánh nắng trực tiếp.</a><a>🚫 Không dùng hóa chất mạnh hoặc thuốc tẩy trực tiếp.</a><a>🕒 Không ngâm quá lâu trong dung dịch giặt.</a><a>🔥 Là ủi: Dưới 110°C để tránh làm hư hại chất liệu.</a>",
          },
          /* Quần Jean Nam HELLOYOU*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/22b1b72be28b9cd9d34a5c8b873b7c3c.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/c04a8e724124d7289b09f5c30196feed.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lpw5ytqzgvyqfb.webp",
            name: "Quần Jean Nam HELLOYOU",
            price: "139.000",
            code: "SPA02",
            category: "A",
            link: "https://s.shopee.vn/30WqUJwNOx",
            description:
              "<p>CHẤT LƯỢNG VƯỢT TRỘI:</p><a>📌 Vải jean chính phẩm với 95% cotton (thấm hút tốt, vải mềm) và 5% spandex (độ co giãn tốt).</a><a>📌 Giặt không phai màu, bề mặt vải mịn bền.</a><p>GIÁ CẢ HỢP LÝ:</p><a>Sản xuất trực tiếp số lượng lớn, đảm bảo giá thành rẻ và chất lượng cao.</a><p>SIZE CHART (THAM KHẢO):</p><a>👖 Size 26: 38 - 44kg, Cao dưới 1m71</a><a>👖 Size 27: 44 - 49kg, Cao dưới 1m71</a><a>👖 Size 28: 50 - 54kg, Cao dưới 1m75</a><a>👖 Size 29: 55 - 58kg, Cao dưới 1m80</a><a>👖 Size 30: 59 - 62kg, Cao dưới 1m80</a><a>👖 Size 31: 63 - 65kg, Cao dưới 1m80</a><a>👖 Size 32: 66 - 69kg, Cao dưới 1m80</a><a>👖 Size 33: 70 - 73kg, Cao dưới 1m80</a><a>👖 Size 34: 74 - 77kg, Cao dưới 1m80</a><a>👖 Size 35: 78 - 81kg, Cao dưới 1m80</a><a>👖 Size 36: 81 - 87kg, Cao dưới 1m80</a><a>👖 Size 37: 88 - 95kg, Cao dưới 1m80</a><p>THÔNG TIN SẢN PHẨM:</p><a>📐 Kiểu dáng: Quần bò nam jean baggy, phù hợp cả nam và nữ.</a><a>🎨 Màu sắc: Xanh Sky, Đen Full, Xanh nhạt.</a><a>💎 Chất liệu: Jean cao cấp, không phai màu.</a><a>📦 Số lượng: Đầy đủ size, hàng xuất khẩu.</a><p>QUẦN JEAN BAGGY HELLOYOU – Dễ phối đồ: Phù hợp với áo thun, hoodie, áo khoác và các loại sneakers, boots.</p>",
          },
          /* Áo Sơ Mi Nam AKUBA*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-ltm7exxdmnm527.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lu7l06ichn3380.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lvzeqai4gmhn09.webp",
            name: "Áo Sơ Mi Nam AKUBA",
            price: "171.840",
            code: "SPA03",
            category: "A",
            link: "https://s.shopee.vn/4pyUfgpOgK",
            description:
              "<p>THÔNG TIN CHI TIẾT</p><a>💎 Chất vải:</a><a>- Cotton lụa cao cấp (80% cotton + 20% polys).</a><a>- Đặc điểm: Không nhăn, mềm mại, thấm hút mồ hôi tốt, mang lại cảm giác dễ chịu cả ngày dài.</a><a>📐 Form dáng:</a><a>- Slimfit: Vừa vặn, ôm nhẹ nhưng không bó sát.</a><a>- Gợi ý: Nếu bạn thích mặc thoải mái hơn, hãy tăng lên 1 size.</a><a>🎨 Màu sắc:</a><a>Đa dạng màu sắc, dễ phối đồ và phù hợp nhiều phong cách.</a><a>🏷 Thiết kế: Sản phẩm được thiết kế và bảo hành bởi CÔNG TY TNHH SẢN XUẤT THƯƠNG MẠI AKUBA.</a><a>📏 Size: Từ M đến 6XL, phù hợp với nhiều dáng người.</a>",
          },
          /* Áo dài long vũ*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m28etdhpfws248@resize_w450_nl.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m28etdh5gq0kea.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m28etdgvh4mq1e.webp",
            name: "Áo dài long vũ",
            price: "177.000",
            code: "SPA04",
            category: "A",
            link: "https://s.shopee.vn/7pdObWU6GU",
            description:
              "<p>❗️✨ GỒM CẢ ÁO + QUẦN ✨❗️</p><p>🌸 𝐒𝐀̉𝐍 𝐏𝐇𝐀̂̉𝐌 𝐃𝐎 𝐌𝐘 𝐓𝐑𝐀̀ 𝐓𝐔̛̣ 𝐌𝐀𝐘 𝟏𝟎𝟎% 🌸</p><a>🪶 Chất liệu: Áo Lông Vũ 🦢 + Quần Satin Lụa 💎 </a><a>📏 Thông số: Freesize dưới 58kg trở lại </a><a> - Áo dài: 110cm (Đo từ cổ xuống) </a><a> - Eo thun: 64-80cm </a><a> - Quần dài: 100cm</a><a>💖 Mềm mại, sang trọng, và đẳng cấp! ✨</a>",
          },
          /* Thời Trang*/
          /* Sữa Tắm 3 In 1 RHYS MAN*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3hc347ukn1kae.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m37bxpi3m5nle4.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m37bxpi3kr3550.webp",
            name: "Sữa Tắm 3 In 1 RHYS MAN",
            price: "165.000",
            code: "SPB01",
            category: "B",
            link: "https://s.shopee.vn/8AEwdf7DK3",
            description:
              "<p>THÔNG TIN THƯƠNG HIỆU:</p><a>🏷️ RHYS MAN là thương hiệu chăm sóc cá nhân dành cho nam giới đã được đăng ký với Bộ Công Thương, tuân thủ đầy đủ các tiêu chuẩn an toàn và mọi thông tin về sản phẩm đều rõ ràng, minh bạch. Với danh mục sản phẩm đa dạng, phù hợp với mọi nhu cầu chăm sóc cá nhân khác nhau của phái mạnh, Rhys Man hướng tới sự toàn diện, hiện đại, trẻ trung, giúp phái mạnh tự tin suốt cả ngày dài.</a><p>THÀNH PHẦN:</p><a>🌿 Decyl Glucoside: Chiết xuất từ thiên nhiên, khả năng tạo bọt tuyệt vời, dịu nhẹ giúp loại bỏ bụi bẩn và dầu hiệu quả trong khi vẫn giữ được độ ẩm cho da.</a><a>🌿 Peppermint Essential Oil: Tinh dầu bạc hà giúp làm sạch da, loại bỏ bụi bẩn và bã nhờn.</a><a>💧 PEG-7 Glyceryl Betain: Cấp ẩm, cải thiện độ mềm mịn của da và tăng khả năng giữ ẩm trên da.</a><a>🧴 Glycerin: Giữ ẩm, làm dịu da và làm chậm quá trình lão hóa.</a><a>🧼 Cocamidopropyl betain: Tạo bọt, ổn định độ bọt, làm sạch tế bào chết.</a><a>🔒 Các thành phần khác giúp bảo quản và làm sạch...</a><p>CÔNG DỤNG SẢN PHẨM:</p><a>🧼 Làm sạch: Sữa tắm gội 3 in 1 giúp làm sạch da, loại bỏ bụi bẩn, dầu nhờn trên da và tóc.</a><a>💧 Dưỡng ẩm: Giúp dưỡng ẩm, làm dịu da.</a><a>🌿 Lưu lại hương: Lưu lại hương nước hoa nam tính thơm mát trên cơ thể.</a><a>🛡️ Chăm sóc toàn diện: Chăm sóc cơ thể toàn diện, giúp phái mạnh tự tin suốt cả ngày.</a><p>HƯỚNG DẪN SỬ DỤNG:</p><a>🛁 Làm ướt cơ thể và tóc.</a><a>🧼 Lấy lượng sữa tắm vừa đủ, tạo bọt với nước hoặc bông tắm rồi tắm cho toàn thân.</a><a>🧼 Massage nhẹ nhàng lên da và da đầu để lấy đi bụi bẩn.</a><a>🚿 Xả lại bằng nước sạch.</a><p>THÔNG TIN CHUNG:</p><a>🥇 Xuất xứ: Việt Nam</a><a>📅 Hạn sử dụng: 2 năm kể từ ngày sản xuất</a><a>📅 Ngày sản xuất: Xem trên bao bì</a>",
          },
          /* Nước Hoa BODYMISS*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llszfjzmt8f304.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llbr793ybsmue1.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llbr793yg0c6e2.webp",
            name: "Nước Hoa BODYMISS",
            price: "38.880",
            code: "SPB02",
            category: "B",
            link: "https://s.shopee.vn/8pUdQpfLsu",
            description:
              "<p>🌟 GIỚI THIỆU SẢN PHẨM 🌟</p><a> Body mist của BODYMISS chính là 'vũ khí bí mật' giúp bạn tự tin tỏa sáng suốt cả ngày dài. Với khả năng lưu hương lên đến 6 tiếng, sản phẩm không chỉ khử mùi cơ thể hiệu quả mà còn xóa tan nỗi lo ám mùi đồ ăn.</a><a>✨ Lý do bạn sẽ yêu ngay BODYMISS:</a><a> - Hương thơm nhẹ nhàng, không nồng gắt như nước hoa, cực kỳ phù hợp cho học sinh, sinh viên.</a><a> - Thiết kế tiện dụng, dễ dàng mang theo mọi lúc, mọi nơi.</a><a> - Đa dạng nốt hương phù hợp với từng tâm trạng và phong cách.</a><p>💐 PHÂN LOẠI BODY MIST</p><a>1️⃣ Stop n Stare - Ngọt ngào, thu hút</a><a> - Tầng đầu: Trái cây ngọt.</a><a> - Tầng giữa: Hoa nhài.</a><a> - Tầng cuối: Hổ phách, Xạ hương.</a><a>2️⃣ Care Free - Nhẹ nhàng, tự tin</a><a> - Tầng đầu: Chanh, Táo.</a><a> - Tầng giữa: Hoa dành dành, hoa nhài.</a><a> - Tầng cuối: Gỗ đàn hương, Xạ hương, Vani.</a><a>3️⃣ Money Honey - Bí ẩn, quyến rũ</a><a> - Tầng đầu: Cam, Chanh, Quýt.</a><a> - Tầng giữa: Hoa nhài, hoa linh lan.</a><a> - Tầng cuối: Vani, Tiêu đen.</a><a>4️⃣ Funky Fresh - Tươi mát, sảng khoái</a><a> - Tầng đầu: Vỏ chanh vàng, Cam Bergamot.</a><a> - Tầng giữa: Hoa oải hương, Phong lữ.</a><a> - Tầng cuối: Gỗ tuyết tùng, Gỗ đàn hương.</a><a>5️⃣ Blinded Love - Kiêu kỳ, hấp dẫn</a><a> - Tầng đầu: Hoa mộc lan, nốt hương xanh.</a><a> - Tầng giữa: Hoa hồng, hoa nhài, hoa lan Nam Phi.</a><a> - Tầng cuối: Vani, Xạ hương.</a><a>6️⃣ Hide & Seek - Trầm ấm, lịch lãm</a><a> - Tầng đầu: Cam vàng, Quýt hồng.</a><a> - Tầng giữa: Rong biển, Hoa oải hương.</a><a> - Tầng cuối: Gỗ hoắc hương, Tuyết tùng.</a><p>📝 HƯỚNG DẪN SỬ DỤNG</p><a>Đặt chai xịt cách vùng cần xịt khoảng 15-20cm để hương tỏa đều.</a><a>Xịt lên các vùng như cổ tay, sau gáy, giữa ngực để giữ mùi lâu hơn.</a><a>Kết hợp lotion và body mist cùng dòng để tăng hiệu quả lưu hương.</a><p>⚠️ LƯU Ý</p><a>Tránh tiếp xúc trực tiếp với mắt.</a><a>Không xịt lên đồ trang sức.</a><a>Ngưng sử dụng nếu có kích ứng.</a><p>🌍 VỀ BODYMISS</p><a>Xuất xứ thương hiệu: Việt Nam.</a><a>Nơi sản xuất: Việt Nam.</a><a>Hạn sử dụng: 2 năm kể từ ngày sản xuất (xem trên bao bì).</a><p>✨ BODYMISS – Lựa chọn hoàn hảo cho mọi phong cách và tâm trạng của bạn!💖</p>",
          },
          /* Dầu Gội - Xả TRESemmé*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4jqmqnpra4nc3@resize_w450_nl.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m30cvorbal6ie8.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3g634gctsf531.webp",
            name: "Dầu Gội - Xả TRESemmé",
            price: "330.000",
            code: "SPB03",
            category: "B",
            link: "https://s.shopee.vn/60BkV2BxTc",
            description:
              "<p>✨ VÀO NẾP SUÔN MƯỢT, GIẢM GÃY RỤNG CÙNG COMBO GỘI – XẢ TRESEMMÉ MỚI ✨</p><a>👉 Tóc không vào nếp? Gãy rụng do nhiệt và hoá chất? Đừng lo lắng! Hãy để TRESemmé mang đến bí quyết chăm sóc tóc chuẩn salon ngay tại nhà!</a><p>🌟 HIỆU QUẢ VƯỢT TRỘI 🌟</p><a>🔸 Combo gội – xả KeratinBond+ :</a><a> - Phục hồi tóc khô xơ, rối, giúp tóc vào nếp suôn mượt như phục hồi Keratin tại salon*.</a><a>🔸 Combo gội – xả PeptideBond+ :</a><a> - Giảm gãy rụng đến 10 lần cho tóc hư tổn do tạo kiểu.</a><a> - Nuôi dưỡng tóc chắc khỏe từ bên trong**, giúp tóc chống lại các tác động từ hóa chất và nhiệt độ cao.</a><a>🔸 Combo gội – xả Gừng & Trà Xanh:</a><a> - Làm sạch sâu, dưỡng tóc chắc khỏe, phù hợp với tóc chịu tổn thương từ môi trường.</a><p>💡 HƯỚNG DẪN SỬ DỤNG 💡</p><a>1️⃣ Thoa đều dầu gội TRESemmé lên tóc ướt, massage nhẹ nhàng và gội sạch.</a><a>2️⃣ Sử dụng thêm dầu xả để cung cấp độ ẩm, tăng cường khả năng phục hồi tóc.</a><p>🌟 ƯU ĐIỂM NỔI BẬT 🌟</p><a>✨ Công nghệ KeratinBond+ & PeptideBond+ độc quyền từ TRESemmé.</a><a>✨ Được chuyên gia tạo mẫu tóc tin dùng.</a><a>✨ Phù hợp cho tóc nhuộm và chịu nhiều tổn thương.</a><a>✨ Công thức chuẩn salon, giúp phục hồi liên kết tóc và giữ tóc luôn bóng mượt, chắc khỏe.</a><p>🌐 Xuất xứ thương hiệu: Mỹ</p><p>📅 Ngày sản xuất, hạn sử dụng: Xem trên bao bì sản phẩm.</p><p>💡 Lưu ý:</p><a>Tránh ánh nắng trực tiếp, bảo quản nơi khô ráo.</a><a>Nếu sản phẩm dính vào mắt, rửa sạch ngay với nước.</a><p>👉 Đừng để mái tóc của bạn phải chờ đợi! Hãy trải nghiệm ngay hôm nay và cảm nhận sự khác biệt chuẩn salon tại nhà. 💆‍♀️✨</p>",
          },
          /* Vitamin E Đỏ Natura Beauty*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2f0ewzuv7as58.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2f0ex9kfl4ide.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2f0ex1ird10fc.webp",
            name: "Vitamin E Đỏ Natura Beauty",
            price: "131.000",
            code: "SPB04",
            category: "B",
            link: "https://s.shopee.vn/gAFEt9BNX",
            description:
              "<p>VITAMIN E ĐỎ NATURA BEAUTY – Bí quyết trẻ hóa làn da và duy trì sắc đẹp 🌟</p><a>💊 Sản phẩm: Vitamin E Đỏ Natura Beauty</a><a>👉 Công dụng: Hỗ trợ làm đẹp da, hạn chế lão hóa, chống oxy hóa, làm mờ thâm nám và giúp tóc chắc khỏe.</a><p>✪ THÔNG TIN SẢN PHẨM:</p><a>Thành phần chính:</a><a> - Vitamin E (DL-alpha-tocopheryl acetate): Chất chống oxy hóa mạnh.</a><a> - Evening Primrose Oil (Tinh dầu hoa anh thảo): Hỗ trợ cân bằng nội tiết, dưỡng da mềm mại.</a><a> - Aloe Vera Oil (Tinh dầu lô hội): Dưỡng ẩm và làm dịu da.</a><a> - Rosehip Oil (Tinh dầu nụ tầm xuân): Giúp làm sáng da, mờ thâm nám.</a><a>Các phụ liệu khác: Dầu đậu nành, gelatin, glycerin, sáp ong, lecithin,...</a><a>Hàm lượng Vitamin E: 2000IU.</a><a>Quy cách đóng gói: Hộp 30 viên.</a><a>Hạn sử dụng: 3 năm kể từ ngày sản xuất.</a><p>✪ TÁC DỤNG NỔI BẬT CỦA VITAMIN E ĐỎ:</p><a>🌟 Làm đẹp da:</a><a> - Chống lão hóa mạnh mẽ, cải thiện độ đàn hồi, giúp da căng mịn, trẻ trung.</a><a> - Hỗ trợ làm mờ thâm nám, vết sẹo, giúp da sáng đều màu.</a><a>🌟 Dưỡng tóc:</a><a> - Ngăn ngừa gãy rụng, kích thích mọc tóc.</a><a> - Giúp tóc mềm mượt, hạn chế khô xơ, chẻ ngọn.</a><a>🌟 Bảo vệ sức khỏe:</a><a> - Chống gốc tự do, bảo vệ tế bào khỏi tổn thương do oxy hóa.</a><a> - Hỗ trợ duy trì sức khỏe hệ tim mạch, hạn chế xơ cứng động mạch.</a><p>✪ ĐỐI TƯỢNG SỬ DỤNG:</p><a>Người có làn da khô, thiếu sức sống.</a><a>Người muốn duy trì thanh xuân, chống lão hóa.</a><a>Những người có chế độ ăn uống không đầy đủ, cần bổ sung vitamin E.</a><p>✪ HƯỚNG DẪN SỬ DỤNG:</p><a>📌 Liều dùng: Uống 2 lần/ngày, mỗi lần 1 viên (sau bữa ăn 30 phút).</a><a>⚠️ Lưu ý: Không dùng cho người mẫn cảm với bất kỳ thành phần nào của sản phẩm.</a>",
          },
          /* Sức Khỏe & Làm Đẹp*/
          /* Quạt Mini Có LED*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3aczmzj3jcsc3.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lua61kdxlnv517.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lua61kdx4t1t8f.webp",
            name: "Quạt Mini Có LED",
            price: "329.000",
            code: "SPC01",
            category: "C",
            link: "https://s.shopee.vn/5VEBSmY4yy",
            description:
              "<p>LUỒNG KHÍ MẠNH MẼ CỦA ĐỘNG CƠ TURBO:</p><a >🌀 Động cơ không chổi than turbo hiệu quả với tốc độ quay 16000 vòng/phút.</a ><a>🔊 Quạt cầm tay yên tĩnh tạo ra ít tiếng ồn hơn dưới 25db.</a><a>🌬️ Tạo ra không khí mạnh mẽ với tốc độ nhanh tối đa 9m/s.</a><a>📏 Khoảng cách làm mát lên đến 5 mét.</a><a >💨 Quạt phản lực giải phóng luồng không khí nén và tập trung đã được lọc, mát như không khí từ điều hòa.</a ><p>ĐIỀU CHỈNH TỐC ĐỘ VÔ CẤP 100:</p><a>🔘 100 tốc độ gió tùy chỉnh để đáp ứng mọi nhu cầu khác nhau.</a><a >🔃 Có 2 nút điều chỉnh để tăng hoặc giảm tốc độ gió một cách linh hoạt.</a ><a >🔧 Tùy chỉnh liền mạch từng bước tốc độ cụ thể bằng cách nhấn và giữ các nút.</a ><p>MÀN HÌNH KỸ THUẬT SỐ LED TRỰC QUAN:</p><a>🔌 Màn hình LED hiển thị tốc độ gió và mức pin.</a><a>📊 Biểu tượng pin sẽ nhấp nháy khi mức pin thấp hơn 10%.</a><a >🔆 Vòng tròn dải đèn xung quanh màn hình chạy theo nhịp của tốc độ gió.</a ><p>ĐÚC TÍCH HỢP BỀN:</p><a>🔧 Quạt được làm từ vật liệu có độ bền kéo cao, đúc liền mạch.</a><a>🔐 Ngăn ngừa các vết nứt hoặc biến dạng trong thời gian dài sử dụng.</a><a>👋 Tay cầm bo tròn vừa vặn thoải mái với lòng bàn tay.</a><p>PIN KÉO DÀI VỚI CỔNG TYPE-C:</p><a >🔋 Pin 4000mAH tích hợp có thể chịu được thời gian làm việc từ 2 đến 10 giờ.</a ><a>🔋 Sạc đầy trong 2,3 giờ và hỗ trợ sạc nhanh từ nhiều nguồn.</a><a>🔄 Cáp sạc Type-C đi kèm tiện dụng.</a><p>DÂY BUỘC CHỐNG THẤT LẠC TIỆN DỤNG:</p><a>🔗 Dây buộc chống thất lạc giúp bạn dễ dàng mang quạt bên mình.</a><a>🔗 Ngăn quạt rơi xuống đất một cách vô tình.</a><p>ỨNG DỤNG DI ĐỘNG VÀ RỘNG RÃI:</p><a>📱 Kích thước nhỏ gọn, chỉ 15x6,2x5,8cm.</a><a>📱 Nặng 330g, dễ dàng bỏ vào túi hoặc túi xách.</a><a>💼 Có thể sử dụng như quạt cầm tay hoặc quạt để bàn.</a><a>🎁 Trở thành món quà hoàn hảo cho bạn bè hoặc gia đình của bạn.</a>",
          },
          /* Đồng Hồ Thông Minh*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/723bde85ff12ce5cb4160b1ec0956f20.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/18fa4ce33d9ed53de23ca3b99e5742a0.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/75daf60465e1496e7a0bbcb87636a5d1.webp",
            name: "Đồng Hồ Thông Minh",
            price: "64.000",
            code: "SPC02",
            category: "C",
            link: "https://s.shopee.vn/1LOcV91DZv",
            description:
              "<p>ĐẶC ĐIỂM:</p><a >🛡️ Chống thấm nước IP67: Hỗ trợ rửa tay, đi mưa, mặc bơi lội, đáp ứng nhu cầu hàng ngày (lưu ý: không thể đeo khi tắm nước nóng và xông hơi khô).</a ><a >💓 Theo dõi sức khỏe: Theo dõi huyết áp, theo dõi nhịp tim, theo dõi giấc ngủ, nhắc nhở ít vận động.</a ><a>🏃‍♂️ Chức năng thể thao tiêu chuẩn: Bước, calo, tính khoảng cách.</a><a >🖥️ Màn hình: 3 loại kiểu giao diện UI (công tắc nhấn và giữ giao diện chính), hiển thị thời gian, hiển thị ngày.</a ><a>🏅 Nhiều chế độ thể thao.</a><a >📱 Đẩy nhắc cuộc gọi và thông tin: Kết nối với Fitpro APP, hiển thị cuộc gọi, tin nhắn văn bản và SNS (Twitter, Line, WhatsApp, Facebook, Line, KaKaoTalk, WeChat, QQ) và các thông báo khác; không bao giờ bỏ lỡ thông tin quan trọng.</a ><a >🕰️ Các chức năng khác: Đồng hồ báo thức, đồng hồ bấm giờ, giơ tay lên để làm sáng màn hình, camera từ xa, tìm vòng đeo tay.</a ><p>THÔNG TIN CHI TIẾT:</p><a>📱 App: Fitpro / Hryfine</a><a>📏 Chất liệu vỏ: Hợp kim nhôm</a><a>📿 Chất liệu dây đeo: TPU</a><a>📱 Màn hình: Màn hình đầy màu sắc IPS 1,3 inch</a><a>📶 Chip: HS6620D</a><a>🔋 Phiên bản Bluetooth: 4.0</a><a >💧 Lớp chống thấm nước: IP67 (lưu ý: không thể đeo cho tắm nước nóng và phòng xông hơi khô).</a ><a>🔋 Dung lượng pin: 100mAh</a><a>⏳ Thời gian sạc: khoảng 2 giờ</a><a>⏳ Thời gian làm việc: 5 ngày</a><a>⏳ Thời gian chờ: khoảng 10 ngày</a><a>🔌 Chế độ sạc: USB tích hợp</a><a>🔘 Nút chức năng: Nút một chạm</a><a>💻 Hệ thống tương thích: Android 4.4 trở lên, IOS 8.0 trở lên.</a><p>LÀM THẾ NÀO ĐỂ GHÉP NỐI VỚI ĐIỆN THOẠI CỦA BẠN?</p><a >💡 Mẹo: Sử dụng ứng dụng Fitpro thay vì kết nối trực tiếp với thiết bị qua Bluetooth.</a ><a>🔗 1. Tải xuống và cài đặt ứng dụng Fitpro trên điện thoại của bạn.</a><a>🔗 2. Mở Bluetooth của điện thoại.</a><a >🔗 3. Mở ứng dụng, nhấp vào Thiết bị: tìm kiếm thiết bị của bạn và nhấp vào nó.</a ><p>GHI CHÚ:</p><a >📊 1. Các thiết bị đeo được giám sát các hoạt động của con người thông qua các cảm biến điện tử và chúng ở cấp độ điện tử tiêu dùng.</a ><a >📊 2. Nó là bình thường cho độ lệch nhất định. Người dùng nên xử lý dữ liệu một cách khách quan. Vui lòng không so sánh với thiết bị bệnh viện về việc đọc, nó KHÔNG phải là thiết bị y tế.</a ><a >⭐ 3. Hầu hết hầu hết các đồng hồ thông minh không có bộ sạc hoặc pin nhỏ, khi bạn nhận được có thể cần sạc 40-50 phút, nó sẽ tự mở</a ><p>GÓI HÀNG BAO GỒM:</p><a>1 x đồng hồ</a><a>1 x Hướng dẫn sử dụng</a><a>Hoặc</a><a>1 * Dây đồng hồ</a>",
          },
          /* Sạc Dự Phòng 20W*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-luk3f0wjjeam41.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-lnr0606h6zkrfd.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-lnr2lvobomfc9e.webp",
            name: "Sạc Dự Phòng 20W",
            price: "449.000",
            code: "SPC03",
            category: "C",
            link: "https://s.shopee.vn/5AbL4DGshp",
            description:
              "<p>ĐÓNG GÓI:</p><a>1 * PowerBank 20000mAh</a><p>THÔNG TIN:</p><a>Thương hiệu: Baseus</a><a>🔧 Tên: Ngân hàng điện</a><a>🔧 Mẫu số: PPAP20K</a><a>🔋 Pin: Pin Lithium Polymer</a><a>🔋 Công suất nguồn: 20000mAh / 74Wh</a><a>⚡ Tỷ lệ chuyển đổi năng lượng: ≥ 75%</a><a>🔌 Đầu vào vi mô: 5V-2A; 9V-2A</a><a>🔌 Đầu vào loại: 5V = 3A; 9V = 2A</a><a>🔌 Đầu ra USB: 5V = 3A; 9V = 2A; 12V = 1.5A</a><a>🔌 Đầu ra loại C: 5V = 3A; 9V = 2,22A; 12V = 1,5A</a><a>⚡ Tổng đầu ra: 5V-3A</a><a>📏 Kích thước: 153,5 ” 69,4 ” 29,6mm</a><a>📏 Khối lượng tịnh: ≈ 446g</a><p>TÍNH NĂNG SẢN PHẨM:</p><a>🔌 Sạc nhanh PD 20W</a><a>🔌 Sạc lại nhanh 18W</a><a>💼 Luôn sẵn sàng đi du lịch</a><a>🧳 Thiết kế nhỏ gọn, tiện lợi mang đi mọi nơi</a><a>🎒 Hỗ trợ nhiều thiết bị cùng lúc</a>",
          },
          /* Điện Thoại Vivo V23 5G*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1nvez3metsjbc.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1m3avweef271d.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1m3avweftmn19.webp",
            name: "Điện Thoại Vivo V23 5G",
            price: "1.988.950",
            code: "SPC04",
            category: "C",
            link: "https://s.shopee.vn/9zgap9wWPX",
            description:
              "<p>NỀN TẢNG:</p><a>🖥 Bộ xử lý: MediaTek dimension 920</a><a>💾 Bộ nhớ: RAM 8GB + ROM 256GB</a><a>🔋 Pin: 4200mAh</a><a>⚡ Sạc nhanh: 44W (11V/4A)</a><a>📱 Hệ điều hành: Funtouch OS 12</a><p>MÀU SẮC:</p><a>🌌 Bụi sao đen 🌑</a><a>🌞 Nắng vàng 🌞</a><p>MÀN HÌNH:</p><a>🔍 Độ phân giải: 2400x1080 (FHD+)</a><a>📏 Kích thước: 6,44 inch, AMOLED</a><a>🖱 Cảm ứng: Cảm ứng đa điểm điện dung</a><p>MẠNG:</p><a>📶 Loại SIM: Nano SIM kép</a><a>📴 Chế độ chờ: DSDS</a><a>📡 Mạng di động 2G GSM: B2/B3/B5/B8</a><a>📡 3G WCDMA: B1/B2/B4/B5/B8</a><a>📡 CDMA: Trước Công Nguyên</a><a>📶 4G TDD-LTE: B38/B39/B40/B41</a><a>📶 4G FDD-LTE: B1/B2/B3/B4/B5/B7/B8/B12/B17/B18/B19/B20/B26/B28/B32</a><a>📶 5G: n1/n3/n5/n8/n7/n20/n28/n38/n40/n41/n77/n78</a><p>MÁY ẢNH:</p><a>📷 Máy ảnh: Mặt trước 50MP AF + góc rộng 8MP/Mặt sau 64MP AF + góc rộng 8MP + macro 2MP</a><a>Miệng vỏ:</a><a>- Mặt trước: chính f/2.0, góc rộng f/2.28</a><a>- Mặt sau: chính f/1.89, góc rộng f/2.2, macro f/2.4</a><a>💡 Tốc biến: Đèn flash sau + Đèn rọi 2 tông màu</a><a>🖌 Chế độ:</a><a>- Mặt trước: Tự động lấy nét, AI Extreme Night, Video selfie Steadiface, Chân dung nhiều phong cách, Phơi sáng kép, Làm đẹp khuôn mặt bằng video, Video chế độ xem kép, Chuyển động chậm, Độ phân giải cao, Ảnh trực tiếp, Nhãn dán AR, Chân dung tự nhiên</a><a>- Mặt sau: Tự động lấy nét mắt, Ban đêm, Đêm siêu rộng, Siêu cận cảnh, Chân dung Bokeh, Bộ lọc chân dung, Chân dung Bokeh Flare, Độ phân giải cao, Ảnh trực tiếp, Nhãn dán AR, Chuyển động chậm, Tua nhanh thời gian, Video chế độ xem kép, Phơi sáng kép, Tài liệu, Toàn cảnh, Chuyên nghiệp, Siêu ổn định</a><p>PHƯƠNG TIỆN TRUYỀN THÔNG:</p><a>🎧 Phát lại âm thanh: AAC, OGG, FLAC, WMA, WAV, APE, MP3, MP2, MP1, OPUS, M4A</a><a>📽 Xem lại video: MP4, 3GP, AVI, FLV, MKV</a><a>📹 Quay video: MP4</a><a>🎤 Ghi âm giọng nói: Được hỗ trợ</a><p>KẾT NỐI:</p><a>📶 Wifi: 2,4GHz, 5GHz</a><a>🔗 Bluetooth: Bluetooth 5.2</a><a>🔌 USB: Loại C</a><a>📍 GPS: Được hỗ trợ</a><a>📱 OTG: Được hỗ trợ</a><a>🌐 NFC: Được hỗ trợ</a><p>CẢM BIẾN:</p><a>🔐 Dấu vân tay: Quét vân tay trong màn hình</a><a>📏 Gia tốc kế: Được hỗ trợ</a><a>🌑 Cảm biến ánh sáng xung quanh: Được hỗ trợ</a><a>📶 Cảm biến tiệm cận: Được hỗ trợ</a><a>📉 La bàn điện tử: Được hỗ trợ</a><a>🔄 Con quay hồi chuyển: Được hỗ trợ</a><p>VỊ TRÍ:</p><a>GPS, BEIDOU, GLONASS, GALILEO, QZSS</a>",
          },
          /* Thiết Bị Điện Tử*/
          /* Giấy VS Treo Tường TopGia*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4fga7c9834f2d.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lu2e1og5xixr45.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lu1tpa981vrz9c.webp",
            name: "Giấy VS Treo Tường TopGia",
            price: "95.000",
            code: "SPD01",
            category: "D",
            link: "https://s.shopee.vn/30Y9z11uIX",
            description:
              "<p>🔥 GIẤY VỆ SINH TREO TƯỜNG TOP GIA – ĐA DẠNG SỰ LỰA CHỌN, ĐA TIỆN ÍCH 🔥</p><p>📦 SẢN PHẨM ĐIỂM NHẤN</p><a>Thùng 6 bịch, 4 bịch, 3 bịch đa sắc: Đáp ứng nhu cầu sử dụng cá nhân, gia đình, hoặc doanh nghiệp.</a><a>Chất liệu cao cấp: Làm từ bột gỗ nguyên chất, an toàn và thân thiện với làn da.</a><a>Độ dày vượt trội: 1280 tờ với 4 lớp siêu dày, mềm mại, không bụi giấy, thấm hút tốt.</a><a>Tiện ích đa năng: Thùng giấy treo dễ dàng lắp đặt, tối ưu không gian sử dụng.</a><p>🌍 XUẤT XỨ</p><a>Sản xuất tại Việt Nam: Kho miền Nam.</a><a>Sản xuất tại Trung Quốc: Kho miền Bắc.</a><p>⏳ HẠN SỬ DỤNG & BẢO QUẢN</p><a>Hạn sử dụng: 3 năm kể từ ngày sản xuất.</a><a>Hướng dẫn bảo quản: Để nơi khô ráo, thoáng mát.</a><a>Lưu ý: Ngưng sử dụng nếu có dấu hiệu dị ứng với bất kỳ thành phần nào trong sản phẩm.</a><p>🎁 KHUYẾN MÃI ĐẶC BIỆT</p><a>Mua sản phẩm là có quà tặng kèm hấp dẫn!</a><p>Hãy trải nghiệm giấy vệ sinh treo tường Top Gia, sự lựa chọn hoàn hảo cho mọi nhu cầu vệ sinh cá nhân và gia đình! 🌟</p>",
          },
          /* Giấy Ăn Rút TopGia*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4fw622b1o4w5d.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lu06nj9rty4x4e.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lsdpe247ogih27.webp",
            name: "Giấy Ăn Rút TopGia",
            price: "119.000",
            code: "SPD02",
            category: "D",
            link: "https://s.shopee.vn/8KZgLJQkaI",
            description:
              "<p>THÔNG TIN SẢN PHẨM 🌟</p><a>Thành phần chính: 100% bột gỗ nguyên sinh 🌳</a><a>Hạn sử dụng: 3 năm kể từ ngày sản xuất 📆</a><a>Kích thước tờ: 115 x 163mm 📏</a><a>Quy cách: 300 tờ / 4 lớp / 75 rút 🧻</a><a>Phân loại: Thùng 16 gói, 30 gói 📦</a><a>Ứng dụng: Thích hợp cho cả gia đình 👨‍👩‍👧‍👦</a>",
          },
          /* Nhà Cửa & Đời Sống*/
          /* Máy Hút Sữa Đôi TopGiaKids*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4jvcdtunkbk74.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m26f5y5ttrck14.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m26f7kom6qb88c.webp",
            name: "Máy Hút Sữa Đôi TopGiaKids",
            price: "519.000",
            code: "SPE01",
            category: "E",
            link: "https://s.shopee.vn/5AcigeECKj",
            description:
              "<p>✨ Đặc Điểm Nổi Bật:</p><a>Công nghệ hiện đại: Máy được trang bị hệ thống cảm ứng thông minh, dễ dàng điều chỉnh chế độ bằng thao tác chạm nhẹ.</a><a>Không dây tiện lợi: Giúp mẹ thoải mái hút sữa mọi lúc, mọi nơi mà không bị vướng víu dây cắm.</a><a>Lực hút mạnh mẽ: Mô phỏng lực hút tự nhiên của bé, giúp kích thích sữa về nhanh hơn mà vẫn đảm bảo nhẹ nhàng, không gây đau rát.</a><a>Đa chế độ: Có thể tùy chỉnh chế độ massage và hút phù hợp với nhu cầu, giảm căng tức và hỗ trợ duy trì nguồn sữa.</a><a>Chất liệu an toàn: Được làm từ nhựa PP và silicone y tế không chứa BPA, đảm bảo an toàn tuyệt đối cho mẹ và bé.</a><a>Thiết kế nhỏ gọn: Phù hợp để mang đi làm, du lịch hoặc sử dụng tại nhà.</a><p>📋 Thông Số Kỹ Thuật:</p><a>Tên sản phẩm: Máy hút sữa điện không dây TopGiaKids</a><a>Chất liệu: Nhựa PP cao cấp, silicone y tế an toàn</a><a>Dung lượng pin: Pin sạc dung lượng lớn, sử dụng lâu dài</a><a>Chế độ hoạt động:</a><a> - Massage nhẹ nhàng</a><a> - Hút sữa mạnh mẽ</a><a>Kích thước: Nhỏ gọn, dễ cầm nắm</a><p>🎯 Ưu Điểm:</p><a>Giảm thiểu tình trạng căng tức ngực.</a><a>Bảo vệ đầu ti khỏi tổn thương nhờ chế độ massage êm ái.</a><a>Tiết kiệm thời gian, phù hợp với mẹ bận rộn.</a><a>Hỗ trợ duy trì và tăng cường lượng sữa mẹ.</a><p>📦 Nội Dung Bộ Sản Phẩm Bao Gồm:</p><a>1 Máy hút sữa không dây TopGiaKids.</a><a>1 Dây sạc USB tiện lợi.</a><a>1 Bộ phễu hút bằng silicone mềm mại.</a><a>1 Sách hướng dẫn sử dụng chi tiết.</a><p>💡 Lưu Ý Khi Sử Dụng:</p><a>Vệ sinh máy và phụ kiện trước và sau mỗi lần sử dụng để đảm bảo vệ sinh.</a><a>Không để nước tràn vào phần động cơ máy.</a><a>Sạc đầy pin trước khi sử dụng lần đầu tiên.</a><a>Đọc kỹ hướng dẫn để sử dụng máy đúng cách và hiệu quả.</a><p>💖 TopGiaKids – Đối tác tin cậy của mẹ bỉm sữa!</a>",
          },
          /* Vinamilk Dielac Alpha Gold 4*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m21xf5v3qz6jc5.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m21xfdt65rbvc8.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m21xfbgtjsgu76.webp",
            name: "Vinamilk Dielac Alpha Gold 4",
            price: "451.880",
            code: "SPE02",
            category: "E",
            link: "https://s.shopee.vn/7V0dTbFZ22",
            description:
              "<p>Sữa Bột Dielac Alpha Gold 4 – 1400g</p><a>Dành cho trẻ từ 2 đến 6 tuổi</a><p>✨ Công thức đột phá COMPLET-IQ:</p><a>Sữa Dielac Alpha Gold 4 tích hợp công thức tiên tiến, bổ sung Sữa non 24h nhập khẩu từ Mỹ, giúp tăng cường sức đề kháng, cải thiện tiêu hóa, và hỗ trợ phát triển toàn diện cho trẻ nhỏ.</a><p>Đặc Điểm Nổi Bật</p><a>1️⃣ Hỗ Trợ Tăng Sức Đề Kháng:</a><a> - Sữa non 24h nhập khẩu từ Mỹ giàu kháng thể IgG.</a><a> - Kết hợp các khoáng chất thiết yếu như Kẽm, Selen, cùng Vitamin A, D, C giúp bảo vệ cơ thể trẻ khỏi các bệnh nhiễm khuẩn thông thường.</a><a>2️⃣ Hỗ Trợ Phát Triển Não Bộ:</a><a> - Bổ sung DHA đạt tiêu chuẩn khuyến nghị của FAO/WHO.</a><a> - Kết hợp với ARA, Axít Linoleic, Axít Alpha-Linolenic, Choline, Taurine, Lutein, giúp phát triển não bộ, thị giác và tăng cường khả năng ghi nhớ.</a><a>3️⃣ Hỗ Trợ Phát Triển Chiều Cao:</a><a> - Tỉ lệ Canxi – Phốt pho (Ca:P) cân đối, cùng Vitamin D, K, Magiê thúc đẩy sự phát triển của xương và chiều cao cho trẻ.</a><a>4️⃣ Giúp Tăng Cân, Tiêu Hóa Khỏe:</a><a> - Bổ sung 36 dưỡng chất thiết yếu, giúp trẻ tăng cân khỏe mạnh.</a><a> - Hỗ trợ tiêu hóa với lợi khuẩn Bifidobacterium, BB-12™ và chất xơ hòa tan FOS, tăng cường vi khuẩn có lợi trong đường ruột và tối ưu hóa khả năng hấp thu.</a><p>Thông Tin Sản Phẩm</p><a>Tên sản phẩm: Dielac Alpha Gold 4</a><a>Khối lượng: 1400g</a><a>Độ tuổi sử dụng: Trẻ từ 2 - 6 tuổi</a><a>Hạn sử dụng: 24 tháng</a><a>Xuất xứ: Việt Nam</a><p>Lợi Ích Chính</p><a>Tăng cường miễn dịch, giảm nguy cơ mắc bệnh.</a><a>Phát triển trí não, thị giác và khả năng học hỏi.</a><a>Hỗ trợ xương chắc khỏe, giúp trẻ cao lớn.</a><a>Cải thiện tiêu hóa và hấp thụ dinh dưỡng hiệu quả.</a><p>Dielac Alpha Gold 4 – Người bạn đồng hành tin cậy, giúp bé yêu phát triển toàn diện và khỏe mạnh!</p>",
          },
          /* Mẹ & Bé*/
          /* Bước Tập Thể Dục*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1weutxrkgxr2c.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lyz18vb77w3x7b.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lyz18v99aqfhf0.webp",
            name: "Bước Tập Thể Dục",
            price: "499.000",
            code: "SPF01",
            category: "F",
            link: "https://s.shopee.vn/6AVFrBPVnV",
            description:
              "<p>🔥 BƯỚC TẬP THỂ DỤC – Đồng hành cùng sức khỏe của bạn! 🔥</p><p>【Thông Tin Chi Tiết Sản Phẩm】 📋</p><a>Tên sản phẩm: Bước tập thể dục 🏃‍♂️🏃‍♀️</a><a>Kích thước: W28,5cm x L31,5cm x H18cm 📏</a><a>Trọng lượng: 6kg ⚖️</a><a>Trọng lượng hỗ trợ: Lên tới 200 kg 💪</a><a>Chất liệu: Nhựa PP, Thép xanh 🛠️</a><a>Luyện tập thể thao: Đi bộ, Xây dựng cơ bắp, Tập aerobic 🏋️‍♂️🤸‍♀️</a><a>Kết quả tập luyện: Rèn luyện các cơ tay, hông, chân và bắp chân 💥</a><p>【Tính Năng】 ✨</p><a>Nhỏ gọn và di động: Phù hợp với mọi ngóc ngách trong gia đình 🏠</a><a>Tiếp xúc an toàn: Bàn đạp và nút không bị trượt, dễ dàng làm sạch 🧼</a><a>Chức năng massage chân: Cởi giày, thư giãn và vui vẻ sau mỗi buổi tập 👟💆‍♀️</a><a>Hiển thị thông tin: Tốc độ (số bước mỗi phút), thời gian và lượng calo đốt cháy 📊⏰🔥</a><a>Vòng quay tối đa: 30 pound, điều chỉnh độ dài của mũi khâu 🔄</a><a>Màn hình dễ đọc: Pin có thể thay thế (một pin LR44, không bao gồm pin) 🔋</a><a>Độ bền cao: Hỗ trợ trọng lượng tối đa 200 kg, tuổi thọ cao 🔧</a><a>Phù hợp mọi lứa tuổi: Đặc biệt thích hợp cho những người bận rộn muốn giảm cân nhanh chóng 👨‍👩‍👧‍👦</p><a>Cơ bắp săn chắc: Giúp cơ bắp săn chắc, ổn định và đốt cháy mỡ thừa 💪🔥</a><a>Hỗ trợ gia đình: Sử dụng cùng xem TV, nghe nhạc, tăng thêm niềm vui 🎶📺</a><p>【Khuyên Bảo】 🛡️</p><a>Lắp pin: Đặt pin LR44 vào phía sau cẩn thận để không làm hỏng sản phẩm 🔋</a><a>Vệ sinh: Làm sạch bằng vải ẩm và lau khô để tránh vết mồ hôi tích tụ 🧽🧴</a><a>Kiểm tra sản phẩm: Luôn kiểm tra xem có vết rách hoặc lỏng lẻo trước khi tập để tránh chấn thương 🚫🩹</a><a>Các biện pháp phòng ngừa:</a><a>Hình ảnh sản phẩm chỉ mang tính tham khảo. Màu sắc thực tế có thể thay đổi tùy theo ánh sáng và màn hình 📸🔍</a><p>【Nội Dung Gói】 📦</p><a>✔️ Bước nhỏ *1</a><a>✔️ Dây kéo kháng lực *2</a><p>🌟 TẠI SAO CHỌN BƯỚC TẬP THỂ DỤC? 🌟</p><a>Tiện lợi: Nhỏ gọn, dễ dàng di chuyển và lắp đặt ở bất kỳ nơi nào trong nhà.</a><a>Đa chức năng: Không chỉ giúp bạn tập luyện mà còn hỗ trợ thư giãn với chức năng massage chân.</a><a>An toàn và bền bỉ: Chất liệu cao cấp, đảm bảo an toàn và sử dụng lâu dài.</a><a>Hiệu quả: Giúp bạn đốt cháy calo, săn chắc cơ bắp và duy trì sức khỏe tốt.</a><p>🚀 ĐẶT HÀNG NGAY HÔM NAY 🚀</p><a>Hãy sở hữu Bước tập thể dục để bắt đầu hành trình chăm sóc sức khỏe của bạn và gia đình ngay hôm nay! 💖</a><p>BƯỚC TẬP THỂ DỤC – Sức khỏe trong tầm tay bạn! 🏅✨</p>",
          },
          /* Giày Thể Thao AF 1 LV*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m42wlafav85j0d.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m42wik6qmkj471.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m42wilrmbbzka4.webp",
            name: "Giày Thể Thao AF 1 LV",
            price: "169.000",
            code: "SPF02",
            category: "F",
            link: "https://s.shopee.vn/1B6ZukLVMx",
            description:
              "<p>👉 Hướng Dẫn Sử Dụng:</p><a>⛔ Không sử dụng hóa chất hoặc bột giặt có hoạt tính tẩy rửa mạnh để làm sạch giày, tránh làm hỏng chất liệu.</a><a>⛔ Không dùng bàn chải cứng để chà xát, dễ gây trầy xước hoặc làm hư hỏng bề mặt giày.</a><a>⛔ Tránh đi mưa hoặc ngâm giày trong nước lâu, dễ làm giảm tuổi thọ sản phẩm.</a><a>⛔ Không phơi trực tiếp dưới nắng gắt, tránh gây biến dạng hoặc bay màu.</a><a>⛔ Vệ sinh thường xuyên đối với giày có màu sáng để giữ sản phẩm luôn như mới.</a><a>⛔ Không cất giữ giày khi còn ướt hoặc ẩm, tránh mùi hôi hoặc nấm mốc.</a><p>💥 LƯU Ý:</p><a>📸 Tất cả hình ảnh và video đều được shop tự chụp bằng điện thoại, không chỉnh sửa, đảm bảo chân thực!</a><p>Cảm ơn bạn đã ủng hộ và đồng hành cùng shop! 💖</p>",
          },
          /* Thể Thao & Du Lịch*/
          /* Khô Bò Củ Chi*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lwo3wm4a6py171.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lwi0mvo502qhf8.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lwi0mvo4yo6141.webp",
            name: "Khô Bò Củ Chi",
            price: "220.000",
            code: "SPG01",
            category: "G",
            link: "https://s.shopee.vn/2Az5hL2zuh",
            description:
              "<p>KHÔ BÒ MIẾNG TASTY FOOD – Món ngon hấp dẫn cho mọi dịp 🎉</p><p>GIỚI THIỆU:</p><a>🥩 Khô bò miếng Tasty Food mang đến hương vị thơm ngon đặc biệt nhờ sự kết hợp tinh tế giữa thịt bò tươi nguyên chất và ngũ vị hương, tạo nên món ăn đậm đà, cay cay, cực kỳ kích thích vị giác.</a><a>✨ Một thớ thịt bò dày dặn, được ướp gia vị kỹ càng, kết hợp vị cay nhẹ của ớt, thích hợp để làm món ăn nhâm nhi cùng bạn bè, người thân trong các buổi tụ họp hoặc đơn giản là món ăn chơi hằng ngày.</a><a>💯 Khô bò nhà làm Tasty, với kinh nghiệm hơn 20 năm, đảm bảo nguyên liệu THẬT 100%, thơm ngon, chất lượng từ mẻ đầu tiên đến tay bạn.</a><p>QUY CÁCH SẢN PHẨM:</p><a>Tên sản phẩm: Khô Bò Miếng Tasty Food.</a><a>Khối lượng: 500G hoặc 1000G (bao gồm cả bao bì).</a><a>Đóng gói:</a><a> - Sản phẩm được bảo quản trong hũ chắc chắn, đảm bảo vệ sinh an toàn thực phẩm.</a><a> - Đóng thùng carton cẩn thận, vừa bảo vệ hàng hóa tốt, vừa lịch sự khi làm quà tặng.</a><a>Hạn sử dụng: 6 tháng kể từ ngày sản xuất.</a>",
          },
          /* Táo đỏ Tân Cương Hoà Điền*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4q88y9s3imfe2.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4q1757n01jja0.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m4q88y9s3imfe2.webp",
            name: "Táo đỏ Tân Cương Hoà Điền",
            price: "135.000",
            code: "SPG02",
            category: "G",
            link: "https://s.shopee.vn/BE1KvVpak",
            description:
              "<p>TÁO ĐỎ TÂN CƯƠNG – Quà tặng sức khỏe từ thiên nhiên 🍎</p><p>🟢 THÔNG TIN SẢN PHẨM:</p><a>Nguồn gốc: Tân Cương – vùng đất nổi tiếng với sản phẩm táo đỏ thơm ngon, chất lượng.</a><a>Khối lượng: Túi 1kg tiện lợi.</a><a>Ngày sản xuất: Được in rõ trên vỏ hộp.</a><a>Hạn sử dụng: 12 tháng kể từ ngày sản xuất.</a><p>🟢 ĐỐI TƯỢNG NÊN SỬ DỤNG TÁO ĐỎ TÂN CƯƠNG:</p><a>🌟 Táo đỏ Tân Cương là lựa chọn hoàn hảo, giàu dinh dưỡng, phù hợp cho các đối tượng sau:</a><a>Mẹ bầu: Giúp bổ sung sắt, tăng cường sức đề kháng, hỗ trợ thai kỳ khỏe mạnh.</a><a>Mẹ sau sinh: Hỗ trợ hồi phục sức khỏe, cung cấp năng lượng và chất dinh dưỡng.</a><a>Người thiếu máu: Giàu sắt tự nhiên, cải thiện tình trạng thiếu máu hiệu quả.</a><a>Người khó ngủ: Táo đỏ giúp thư giãn, hỗ trợ giấc ngủ ngon và sâu hơn.</a><a>Người suy yếu vóc dáng: Bổ sung dưỡng chất, giúp cơ thể khỏe mạnh, phục hồi sức sống.</a><a>Người sau phẫu thuật: Hỗ trợ tăng cường miễn dịch và phục hồi nhanh chóng.</a><p>LÝ DO BẠN NÊN CHỌN TÁO ĐỎ TÂN CƯƠNG?</p><a>✔️ Chất lượng cao cấp: Được chọn lọc từ vùng đất nổi tiếng, táo đỏ Tân Cương đảm bảo sạch, không chất bảo quản.</a><a>✔️ Giàu dinh dưỡng: Bổ sung vitamin, khoáng chất và chất xơ cần thiết cho cơ thể.</a><a>✔️ Đa dụng: Có thể dùng ăn trực tiếp, pha trà hoặc nấu cùng các món ăn để tăng hương vị và giá trị dinh dưỡng.</a><p>🌟 MUA NGAY để chăm sóc sức khỏe bản thân và gia đình từ những điều nhỏ nhất! 🍎</p>",
          },
          /* Tiêu Dùng*/
          /* Tư Duy Ngược*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lwxpv4ydgxjt57@resize_w450_nl.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7qukw-ljhy12voht6q4c.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7qukw-ljhy12venu2qca@resize_w450_nl.webp",
            name: "Tư Duy Ngược",
            price: "125.000",
            code: "SPH01",
            category: "H",
            link: "https://s.shopee.vn/20fbfhq1ox",
            description:
              "<p>TƯ DUY NGƯỢC - Nguyễn Anh Dũng 🌟</p><a>Bạn đã từng tự hỏi:</a><a>❓ Chúng ta có thật sự hạnh phúc không?</a><a>❓ Chúng ta có đang sống đúng với chính mình?</a><a>❓ Liệu mình có dám vượt qua khuôn mẫu, định kiến để khẳng định bản sắc riêng? </a><a> Nếu bạn đã từng trăn trở nhưng chưa có câu trả lời, thì đây chính là cuốn sách dành cho bạn.</a><a> 📖 'Tư Duy Ngược' được viết dựa trên những câu chuyện đời sống, nghiên cứu sâu sắc và trải nghiệm cá nhân của tác giả Nguyễn Anh Dũng. Cuốn sách giúp bạn: </a><a> - Hiểu rõ bản thân và nhận diện những rào cản trong cuộc sống. </a><a> - Học cách tư duy ngược dòng, thoát khỏi lối mòn để tìm đến sự sáng tạo và thành công. </a><a> - Sở hữu các phương pháp thực tiễn để can đảm sống cuộc đời bạn mong muốn. </a><a>🔥 Đây không chỉ là một cuốn sách, mà là lời mời gọi bạn bứt phá để tìm kiếm hạnh phúc thực sự trong cuộc đời.</a><p>TƯ DUY MỞ - Nguyễn Anh Dũng 🚀</p><a> 🌐 Trong kỷ nguyên công nghệ số, khi thế giới thay đổi từng giây, điều bạn cần nhất là một tư duy mở để linh hoạt thích ứng và bắt kịp xu hướng. </a><a>Người có tư duy mở luôn:</a><a> - Tin tưởng vào sự thay đổi và nỗ lực để tiến bộ hơn mỗi ngày.</a><a>Đón nhận thử thách như cơ hội học hỏi, không sợ thất bại mà coi đó là bài học quý giá. </a><a> - Sẵn sàng thay đổi góc nhìn, thử nghiệm nhiều cách khác nhau để đạt được kết quả tốt hơn. </a><a>📘 'Tư Duy Mở' sẽ giúp bạn:</a><a> - Nhận diện loại tư duy của mình – đang đóng hay mở?</a><a> - Hiểu rõ vai trò của tư duy mở trong việc phát triển bản thân và sự nghiệp. </a><a> - Trang bị kỹ năng và phương pháp để rèn luyện tư duy mở, vượt qua mọi chướng ngại và chinh phục ước mơ. </a><a> 💡 Cuốn sách được chắt lọc từ những nghiên cứu trong và ngoài nước, cùng trải nghiệm thực tế của tác giả, là kim chỉ nam để bạn sống tự tin, khám phá bản thân và luôn vui vẻ trước mọi thử thách. </a><a>🔥 Nếu bạn muốn nắm bắt tương lai, hãy để 'Tư Duy Mở' dẫn lối!</a>",
          },
          /* Đám Trẻ Ở Đại Dương Đen*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lp24t90kapfycd.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134201-7qukw-leqn05hxqroz98.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134201-7qukw-leqn05ihpygj5a.webp",
            name: "Đám Trẻ Ở Đại Dương Đen",
            price: "99.000",
            code: "SPH02",
            category: "H",
            link: "https://s.shopee.vn/8zpN9JQ8ML",
            description:
              "<p>ĐÁM TRẺ Ở ĐẠI DƯƠNG ĐEN 🌊✨</p><a>Tác giả: Châu Sa Đáy Mắt</a><a>Thể loại: Tản văn</a><a>Kích thước: 13 x 19 cm 📏</a><a>Nhà xuất bản: NXB Thế giới 📚</a><a>Thương hiệu: AZ Việt Nam – Thương hiệu Wavebooks</a><a>Loại bìa: Bìa mềm 📖</a><a>Số trang: 280 trang 📝</a><a>Ngày phát hành: 01/04/2023 📅</a><p>GIỚI THIỆU SÁCH 🌟</p><a>'ĐÁM TRẺ Ở ĐẠI DƯƠNG ĐEN'</a><a>'nỗi buồn không rõ hình thù</a><a>ta cho nó dáng, ta thu vào lòng</a><a>ta ôm mà chẳng đề phòng</a><a>một ngày nó lớn chất chồng tâm can</a><a>kẻ sống muốn đời cạn</a><a>người chết muốn hồi sinh</a><a>trần gian bi hài nhỉ?</a><a>ta còn muốn bỏ mình?'</a><a>🌑 Đám trẻ ở đại dương đen là lời độc thoại và đối thoại của những đứa trẻ lạc lõng trong đại dương sâu thẳm của nỗi buồn và tuyệt vọng. Nơi đó, những con sóng cảm xúc không ngừng cuộn trào: lúc âm ỉ, khi dữ dội.</a><a>Những đứa trẻ ấy phải vật lộn với những góc tối tâm lý – từ tổn thương vì không được lớn lên trong gia đình toàn vẹn, đến những gánh nặng đè lên đôi vai non trẻ.</a><a>✨ Nhưng không chỉ dừng lại ở nỗi đau, đây còn là hành trình tự chữa lành đầy gian nan. Từng chút, từng chút, những đứa trẻ cố vươn mình khỏi bóng tối để tìm thấy ánh sáng. Những nỗ lực đó đã hóa thành câu từ chân thực, đau đớn nhưng đầy hy vọng trong cuốn sách này.</a><a>✍️ Cuốn sách được viết bởi Châu Sa Đáy Mắt, một tác giả thuộc GenZ, mong muốn cùng các bạn trẻ chia sẻ, bộc bạch và xoa dịu những xúc cảm chân thật về gia đình, xã hội và chính bản thân mình.</a><a>📖 ĐÁM TRẺ Ở ĐẠI DƯƠNG ĐEN – Một cuốn sách dành cho tâm hồn đang tìm kiếm sự vỗ về.</a><p>ĐIỂM NHẤN 📌</p><a>Thương hiệu sách trẻ: Phát hành bởi Wavebooks – thương hiệu dành riêng cho người trẻ Việt.</a><a>Thông điệp sâu sắc: Chạm tới những nỗi niềm sâu kín mà ai cũng có nhưng không dễ nói ra.</a><a>Hành trình chữa lành: Mang lại sự đồng cảm và động lực cho những ai đang lạc lối giữa đại dương cảm xúc của chính mình.</a><p>SẢN PHẨM DÀNH CHO AI?</p><a>👉 Những người trẻ đang tìm kiếm một cuốn sách đồng điệu với cảm xúc.</a><a>👉 Những ai muốn hiểu thêm về sự phức tạp trong tâm lý con người.</a><a>👉 Những người yêu thích tản văn và câu từ đầy chất thơ.</a><p>💡 Hãy để ĐÁM TRẺ Ở ĐẠI DƯƠNG ĐEN đồng hành cùng bạn trong hành trình tìm lại chính mình.</p>",
          },
          /* Đề Minh Hoạ THPT 2025*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3adhinp79k116.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3yg4bsipephe4.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m3kcgsovn1yt4b.webp",
            name: "Đề Minh Hoạ THPT 2025",
            price: "149.000",
            code: "SPH03",
            category: "H",
            link: "https://s.shopee.vn/50JIPs7vw9",
            description:
              "<p>SÁCH LUYỆN ĐỀ THPT QUỐC GIA 2025 – 50 ĐỀ MINH HỌA MOONBOOK 📘</p><p>🟢 ĐIỂM NỔI BẬT:</p><a>Định dạng mới nhất 2025: Theo hướng dẫn từ Bộ Giáo dục, bám sát cấu trúc đề thi minh họa.</a><a>Hệ thống câu hỏi đánh giá năng lực: Thiết kế dựa trên thực tiễn và khoa học, hỗ trợ học sinh phát triển tư duy.</a><a>Lời giải chi tiết & video hướng dẫn: 100% bài tập có lời giải chi tiết, kết hợp video minh họa và livestream hỗ trợ học sinh hiểu sâu từng dạng bài.</a><a>Phân bổ rõ ràng: Đề thi gồm các mức độ: Nhận biết, Thông hiểu, Vận dụng, Vận dụng cao.</a><p>🟢 NỘI DUNG CHI TIẾT:</p><a>Nhận biết & Thông hiểu: Các câu hỏi bám sát lý thuyết, có cài bẫy để rèn luyện sự cẩn thận, chính xác.</a><a>Vận dụng & Vận dụng cao: Các dạng bài HAY - LẠ - KHÓ, đòi hỏi tư duy đa chiều, xử lý sáng tạo.</a><p>🟢 ĐỐI TƯỢNG SỬ DỤNG:</p><a>Học sinh lớp 12: Chuẩn bị ôn thi tốt nghiệp THPT và kỳ thi đánh giá năng lực năm 2025.</a><a>Học sinh lớp 11: Muốn luyện đề sớm, làm quen cấu trúc đề thi.</a><a>Giáo viên: Tham khảo bộ đề thi thử chất lượng, làm tài liệu ôn luyện.</a><p>🟢 THÔNG TIN SÁCH:</p><a>Nhà xuất bản: Dân Trí.</a><a>Phát hành: Công ty CP Công nghệ Giáo dục trực tuyến Aladanh.</a><a>Tác giả:</a><a> - Toán: Lê Văn Tuấn, Đặng Việt Hùng, Nguyễn Thế Duy,...</a><a> - Tiếng Anh: Trang Anh, Đức Tài.</a><a> - Lý: Lại Đắc Hợp, Bùi Xuân Dương,...</a><a> - Hóa: Trần Công Minh, Lê Quỳnh Trang,...</a><a> - Sinh: TS Phan Khắc Nghệ, Thịnh Văn Nam,...</a><a> - Văn: Vũ Dung, Hà Thùy Linh,...</a><a> - Địa: Phương Dung, Quỳnh Hương.</a><a>Năm xuất bản: 2024.</a><a>Số trang: 3,145 trang, chia theo môn học:</a><a> - Toán: 288 trang.</a><a> - Lý: 314 trang.</a><a> - Hóa: 352 trang.</a><a> - Văn: 256 trang.</a><a> - Sử: 438 trang.</a><a> - Anh: 476 trang.</a><a> - Địa: 358 trang.</a><a> - Sinh: 328 trang.</a>",
          },
          /* Tổng Ôn THPT QG 2025*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1eznbe9groc3d.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lw59upkkhn1521.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lw59upkkluqh33.webp",
            name: "Tổng Ôn THPT QG 2025",
            price: "129.000",
            code: "SPH04",
            category: "H",
            link: "https://s.shopee.vn/AA1Oa905M8",
            description:
              "<p>BỘ SÁCH TỔNG ÔN LỚP 12 CHƯƠNG TRÌNH MỚI – ÔN THI THPT QUỐC GIA 2025 & ĐÁNH GIÁ NĂNG LỰC</p><p>🟢 ĐIỂM NỔI BẬT:</p><a>Hệ thống kiến thức toàn diện: Bám sát chương trình giáo dục phổ thông tổng thể, cập nhật từ các bộ sách giáo khoa mới: Cánh Diều, Kết nối tri thức, Chân trời sáng tạo.</a><a>Hỗ trợ đa dạng: Tích hợp lời giải chi tiết dạng text và video bài giảng theo mã ID, giúp học sinh nắm bắt kiến thức dễ dàng.</a><a>Đề thi sát thực tế: Các dạng bài tập và câu hỏi bám sát định dạng thi THPT Quốc gia 2025 và kỳ thi đánh giá năng lực.</a><a>Tài liệu toàn diện: Phù hợp với tất cả học sinh trên cả nước và các giáo viên ôn thi tham khảo.</a><p>🟢 NỘI DUNG SÁCH:</p><a>Hệ thống kiến thức: Được chắt lọc từ thực tiễn và yêu cầu của Bộ Giáo dục.</a><a>Phân loại bài tập: Từ cơ bản đến nâng cao, có lời giải và video hướng dẫn.</a><a>Đáp ứng mọi nhu cầu: Dành cho học sinh ôn thi tốt nghiệp, đánh giá năng lực và cả luyện thi đại học.</a><p>🟢 THÔNG TIN CHI TIẾT SÁCH THEO MÔN:</p><a>📊Tổng Ôn Toán Học Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: Thầy Lê Văn Tuấn.</a><a> - Số trang: 244 trang (Tập 1), 255 trang (Tập 2).</a><a> - Năm xuất bản: 2024.</a><a>🧬Tổng Ôn Sinh Học Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: TS Phan Khắc Nghệ, Thầy Nguyễn Văn Hoà.</a><a> - Số trang: 360 trang (Tập 1), 375 trang (Tập 2).</a><a> - Năm xuất bản: 2024.</a><a>💡Tổng Ôn Vật Lý Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: Thầy Lại Đắc Hợp.</a><a> - Số trang: 245 trang (Tập 1), 255 trang (Tập 2).</a><a> - Năm xuất bản: 2024.</a><a>🧪Tổng Ôn Hoá Học Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: Thầy Trần Công Minh, Cô Nguyễn Quỳnh Trang, Thầy Phạm Hùng Vương.</a><a> - Số trang: 326 trang (Tập 1 & Tập 2).</a><a> - Năm xuất bản: 2024.</a><a>📖Tổng Ôn Ngữ Văn Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: TS Vũ Dung, Cô Hà Linh.</a><a> - Số trang: 291 trang (Tập 1), 289 trang (Tập 2).</a><a> - Năm xuất bản: 2024.</a><a>🌍Tổng Ôn Địa Lý Lớp 12 (Tập 1 & 2):</a><a> - Nhà xuất bản: Dân Trí.</a><a> - Tác giả: Cô Phương Dung.</a><a> - Số trang: 191 trang (Tập 1), 190 trang (Tập 2).</a><a> - Năm xuất bản: 2024.</a>",
          },
          /* Văn Phòng & Đồ Chơi*/

          /* Xe & Phụ Kiện*/

          /* Linh Kiện & Mạch Điện*/

          /* Khác*/
        ],
        TIKTOK: [
          /*{
            imgSrc1: "Link SP1",
            imgSrc2: "Link SP2",
            imgSrc3: "Link SP3",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "",
          },*/
        ],
        OTISShop: [
          /*{
            imgSrc1: "Link SP1",
            imgSrc2: "Link SP2",
            imgSrc3: "Link SP3",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "",
          },*/
        ],
      };

      // Tạo HTML cho sản phẩm SHOPEE
      function generateShopeeHTML(product) {
        return `
                    <div class="product-column">
                      <div class="product-row2">
                        <img
                          src="${product.imgSrc1}"
                          alt="${product.name}"
                          onclick="toggleDescription('product-description-${
                            product.code
                          }')"
                        />
                        <div class="product-column2">
                          <div class="name">${product.name}</div>
                          <div class="price">Giá: ${product.price} VNĐ</div>
                          <div class="product-actions">
                            <button
                              class="save"
                              onclick="copyProductInfo('${product.code}','')"
                            >
                              ${product.code}
                            </button>
                            <img src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg" alt="SHOPEE"/>
                            <button
                              class="link"
                              onclick="window.open('${product.link}', '_blank')"
                            >
                              Liên Kết
                            </button>
                          </div>
                          <div class="styler">Click vào ảnh để xem mô tả!</div>
                        </div>
                      </div>
                      <div
                        class="product-description"
                        id="product-description-${product.code}"
                      >
                          <div class="description-img">
                            ${
                              product.imgSrc1
                                ? `<img style="height: 105px" src="${product.imgSrc1}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc2
                                ? `<img style="height: 105px" src="${product.imgSrc2}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc3
                                ? `<img style="height: 105px" src="${product.imgSrc3}"></img>`
                                : ""
                            }
                          </div>
                          <a
                            style="position: fixed;
                              text-align: center;
                              text-justify: auto;
                              color: white;
                              font-size: 18px;
                              right: 5px; top: -3px;"
                            onclick="toggleDescription('product-description-${
                              product.code
                            }')"
                          >
                            x
                          </a>
                          <div class="description-text">
                            <div style="width: auto;
                              margin: 2% 0 1% 0;
                              font-size: 15px;
                              font-weight: 600;
                              text-align: center;
                              text-justify: auto;
                            ">
                              <button
                                style="position: fixed; top: calc(17% + 4px); left:4px;"
                                class="save"
                                onclick="copyProductInfo('${product.code}','')"
                              >
                                ${product.code}
                              </button>
                                ${product.name}
                              <button
                                style="position: fixed; top: calc(17% + 4px); right:4px;"
                                class="link"
                                onclick="window.open('${
                                  product.link
                                }', '_blank')"
                              >
                                Liên Kết
                              </button>
                            </div>
                            <div style="overflow-y: auto; user-select: text;">${
                              product.description ||
                              "<p><i>Thông tin đang được cập nhật!</i></p>"
                            }
                            </div>
                          </div>
                      </div>
                    </div>
                    `;
      }

      // Tạo HTML cho sản phẩm TIKTOK
      function generateTiktokHTML(product) {
        return `
                    <div class="product-column">
                      <div class="product-row2">
                        <img
                          src="${product.imgSrc1}"
                          alt="${product.name}"
                          onclick="toggleDescription('product-description-${
                            product.code
                          }')"
                        />
                        <div class="product-column2">
                          <div class="name">${product.name}</div>
                          <div class="price">Giá: ${product.price} VNĐ</div>
                          <div class="product-actions">
                            <button
                              class="save"
                              onclick="copyProductInfo('${product.code}','')"
                            >
                              ${product.code}
                            </button>
                            <img src="https://i.pinimg.com/474x/05/8b/7c/058b7cd1e3a6d8e14d5b5906e84cb37a.jpg" alt="TIKTOK" />
                            <button
                              class="link"
                              onclick="window.open('${product.link}', '_blank')"
                            >
                              Liên Kết
                            </button>
                          </div>
                          <div class="styler">Click vào ảnh để xem mô tả!</div>
                        </div>
                      </div>
                      <div
                        class="product-description"
                        id="product-description-${product.code}"
                      >
                          <div class="description-img">
                            ${
                              product.imgSrc1
                                ? `<img style="height: 105px" src="${product.imgSrc1}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc2
                                ? `<img style="height: 105px" src="${product.imgSrc2}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc3
                                ? `<img style="height: 105px" src="${product.imgSrc3}"></img>`
                                : ""
                            }
                          </div>
                          <a
                            style="position: fixed;
                              text-align: center;
                              text-justify: auto;
                              color: white;
                              font-size: 18px;
                              right: 5px; top: -3px;"
                              onclick="toggleDescription('product-description-${
                                product.code
                              }')"
                          >
                            x
                          </a>
                          <div class="description-text">
                            <div style="width: auto;
                              margin: 2% 0 1% 0;
                              font-size: 15px;
                              font-weight: 600;
                              text-align: center;
                              text-justify: auto;
                            ">
                              <button
                                style="position: fixed; top: calc(17% + 4px); left:4px;"
                                class="save"
                                onclick="copyProductInfo('${product.code}','')"
                              >
                                ${product.code}
                              </button>
                                ${product.name}
                              <button
                                style="position: fixed; top: calc(17% + 4px); right:4px;"
                                class="link"
                                onclick="window.open('${
                                  product.link
                                }', '_blank')"
                              >
                                Liên Kết
                              </button>
                            </div>
                            <div style="overflow-y: auto; user-select: text;">${
                              product.description ||
                              "<p><i>Thông tin đang được cập nhật!</i></p>"
                            }
                            </div>
                          </div>
                      </div>
                    </div>
                    `;
      }

      // Tạo HTML cho sản phẩm OTISShop
      function generateOtisHTML(product) {
        return `
                    <div class="product-column">
                      <div class="product-row2">
                        <img
                          src="${product.imgSrc1}"
                          alt="${product.name}"
                          onclick="toggleDescription('product-description-${
                            product.code
                          }')"
                        />
                        <div class="product-column2">
                          <div class="name">${product.name}</div>
                          <div class="price">Giá: ${product.price} VNĐ</div>
                          <div class="product-actions">
                            <button
                              class="save"
                              onclick="copyProductInfo('${product.code}','')"
                            >
                              ${product.code}
                            </button>
                            <img src="https://i.pinimg.com/474x/ea/24/e1/ea24e1a0ed40857020ab39336b9fc78c.jpg" alt="OTISShop" />
                            <button
                              class="oder"
                              onclick="sendMessageWithClipboard('${
                                product.code
                              }')"
                            >
                              Mua Ngay
                            </button>
                          </div>
                          <div class="styler">Click vào ảnh để xem mô tả!</div>
                        </div>
                      </div>
                      <div
                        class="product-description"
                        id="product-description-${product.code}"
                      >
                          <div class="description-img">
                            ${
                              product.imgSrc1
                                ? `<img style="height: 105px" src="${product.imgSrc1}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc2
                                ? `<img style="height: 105px" src="${product.imgSrc2}"></img>`
                                : ""
                            }
                            ${
                              product.imgSrc3
                                ? `<img style="height: 105px" src="${product.imgSrc3}"></img>`
                                : ""
                            }
                          </div>
                          <a
                            style="position: fixed;
                              text-align: center;
                              text-justify: auto;
                              color: white;
                              font-size: 18px;
                              right: 5px; top: -3px;"
                            onclick="toggleDescription('product-description-${
                              product.code
                            }')"
                          >
                            x
                          </a>
                          <div class="description-text">
                            <div style="width: auto;
                              margin: 2% 0 1% 0;
                              font-size: 15px;
                              font-weight: 600;
                              text-align: center;
                              text-justify: auto;
                            ">
                              <button
                                style="position: fixed; top: calc(17% + 4px); left:4px;""
                                class="save"
                                onclick="copyProductInfo('${product.code}','')"
                              >
                                ${product.code}
                              </button>
                                ${product.name}
                              <button
                                style="position: fixed; top: calc(17% + 4px); right:4px;"
                                class="oder"
                                onclick="sendMessageWithClipboard('${
                                  product.code
                                }')"
                              >
                                Liên Kết
                              </button>
                            </div>
                            <div style="overflow-y: auto; user-select: text;">${
                              product.description ||
                              "<p><i>Thông tin đang được cập nhật!</i></p>"
                            }
                            </div>
                          </div>
                      </div>
                    </div>
                    `;
      }

      // Hàm toggle mô tả sản phẩm
      function toggleDescription(contentID) {
        var content = document.getElementById(contentID);

        if (content) {
          content.style.display =
            content.style.display === "block" ? "none" : "block";
        }
      }

      // Hàm tính số lượng sản phẩm sau khi lọc
      function countFilteredProducts(shop, category) {
        let count = 0;

        Object.keys(products).forEach((shopName) => {
          if (shop !== "all" && shop !== shopName) return;

          const filteredProducts = products[shopName].filter((product) => {
            return category === "all" || product.category === category;
          });

          count += filteredProducts.length;
        });

        return count;
      }

      function filterProducts() {
        const shop = document.getElementById("shop-select").value;
        const category = document.getElementById("category-select").value;

        // Xóa các sản phẩm cũ trước khi thêm sản phẩm mới
        document
          .querySelectorAll(".product-row")
          .forEach((row) => (row.innerHTML = ""));

        // Lọc và hiển thị sản phẩm cho từng shop
        Object.keys(products).forEach((shopName) => {
          if (shop !== "all" && shop !== shopName) return;

          const filteredProducts = products[shopName].filter((product) => {
            return category === "all" || product.category === category;
          });

          const productRow = document.querySelector(
            `.${shopName} .product-row`
          );

          filteredProducts.forEach((product) => {
            productRow.innerHTML +=
              shopName === "SHOPEE"
                ? generateShopeeHTML(product)
                : shopName === "OTISShop"
                ? generateOtisHTML(product)
                : generateTiktokHTML(product);
          });

          // Tính và hiển thị số lượng sản phẩm
          const count = countFilteredProducts(shop, category);
          const countElement = document.getElementById("product-count");
          if (countElement) {
            countElement.innerText = `${count}`;
          }
        });
      }

      // Gọi hàm lọc sản phẩm khi thay đổi điều kiện
      document
        .getElementById("shop-select")
        .addEventListener("change", filterProducts);
      document
        .getElementById("category-select")
        .addEventListener("change", filterProducts);

      // Thực hiện lần đầu khi trang được tải
      filterProducts();
    </script>
    <div
      class="icon-container"
      style="
        background-image: url('https://i.pinimg.com/736x/30/b1/9b/30b19b5deca9683e67a3960d44a6df83.jpg');
        background-repeat: repeat-x;
        background-size: auto 100%;
      "
    >
      <!-- Home -->
      <div class="icon" onclick="toggleContact('contact-Home')">
        <img
          src="https://i.pinimg.com/474x/8c/f6/3a/8cf63afd93dd860aa73efdcf609e7971.jpg"
          alt="Home"
        />
      </div>
      <!-- Nội dung Home-->
      <div class="contact-Home" id="contact-Home">
        <h3 style="text-align: center; width: 100%">
          OTISShop
          <button
            style="
              position: fixed;
              right: 7px;
              top: 7px;
              border-radius: 5px;
              border: none;
            "
            onclick="toggleContact('contact-Home')"
          >
            x
          </button>
        </h3>
        <p style="text-align: center; font-size: 13px">
          🍀 Theo dỗi <b>OTISShop</b> trên các nền tảng sau nhak! 🍀
        </p>
        <div class="header2">
          <!-- Icon Facebook -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('Facebook')"
          >
            <img
              src="https://i.pinimg.com/474x/c6/75/4f/c6754f858018877052f6b25bb2918b83.jpg"
              alt="Facebook"
            />
          </div>

          <!-- Icon Instagram -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('Instagram')"
          >
            <img
              src="https://i.pinimg.com/474x/f6/bc/ca/f6bccaf046f990955aa739ade2f390b9.jpg"
              alt="Instagram"
            />
          </div>

          <!-- Icon Hotline -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('Hotline')"
          >
            <img
              src="https://i.pinimg.com/474x/ba/6f/1d/ba6f1dcaebce3bef7a97cd4675c18cbf.jpg"
              alt="Hotline"
            />
          </div>

          <!-- Icon Messenger -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('Messenger')"
          >
            <img
              src="https://i.pinimg.com/474x/c1/77/92/c177924c4785314bb74dc5348567f253.jpg"
              alt="Messenger"
            />
          </div>

          <!-- Icon Threads -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('Threads')"
          >
            <img
              src="https://i.pinimg.com/474x/b4/e7/c2/b4e7c21b60917993b65259e40bab277e.jpg"
              alt="Threads"
            />
          </div>

          <!-- Icon TikTok -->
          <div
            class="icon"
            style="width: 35px; height: 35px"
            onclick="toggleContact('TikTok')"
          >
            <img
              src="https://i.pinimg.com/474x/05/8b/7c/058b7cd1e3a6d8e14d5b5906e84cb37a.jpg"
              alt="TikTok"
            />
          </div>
        </div>
        <p style="text-align: center">
          ❤️ OTISShop - Chân Thành Cảm Ơn Quý Khách! ❤️
        </p>
      </div>
      <!-- Nội dung StyleFacebook -->
      <div class="contact-Style" id="Facebook">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Chuyển đến trang Fanpage của OTISShop!
        </h3>
        <div class="div-style">
          <a href="https://www.facebook.com/OtisSeller" target="_blank">
            <button class="div-style2" style="background-color: #5ae73b">
              Có
            </button>
          </a>
          <button
            onclick="toggleContact('Facebook')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Nội dung StyleInstagram -->
      <div class="contact-Style" id="Instagram">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Chuyển đến trang Instagram của OTISShop!
        </h3>
        <div class="div-style">
          <a href="https://www.instagram.com/otisshopvn" target="_blank"
            ><button class="div-style2" style="background-color: #5ae73b">
              Có
            </button></a
          >
          <button
            onclick="toggleContact('Instagram')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Nội dung StyleHotline -->
      <div class="contact-Style" id="Hotline">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Bạn muốn liên hệ Hotline của OTISShop!
        </h3>
        <div class="div-style">
          <a href="tel:0329022431" target="_blank">
            <button class="div-style2" style="background-color: #5ae73b">
              Có
            </button>
          </a>
          <button
            onclick="toggleContact('Hotline')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Nội dung StyleMessenger -->
      <div class="contact-Style" id="Messenger">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Bạn muốn nhắn tin cho OTISShop!
        </h3>
        <div class="div-style">
          <a href="https://m.me/460099260527241?" target="_blank">
            <button class="div-style2" style="background-color: #5ae73b">
              Có
            </button>
          </a>
          <button
            onclick="toggleContact('Messenger')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Nội dung StyleThreads -->
      <div class="contact-Style" id="Threads">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Chuyển đến trang Threads của OTISShop!
        </h3>
        <div class="div-style">
          <a href="https://www.threads.net/@otisshopvn" target="_blank">
            <button class="div-style2" style="background-color: #5ae73b">
              Có
            </button>
          </a>
          <button
            onclick="toggleContact('Threads')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Nội dung StyleTikTok -->
      <div class="contact-Style" id="TikTok">
        <h3 style="text-align: center; margin-bottom: 5px; width: 100%">
          Chuyển đến trang TikTok của OTISShop!
        </h3>
        <div class="div-style">
          <a href="https://www.tiktok.com/@otisshop" target="_blank">
            <button class="div-style2" style="background-color: #5ae73b">
              Có
            </button>
          </a>
          <button
            onclick="toggleContact('TikTok')"
            class="div-style2"
            style="background-color: #ff4b4b"
          >
            Không
          </button>
        </div>
      </div>
      <!-- Logo để mở/ẩn phần Chatting -->
      <div class="icon" onclick="toggleContact('contact-Chatting')">
        <img
          src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
          alt="Chatting"
        />
      </div>
      <!-- Nội dung Chatting-->
      <div class="contact-Chatting" id="contact-Chatting">
        <h3 style="text-align: center; width: 100%">
          Chăm Sóc Khách Hàng!
          <button
            style="
              position: fixed;
              right: 7px;
              top: 7px;
              border-radius: 5px;
              border: none;
            "
            onclick="toggleContact('contact-Chatting')"
          >
            x
          </button>
          <button
            class="oder"
            style="position: fixed; left: 5px"
            onclick="sendMessageWithClipboard('')"
          >
            Tư Vấn
          </button>
        </h3>
        <p>
          <li>
            Để mua hàng bạn có thể Click vào nút <b>Liên Kết</b> để đặt hàng
            trực tiếp với Shopee hoặc liên hệ cho OTISShop để được hổ trợ!
          </li>
          <li>
            Shop chỉ tư vấn - <b>không</b> bán sản phẩm thuộc <b>Shopee</b>,
            <b>TikTok</b>! Vui lòng liên hệ <b>Shop bán hàng</b> bằng
            <b>Liên Kết</b> có trên sản phẩm!
          </li>
          <li>
            Bạn nhớ để lại
            <a
              href="https://forms.gle/B2Gk6Hsjm3EmbeR56"
              target="_blank"
              style="font-weight: 600"
              >Đánh Giá</a
            >
            giúp OTISShop nhak!
          </li>
        </p>
        <p style="text-align: center">
          ❤️ OTISShop - Chân Thành Cảm Ơn Quý Khách! ❤️
        </p>
      </div>
      <!-- Logo để mở/ẩn phần Hướng dẫn -->
      <div class="icon" onclick="toggleContact('contact-Content')">
        <img
          src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
          alt="Content"
        />
      </div>
      <!-- Nội dung Hướng dẫn -->
      <div class="contact-Content" id="contact-Content">
        <h3 style="text-align: center; width: 100%">
          Hướng Dẫn!
          <button
            style="
              position: fixed;
              right: 7px;
              top: 7px;
              border-radius: 5px;
              border: none;
            "
            onclick="toggleContact('contact-Content')"
          >
            x
          </button>
        </h3>
        <p>
          <li>
            Click vào mã sản phẩm (<b>SPA00</b>) để lưu, sau đó gửi mã sản phẩm
            khi
            <a
              href="https://www.messenger.com/t/460099260527241?"
              target="_blank"
              ><b>Liên Hệ</b></a
            >
            với OTISShop để được tư vấn!
          </li>
          <li>
            Để mua hàng bạn có thể Click vào nút <b>Liên Kết</b> để đặt hàng
            trực tiếp với Shopee hoặc liên hệ cho OTISShop để được hổ trợ!
          </li>
          <li>
            Shop chỉ tư vấn - <b>không</b> bán sản phẩm thuộc <b>Shopee</b>! Bạn
            có thể liên hệ <b>Shop bán hàng</b> bằng <b>Liên Kết</b> có trên sản
            phẩm!
          </li>
        </p>
        <p style="text-align: center">
          ❤️ OTISShop - Chân Thành Cảm Ơn Quý Khách! ❤️
        </p>
      </div>
    </div>

    <!-- SEO -->
    <div style="display: none">
      <h6>Mua laptop chơi game</h6>
      <h6>Máy tính bàn văn phòng</h6>
      <h6>Mua smartphone giá rẻ</h6>
      <h6>Mua smartphone cao cấp</h6>
      <h6>Mua máy tính bảng chính hãng</h6>
      <h6>Máy tính bảng Apple</h6>
      <h6>Mua ổ cứng SSD 1TB</h6>
      <h6>Tai nghe gaming</h6>
      <h6>Mua smartphone Samsung</h6>
      <h6>Smartwatch Xiaomi</h6>
      <h6>Mua máy ảnh Canon</h6>
      <h6>Mua máy chiếu giá rẻ</h6>
      <h6>Mua máy chiếu mini</h6>
      <h6>Mua loa bluetooth không dây</h6>
      <h6>Mua pin sạc dự phòng</h6>
      <h6>Mua bàn phím cơ</h6>
      <h6>Mua chuột gaming</h6>
      <h6>Tai nghe Sony</h6>
      <h6>Mua máy tính chơi game</h6>
      <h6>Mua laptop Asus</h6>
      <h6>Mua laptop Dell</h6>
      <h6>Mua laptop HP</h6>
      <h6>Mua webcam Logitech</h6>
      <h6>Mua microphone thu âm</h6>
      <h6>Mua máy tính xách tay văn phòng</h6>
      <h6>Mua card đồ họa Nvidia</h6>
      <h6>Mua ổ cứng gắn ngoài</h6>
      <h6>Mua camera an ninh</h6>
      <h6>Mua laptop Lenovo</h6>
      <h6>Mua màn hình máy tính</h6>
      <h6>Mua laptop gaming</h6>
      <h6>Mua router wifi tốc độ cao</h6>
      <h6>Mua máy phát điện</h6>
      <h6>Mua card âm thanh</h6>
      <h6>Mua điện thoại Apple</h6>
      <h6>Mua máy tính xách tay HP</h6>
      <h6>Mua máy quay phim</h6>
      <h6>Mua màn hình gaming</h6>
      <h6>Mua máy tính chơi game RTX</h6>
      <h6>Mua máy tính i7</h6>
      <h6>Mua laptop Macbook</h6>
      <h6>Mua máy tính Apple</h6>
      <h6>Mua laptop màn hình 15 inch</h6>
      <h6>Mua thiết bị mạng wifi mesh</h6>
      <h6>Mua game console PS5</h6>
      <h6>Mua loa JBL</h6>
      <h6>Mua loa Bose</h6>
      <h6>Mua phụ kiện máy tính</h6>
      <h6>Mua màn hình UltraWide</h6>
      <h6>Mua máy tính xách tay giá rẻ</h6>
      <h6>Mua ổ cứng 2TB</h6>
      <h6>Mua phần mềm diệt virus</h6>
      <h6>Mua chuột không dây</h6>
      <h6>Mua máy tính bảng Android</h6>
      <h6>Mua màn hình 4K</h6>
      <h6>Mua thiết bị lưu trữ NAS</h6>
      <h6>Mua máy tính mini</h6>
      <h6>Mua máy tính xách tay có webcam</h6>
      <h6>Mua laptop Acer</h6>
      <h6>Mua laptop Surface</h6>
      <h6>Mua máy tính chơi game cấu hình cao</h6>
      <h6>Mua hệ thống âm thanh surround</h6>
      <h6>Mua thiết bị mạng không dây</h6>
      <h6>Mua micro thu âm cao cấp</h6>
      <h6>Mua laptop chơi game giá rẻ</h6>
      <h6>Mua thiết bị đồ họa chuyên nghiệp</h6>
      <h6>Mua máy ảnh DSLR</h6>
      <h6>Mua laptop 13 inch</h6>
      <h6>Mua thiết bị gia dụng thông minh</h6>
      <h6>Mua laptop Lenovo giá rẻ</h6>
      <h6>Mua điện thoại Samsung Galaxy</h6>
      <h6>Mua điện thoại OPPO</h6>
      <h6>Mua máy tính bảng giá rẻ</h6>
      <h6>Mua camera hành trình</h6>
      <h6>Mua máy ảnh mirrorless</h6>
      <h6>Mua máy tính bảng giá tốt</h6>
      <h6>Mua máy tính có màn hình cảm ứng</h6>
      <h6>Mua thẻ nhớ SD</h6>
      <h6>Mua phụ kiện game console</h6>
      <h6>Mua hệ thống âm thanh</h6>
      <h6>Mua máy tính chơi game RTX 3060</h6>
      <h6>Mua điện thoại Android</h6>
      <h6>Mua tai nghe Over-Ear</h6>
      <h6>Mua máy tính màn hình 17 inch</h6>
      <h6>Mua máy tính chơi game với màn hình 144Hz</h6>
      <h6>Mua loa siêu trầm</h6>
      <h6>Mua bộ phát wifi</h6>
      <h6>Mua máy ảnh thể thao</h6>
      <h6>Mua phụ kiện laptop</h6>
      <h6>Mua thẻ nhớ USB</h6>
      <h6>Mua máy ảnh chuyên nghiệp</h6>
      <h6>Mua laptop màn hình 13 inch</h6>
      <h6>Mua quạt làm mát cho máy tính</h6>
      <h6>Mua điện thoại Huawei</h6>
      <h6>Mua máy tính chơi game AMD</h6>
      <h6>Mua hệ thống âm thanh karaoke</h6>
      <h6>Mua màn hình OLED</h6>
      <h6>Mua thiết bị gia đình thông minh</h6>
      <h6>Mua card đồ họa AMD</h6>
      <h6>Mua máy tính bảng Windows</h6>
      <h6>Mua bàn phím cơ RGB</h6>
      <h6>Mua bộ camera 360 độ</h6>
      <h6>Mua máy tính với vi xử lý Intel</h6>
      <h6>Mua máy tính xách tay với cấu hình cao</h6>
      <h6>Mua thiết bị VR</h6>
      <h6>Mua ghế sofa phòng khách</h6>
      <h6>Giường ngủ gỗ tự nhiên</h6>
      <h6>Bàn làm việc văn phòng</h6>
      <h6>Bàn ăn hiện đại</h6>
      <h6>Mua tủ quần áo 2 cánh</h6>
      <h6>Tủ bếp gỗ cao cấp</h6>
      <h6>Kệ TV bằng gỗ</h6>
      <h6>Mua kệ sách phòng khách</h6>
      <h6>Ghế làm việc văn phòng</h6>
      <h6>Bàn ăn gia đình 4 ghế</h6>
      <h6>Bàn làm việc cho phòng ngủ</h6>
      <h6>Tủ giày thông minh</h6>
      <h6>Giường ngủ bọc nệm</h6>
      <h6>Mua ghế ăn gia đình</h6>
      <h6>Mua tủ lạnh mini</h6>
      <h6>Mua bàn trang điểm cho phái đẹp</h6>
      <h6>Mua đèn trang trí phòng khách</h6>
      <h6>Mua bàn cafe cho phòng khách</h6>
      <h6>Mua kệ sách treo tường</h6>
      <h6>Mua tủ tivi hiện đại</h6>
      <h6>Mua ghế sofa da</h6>
      <h6>Tủ đựng quần áo lớn</h6>
      <h6>Mua đèn chùm phòng ăn</h6>
      <h6>Mua thảm trải sàn cho phòng khách</h6>
      <h6>Mua kệ tivi phòng ngủ</h6>
      <h6>Ghế bập bênh phòng khách</h6>
      <h6>Tủ trang trí đẹp</h6>
      <h6>Bàn làm việc cho học sinh</h6>
      <h6>Mua giường tầng cho trẻ em</h6>
      <h6>Bàn học sinh hiện đại</h6>
      <h6>Mua bàn ăn bằng đá mặt kính</h6>
      <h6>Mua kệ trang trí phòng khách</h6>
      <h6>Mua ghế dài ngoài trời</h6>
      <h6>Bàn làm việc gỗ tự nhiên</h6>
      <h6>Mua ghế massage</h6>
      <h6>Tủ lạnh side by side</h6>
      <h6>Mua giường ngủ có ngăn kéo</h6>
      <h6>Mua ghế ngồi văn phòng</h6>
      <h6>Mua tủ quần áo cửa lùa</h6>
      <h6>Tủ bếp inox cao cấp</h6>
      <h6>Bàn trang điểm gỗ tự nhiên</h6>
      <h6>Bàn học sinh thông minh</h6>
      <h6>Mua tủ lạnh Inverter</h6>
      <h6>Mua ghế thư giãn phòng ngủ</h6>
      <h6>Mua bộ bàn ghế ăn 6 ghế</h6>
      <h6>Mua tủ đựng đồ gọn gàng</h6>
      <h6>Mua bộ sofa góc</h6>
      <h6>Mua giường ngủ có hộc kéo</h6>
      <h6>Ghế lười phòng khách</h6>
      <h6>Tủ đựng giày dép thông minh</h6>
      <h6>Bàn làm việc cho không gian nhỏ</h6>
      <h6>Mua tủ kệ phòng ngủ</h6>
      <h6>Mua ghế ngoài trời cao cấp</h6>
      <h6>Mua sofa góc L</h6>
      <h6>Mua bàn làm việc chân sắt</h6>
      <h6>Mua tủ sách cho phòng làm việc</h6>
      <h6>Ghế thư giãn ngoài trời</h6>
      <h6>Mua bàn học sinh nhỏ gọn</h6>
      <h6>Mua kệ sách đa năng</h6>
      <h6>Mua tủ giày thông minh kéo</h6>
    </div>

    <!-- ĐÁNH GIÁ -->
    <div
      id="fixed-element"
      style="
        position: fixed;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        right: 15px;
        bottom: 80px;
        width: auto;
        height: auto;
        border-radius: 5px;
        background-color: rgba(255, 255, 255, 0.888);
        transform: scale(1); /* Kích thước ban đầu */
        transition: transform 3s ease;
      "
    >
      <div
        style="
          display: flex;
          flex-direction: row;
          justify-content: center;
          align-items: center;
          margin-top: 2px;
        "
      >
        <a
          href="https://forms.gle/B2Gk6Hsjm3EmbeR56"
          target="_blank"
          style="
            font-weight: 600;
            color: rgb(24, 19, 156);
            margin: 0px 5px 3px 5px;
            font-size: 16px;
            text-align: center;
            text-justify: center;
          "
        >
          Đánh Giá!
        </a>
        <div
          onclick="toggleContact('fixed-element')"
          style="
            position: fixed;
            right: 2px;
            top: 2px;
            font-weight: 450;
            border: none;
            width: 15px;
            height: 20px;
            font-size: 14px;
            text-align: center;
            text-justify: center;
          "
        >
          x
        </div>
      </div>
      <a
        style="
          background-color: #c6c6c687;
          border-radius: 5px;
          display: flex;
          height: 24px;
          font-size: 16px;
          margin: 0 5px 5px 5px;
          text-align: center;
          text-justify: center;
        "
      >
        ⭐️ ⭐️ ⭐️ ⭐️ ⭐️
      </a>
    </div>
    <script>
      document.addEventListener("DOMContentLoaded", () => {
        const element = document.getElementById("fixed-element");
        let isHidden = false; // Trạng thái ban đầu: phần tử đang hiển thị

        setInterval(() => {
          // Thay đổi trạng thái phóng to hoặc thu nhỏ
          isHidden = !isHidden; // Đảo trạng thái

          element.style.transform = isHidden ? "scale(1.2)" : "scale(1)"; // Phóng to khi hiện, thu nhỏ khi ẩn
        }, 750);
      });

      document.addEventListener("DOMContentLoaded", () => {
        // Đọc danh sách mã từ clipboard khi trang được tải
        readClipboardForProducts();
      });

      // Biến toàn cục để lưu các mã sản phẩm đã được chọn
      let selectedProductCodes = [];

      // Hàm đọc nội dung từ clipboard và lấy các mã sản phẩm
      async function readClipboardForProducts() {
        try {
          const clipboardText = await navigator.clipboard.readText();
          const codePattern = /(SP|TT|OS)[A-Z]{1}\d{2}[; |. ]/g;

          const matches = clipboardText.match(codePattern);

          if (matches && matches.length > 0) {
            matches.forEach((match) => {
              const code = match.replace(";", " ").trim();
              copyProductInfo(code, "DK");
            });

            if (matches.length > 0) {
              alert(`Có ${matches.length} mã sản phẩm hợp lệ.`);
            }
          } else {
            alert("Không tìm thấy mã sản phẩm nào.");
          }
        } catch (err) {
          console.error("Không thể đọc dữ liệu sản phẩm từ Clipboard: ", err);
          alert("Vui lòng cấp quyền truy cập Clipboard.");
        }
      }

      // Hàm để sao chép mã sản phẩm vào danh sách đã chọn
      function copyProductInfo(name, DK) {
        // Kiểm tra xem mã sản phẩm đã tồn tại trong danh sách chưa
        if (selectedProductCodes.includes(name)) {
          alert("Mã sản phẩm đã tồn tại!");
        } else {
          // Thêm mã sản phẩm vào danh sách đã chọn
          selectedProductCodes.push(name);

          // Chỉ hiển thị thông báo lưu sản phẩm khi người dùng thực sự thêm nó
          if (!DK.trim()) {
            alert("Lưu sản phẩm thành công!");
          }
          updateClipboard(); // Cập nhật clipboard ngay sau khi thêm
        }
      }

      // Cập nhật clipboard với danh sách mã sản phẩm mới
      function updateClipboard() {
        const newText = `${selectedProductCodes.join("; ")};`;
        navigator.clipboard.writeText(newText).then(
          function () {
            console.log("Đã cập nhật mã sản phẩm thành công.");
          },
          function (err) {
            console.error("Không thể cập nhật mã sản phẩm: ", err);
            alert("Không thể thêm mã sản phẩm. Vui lòng thử lại.");
          }
        );
      }

      // Hàm gửi tin nhắn với nội dung từ biến `ID` và `selectedProductCodes`
      function sendMessageWithClipboard(ID) {
        try {
          // Kiểm tra nếu không có ID hợp lệ và danh sách mã sản phẩm trống
          if (!ID.trim() && selectedProductCodes.length === 0) {
            alert("Vui lòng lưu mã sản phẩm trước!");
            return;
          }

          // Soạn nội dung tin nhắn
          const message = ID.trim()
            ? `Tôi muốn biết thông tin về sản phẩm sau: ${ID}.`
            : `Tôi muốn biết thông tin về các sản phẩm sau: ${selectedProductCodes.join(
                "; "
              )}.`;

          // Tạo URL Messenger với nội dung tin nhắn
          const url1 = `https://m.me/460099260527241?text=${encodeURIComponent(
            message
          )}`;
          const url2 = `https://www.messenger.com/t/460099260527241?text=${encodeURIComponent(
            message
          )}`;

          // Kiểm tra môi trường di động
          if (/Mobi|Android/i.test(navigator.userAgent)) {
            // Trên di động, sử dụng m.me thay vì messenger.com để mở trực tiếp ứng dụng Messenger
            window.location.href = url1; // Dùng window.location.href để mở ứng dụng Messenger trên di động
          } else {
            // Nếu không phải thiết bị di động, mở trong tab mới
            window.open(url2, "_blank");
          }
        } catch (err) {
          console.error("Không thể gửi tin nhắn: ", err);
          alert("Đã xảy ra lỗi khi gửi tin nhắn. Vui lòng thử lại.");
        }
      }

      // Hàm để chuyển đổi hiển thị của các phần nội dung liên lạc
      function toggleContact(contentID) {
        var content = document.getElementById(contentID);
        var content1 = document.getElementById("contact-Content");
        var content2 = document.getElementById("contact-Chatting");
        var content3 = document.getElementById("contact-Home");
        var content4 = document.getElementById("Facebook");
        var content5 = document.getElementById("Instagram");
        var content6 = document.getElementById("Hotline");
        var content7 = document.getElementById("Messenger");
        var content8 = document.getElementById("Threads");
        var content9 = document.getElementById("TikTok");

        // Ẩn tất cả các phần tử khác trước khi hiển thị phần tử mới
        if (contentID === "contact-Content") {
          content2.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
          content6.style.display = "none";
          content7.style.display = "none";
          content8.style.display = "none";
          content9.style.display = "none";
        }
        if (contentID === "contact-Chatting") {
          content1.style.display = "none";
          content3.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
          content6.style.display = "none";
          content7.style.display = "none";
          content8.style.display = "none";
          content9.style.display = "none";
        }
        if (contentID === "contact-Home") {
          content1.style.display = "none";
          content2.style.display = "none";
          content4.style.display = "none";
          content5.style.display = "none";
          content6.style.display = "none";
          content7.style.display = "none";
          content8.style.display = "none";
          content9.style.display = "none";
        }

        // Chuyển đổi trạng thái hiển thị của phần tử được chọn
        if (content.style.display !== "block") {
          content.style.display = "block";
        } else {
          content.style.display = "none";
        }
      }
      // HÀM 4 MÙA
      const effectContainer = document.getElementById("effect-container");
      // Xác định mùa hiện tại
      const month = new Date().getMonth() + 1;

      let asset;
      if (month >= 1 && month <= 3) {
        // Mùa Xuân: Hoa rơi
        asset = "🌸";
      } else if (month >= 4 && month <= 6) {
        // Mùa Hè: Ánh sáng mặt trời
        asset = "☀️";
      } else if (month >= 7 && month <= 9) {
        // Mùa Thu: Lá vàng rơi
        asset = "🍁";
      } else {
        // Mùa Đông: Bông tuyết
        asset = "❄️";
      }

      // Hàm tạo hiệu ứng động
      function createEffect() {
        const effect = document.createElement("div");
        effect.classList.add("effect");

        const size = Math.random() * 10 + 5; // Kích thước ngẫu nhiên
        const positionX = Math.random() * window.innerWidth; // Vị trí X ngẫu nhiên
        const delay = Math.random() * 5; // Độ trễ ngẫu nhiên
        const duration = Math.random() * 5 + 10; // Thời gian rơi ngẫu nhiên

        effect.style.fontSize = `${size}px`; // Cỡ chữ emoji
        effect.style.left = `${positionX}px`;
        effect.style.animationDelay = `${delay}s`;
        effect.style.animationDuration = `${duration}s`;
        effect.textContent = asset; // Emoji hiện tại (🌸, ☀️, 🍁, ❄️)

        effectContainer.appendChild(effect);

        // Xóa hiệu ứng khi rơi xong
        setTimeout(() => {
          effect.remove();
        }, (duration + delay) * 2500);
      }

      // Tạo hiệu ứng liên tục
      setInterval(createEffect, 1000);
    </script>
  </body>
</html>
