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

        width: 100%;

        /* Loại bỏ khoảng cách mặc định của body */
        margin: 22.5px auto 30px auto; /* Căn giữa body theo chiều ngang trong viewport */
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
        gap: 15px; /* Phân bố đều khoảng cách giữa các phần tử */
        height: auto; /* Chiều cao của container */
      }

      /* Ảnh logo */
      .header img {
        width: 90px;
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
        gap: 5px;
        padding: 2px;
        width: auto;
        height: auto;
      }
      /* Phần hiển thị sản phẩm dọc */
      .SHOPEE,
      .TIKTOK,
      .OTISShop {
        display: flex;
        width: 380px;
        flex-direction: column; /* Sắp xếp các phần tử con theo chiều dọc */
        align-items: center; /* Căn giữa các phần tử con theo chiều ngang */
        justify-content: center; /* Căn các phần tử con theo chiều dọc (mặc định là từ trên xuống) */
      }
      .product-row {
        width: 380px; /* Chiều rộng tối đa */
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: auto;
        gap: 5px;
        padding: 2.5px 0;
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
        gap: 5px;
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
        gap: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
        border: 1px solid black;
      }
      /* Phần sản phẩm */
      .product-column2 {
        width: 240px;
        height: 120px;
        display: flex;
        margin: 5px 5px 5px 0;
        background-color: #f5f5f5a5;
        flex-direction: column;
        align-items: auto;
        border: 1px solid black;
        border-radius: 5px;
        justify-content: center; /* Căn giữa các phần tử theo chiều ngang */
        align-items: center; /* Căn giữa các phần tử theo chiều dọc (nếu cần) */
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
      }
      /* Ảnh sản phẩm */
      .product-row2 img {
        width: 120px;
        height: 120px;
        margin: 5px 0 5px 5px;
        object-fit: cover;
        border-radius: 5px;
        border: 1px solid black;
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
        max-width: 450px;
        height: 100%;
        color: #000;
        background-color: #616161cd;
        z-index: 999;
      }
      .description-content {
        height: calc(98% + 6px);
        margin: 1%;
        gap: 1%;
        display: flex;
        flex-direction: column;
        border: 1px solid rgb(255, 255, 255);
        justify-items: center;
        align-items: center;
      }
      .description-img {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        width: calc(98%);
        height: 20%;
        gap: 10px;
      }
      .description-text {
        position: fixed;
        display: flex;
        flex-direction: column;
        text-align: left;
        bottom: calc(2% - 8px);
        width: calc(96% - 2px);
        height: calc(78% + 4px);
        background-color: #ffffffe3;
        border-radius: 3px;
      }

      .description-text p {
        margin: 1% 0 1% 2%;
        width: 98%;
        font-size: 13px;
        font-weight: 500;
      }
      .description-text a {
        margin: 0.5% 0 0 4%;
        width: 96%;
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
        font-size: 14px;
        font-weight: 600;
      }
      /* Giá */
      .product-column .price {
        color: #d81414;
        margin: 2.5px;
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
        margin: 3px;
      }
      .oder,
      .save,
      .link {
        margin: 2.5px;
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
    </style>
  </head>

  <body>
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
              margin: 2px 2px;
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
                margin: 0 0 0 3px;
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
              <a style="font-size: 13px"> 07:30 - 03.12.2024</a>
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
          /* Nước Hoa - BODYMISS*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llszfjzmt8f304.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llszfjzmt8f304.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-llszfjzmt8f304.webp",
            name: "Nước Hoa - BODYMISS",
            price: "55.800",
            code: "SPB101",
            category: "B",
            link: "https://s.shopee.vn/8pUdQpfLsu",
            description: "<p>Mô tả</p><a>Cách dùng</a><a>Bảo hành</a>",
          },
          /* Sữa tắm gội 3 in 1*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2172u9swogu94.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2172u9swogu94.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2172u9swogu94.webp",
            name: "Sữa tắm gội 3 in 1",
            price: "169.000",
            code: "SPG102",
            category: "G",
            link: "https://s.shopee.vn/8AEwdf7DK3",
            description: "",
          },
          /* Quạt mini có LED*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lua61kdx7m6pd9.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lua61kdx7m6pd9.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lua61kdx7m6pd9.webp",
            name: "Quạt mini có LED",
            price: "329.000",
            code: "SPC103",
            category: "C",
            link: "https://s.shopee.vn/5VEBSmY4yy",
            description: "",
          },
          /* Đồng Hồ Thông Minh*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/75daf60465e1496e7a0bbcb87636a5d1.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/75daf60465e1496e7a0bbcb87636a5d1.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/75daf60465e1496e7a0bbcb87636a5d1.webp",
            name: "Đồng Hồ Thông Minh",
            price: "56.000",
            code: "SPC104",
            category: "C",
            link: "https://s.shopee.vn/1LOcV91DZv",
            description: "",
          },
          /* Sạc dự phòng 20W*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-luk3f0wjjeam41.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-luk3f0wjjeam41.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/cn-11134207-7r98o-luk3f0wjjeam41.webp",
            name: "Sạc dự phòng 20W",
            price: "321.000",
            code: "SPC105",
            category: "C",
            link: "https://s.shopee.vn/5AbL4DGshp",
            description: "",
          },
          /* Điện Thoại Vivo V23 5G*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1nvez3metsjbc.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1nvez3metsjbc.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m1nvez3metsjbc.webp",
            name: "Điện Thoại Vivo V23 5G",
            price: "1.993.950",
            code: "SPC106",
            category: "C",
            link: "https://s.shopee.vn/9zgap9wWPX",
            description: "",
          },
          /* Áo Len Nam Nữ*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lpew02e1r2vvf4.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lpew02e1r2vvf4.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-lpew02e1r2vvf4.webp",
            name: "Áo Len Nam Nữ",
            price: "139.000",
            code: "SPA107",
            category: "A",
            link: "https://s.shopee.vn/3AqGgcvk3y",
            description: "",
          },
          /* Quần jean nam*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m39gtktdm4gx09.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m39gtktdm4gx09.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m39gtktdm4gx09.webp",
            name: "Quần jean nam",
            price: "139.000",
            code: "SPA108",
            category: "A",
            link: "https://s.shopee.vn/30WqUJwNOx",
            description: "",
          },
          /* Áo sơ mi trắng nam*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-ltm7exxdmnm527.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-ltm7exxdmnm527.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7r98o-ltm7exxdmnm527.webp",
            name: "Áo sơ mi trắng nam",
            price: "155.100",
            code: "SPA109",
            category: "A",
            link: "https://s.shopee.vn/4pyUfgpOgK",
            description: "",
          },
          /* Quần Jean BIGSIZE*/ {
            imgSrc1:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2m8kpfbnrie79@resize_w450_nl.webp",
            imgSrc2:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2m8kpfbnrie79@resize_w450_nl.webp",
            imgSrc3:
              "https://down-vn.img.susercontent.com/file/vn-11134207-7ras8-m2m8kpfbnrie79@resize_w450_nl.webp",
            name: "Quần Jean BIGSIZE",
            price: "150.000",
            code: "SPA110",
            category: "A",
            link: "https://s.shopee.vn/4ff4TNq21J",
            description: "",
          },
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
              onclick="toggleDescription('product-description-${product.code}')"
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
            <div class="description-content">
              <div class="description-img">
                ${
                  product.imgSrc1
                    ? `<img style="height: 115px" src="${product.imgSrc1}"></img>`
                    : ""
                }
                ${
                  product.imgSrc2
                    ? `<img style="height: 115px" src="${product.imgSrc2}"></img>`
                    : ""
                }
                ${
                  product.imgSrc3
                    ? `<img style="height: 115px" src="${product.imgSrc3}"></img>`
                    : ""
                }
              </div>
              <a
                style="position: fixed;
                  text-align: center;
                  text-justify: auto;
                  color: white;
                  font-size: 18px;
                  right: 14px; top: 2px;"
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
                    style="position: fixed; top: calc(20% + 6px); left: calc(2% + 4px);""
                    class="save"
                    onclick="copyProductInfo('${product.code}','')"
                  >
                    ${product.code}
                  </button>
                    ${product.name}
                  <button
                    style="position: fixed; top: calc(20% + 6px); right: calc(2% + 4px);"
                    class="link"
                    onclick="window.open('${product.link}', '_blank')"
                  >
                    Liên Kết
                  </button>
                </div>
                <div style="overflow-y: auto;">${
                  product.description ||
                  "<p><i>Thông tin đang được cập nhật!</i></p>"
                }
                </div>
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
              onclick="toggleDescription('product-description-${product.code}')"
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
            <div class="description-content">
              <div class="description-img">
                ${
                  product.imgSrc1
                    ? `<img style="height: 115px" src="${product.imgSrc1}"></img>`
                    : ""
                }
                ${
                  product.imgSrc2
                    ? `<img style="height: 115px" src="${product.imgSrc2}"></img>`
                    : ""
                }
                ${
                  product.imgSrc3
                    ? `<img style="height: 115px" src="${product.imgSrc3}"></img>`
                    : ""
                }
              </div>
              <a
                style="position: fixed;
                  text-align: center;
                  text-justify: auto;
                  color: white;
                  font-size: 18px;
                  right: 14px; top: 2px;"
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
                    style="position: fixed; top: calc(20% + 6px); left: calc(2% + 4px);""
                    class="save"
                    onclick="copyProductInfo('${product.code}','')"
                  >
                    ${product.code}
                  </button>
                    ${product.name}
                  <button
                    style="position: fixed; top: calc(20% + 6px); right: calc(2% + 4px);"
                    class="link"
                    onclick="window.open('${product.link}', '_blank')"
                  >
                    Liên Kết
                  </button>
                </div>
                <div style="overflow-y: auto;">${
                  product.description ||
                  "<p><i>Thông tin đang được cập nhật!</i></p>"
                }
                </div>
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
              onclick="toggleDescription('product-description-${product.code}')"
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
                  onclick="sendMessageWithClipboard('${product.code}')"
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
            <div class="description-content">
              <div class="description-img">
                ${
                  product.imgSrc1
                    ? `<img style="height: 115px" src="${product.imgSrc1}"></img>`
                    : ""
                }
                ${
                  product.imgSrc2
                    ? `<img style="height: 115px" src="${product.imgSrc2}"></img>`
                    : ""
                }
                ${
                  product.imgSrc3
                    ? `<img style="height: 115px" src="${product.imgSrc3}"></img>`
                    : ""
                }
              </div>weight: 24px; height: 24px;
              <a
                style="position: fixed;
                  text-align: center;
                  text-justify: auto;
                  color: white;
                  font-size: 18px;
                  right: 14px; top: 2px;"
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
                    style="position: fixed; top: calc(20% + 6px); left: calc(2% + 4px);""
                    class="save"
                    onclick="copyProductInfo('${product.code}','')"
                  >
                    ${product.code}
                  </button>
                    ${product.name}
                  <button
                    style="position: fixed; top: calc(20% + 6px); right: calc(2% + 4px);"
                    class="oder"
                    onclick="sendMessageWithClipboard('${product.code}')"
                  >
                    Liên Kết
                  </button>
                </div>
                <div style="overflow-y: auto;">${
                  product.description ||
                  "<p><i>Thông tin đang được cập nhật!</i></p>"
                }
                </div>
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
      <div
        class="icon"
        style="width: 42px; height: 42px"
        onclick="toggleContact('contact-Home')"
      >
        <img
          src="https://i.pinimg.com/474x/8c/f6/3a/8cf63afd93dd860aa73efdcf609e7971.jpg"
          alt="Home"
        />
      </div>
      <!-- Nội dung Home-->
      <div class="contact-Home" id="contact-Home">
        <h3 style="text-align: center">
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
        <h3 style="text-align: center; margin-bottom: 5px">
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
        <h3 style="text-align: center; margin-bottom: 5px">
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
        <h3 style="text-align: center; margin-bottom: 5px">
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
        <h3 style="text-align: center; margin-bottom: 5px">
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
        <h3 style="text-align: center">
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
        <h3 style="text-align: center">
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
      <div
        class="icon"
        style="width: 50px; height: 50px"
        onclick="toggleContact('contact-Chatting')"
      >
        <img
          src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
          alt="Chatting"
        />
      </div>
      <!-- Nội dung Chatting-->
      <div class="contact-Chatting" id="contact-Chatting">
        <h3 style="text-align: center; margin-bottom: 5px">
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
            Để đặt hàng vui lòng lưu mã sản phẩm sau đó chọn
            <a
              href="https://www.messenger.com/t/460099260527241?"
              target="_blank"
              ><b>Tư Vấn</b></a
            >
            để gửi thông tin quan Fanpage của <b>OTISShop</b>!
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
      <div
        class="icon"
        style="width: 42px; height: 42px"
        onclick="toggleContact('contact-Content')"
      >
        <img
          src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
          alt="Content"
        />
      </div>
      <!-- Nội dung Hướng dẫn -->
      <div class="contact-Content" id="contact-Content">
        <h3 style="text-align: center">
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
            Click vào mã sản phẩm (<b>SP-A000</b>) để lưu, sau đó gửi mã sản
            phẩm khi
            <a
              href="https://www.messenger.com/t/460099260527241?"
              target="_blank"
              ><b>Liên Hệ</b></a
            >
            với chúng tôi qua Fanpage của OTISShop!
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
          const codePattern = /(SP|TT|OS)[A-Z]{1}\d{3}[; |. ]/g;

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
    </script>
  </body>
</html>
