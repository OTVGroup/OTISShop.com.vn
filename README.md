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
        /* Giới hạn chiều rộng của body */
        max-width: 100%;
        width: 380px; /* Cố định chiều rộng */

        /* Loại bỏ khoảng cách mặc định của body */
        margin: 35px auto 35px auto; /* Căn giữa body theo chiều ngang trong viewport */
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
        width: 100px;
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
        justify-items: center;
        text-align: left;
        background-color: #63e2ffb1;
        border-radius: 7px;
        gap: 5px;
        padding: 3px;
        width: auto;
        height: auto;
      }
      /* Phần hiển thị sản phẩm dọc */
      .SHOPEE,
      .TIKTOK,
      .OTISShop {
        display: flex;
        width: 350px;
        flex-direction: column; /* Sắp xếp các phần tử con theo chiều dọc */
        align-items: center; /* Căn giữa các phần tử con theo chiều ngang */
        justify-content: center; /* Căn các phần tử con theo chiều dọc (mặc định là từ trên xuống) */
      }
      .product-row {
        width: 100%; /* Chiều rộng tối đa */
        display: grid;
        flex-direction: row;
        justify-content: center;
        align-items: auto;
        gap: 5px;
        padding: 5px;
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
        padding: 5px;
        gap: 5px;
        text-align: center;
        box-sizing: border-box;
        flex: 0 0 auto; /* Đảm bảo phần tử không bị co giãn */
        border: 1px solid black;
      }
      /* Phần sản phẩm */
      .product-column2 {
        width: 240px;
        height: 110px;
        display: flex;
        background-color: #ffffffb1;
        flex-direction: column;
        align-items: auto;
        padding: 5px;
        border-radius: 5px;
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
        border-radius: 5px;
      }
      .product-description {
        margin-top: 0 1% 1% 1%;
        display: flex;
        flex-direction: column;
        padding: 5px;
        align-items: center;
        width: 345px;
        color: #000;
        background-color: #ffffffb1;
        border-radius: 5px;
      }
      .description-text {
        display: none;
        text-align: left;
        padding: 2.5px;
        width: 340px;
        background-color: #f9f9f9;
        border: 1px solid #ddd;
        border-radius: 3px;
        font-size: 12px;
      }
      .product-description a,
      .product-column .name {
        color: #000000;
        margin: 2.5px;
        font-size: 14px;
        font-weight: 600;
      }
      /* Giá */
      .product-column .price {
        color: #d30808;
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
        border: 1.5px solid #000000;
        border-radius: 50%;
        margin: 3px;
      }
      .OUT,
      .oder,
      .save,
      .link {
        margin: 2.5px;
        width: auto;
        height: 24px;
        font-size: 11px; /* Kích thước chữ */
        font-weight: 550; /* Độ đậm của chữ */
        text-align: center; /* Căn giữa chữ theo chiều ngang */
        justify-content: center; /* Căn giữa ngang */
        align-items: center; /* Căn giữa dọc */
        border: 1px solid #000000;
        color: rgb(0, 0, 0); /* Màu chữ */
        border-radius: 5px;
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
        gap: 10px; /* Phân bố đều khoảng cách giữa các phần tử */
        height: auto; /* Chiều cao của container (thay đổi tuỳ theo số lượng và kích thước các phần tử) */
      }
      /* Các phần tử icon */
      .icon {
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: transform 0.5s ease, box-shadow 0.5s ease;
        border: 1px solid black;
      }
      .icon:active {
        transform: scale(1.2); /* Phóng to */
        box-shadow: 0 0 10px #000000;
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
      .contact-Shopping,
      .contact-Chatting {
        position: fixed;
        background-color: #ffffff;
        border-radius: 10px;
        padding: 10px;
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
      .contact-Chatting,
      .contact-Shopping {
        display: none;
      }
      /* Hiện ban đầu */
      .contact-Content {
        display: block;
      }
      .contact-Content h3,
      .contact-Shopping h3,
      .contact-Chatting h3 {
        margin: 0;
        font-size: 16px;
        color: #000000;
        text-align: left;
        font-weight: 750;
      }
      .contact-Content p,
      .contact-Shopping p,
      .contact-Chatting p {
        margin: 2.5px 0;
        font-size: 12px;
        color: #000000;
        text-align: left;
        font-weight: 450;
      }
      .contact-Content li,
      .contact-Shopping li,
      .contact-Chatting li {
        margin: 2.5px 0;
        font-size: 12px;
        color: #000000;
        text-align: left;
        font-weight: 400;
      }
    </style>
  </head>

  <body>
    <!-- Phần logo -->
    <div class="header">
      <img
        src="https://i.pinimg.com/474x/ea/24/e1/ea24e1a0ed40857020ab39336b9fc78c.jpg"
        alt="Logo OTISShop"
      />
      <!-- Thanh điều kiện (Filter) -->
      <div
        style="
          max-width: 280px;
          max-height: 70px;
          padding: 3px;
          display: grid;
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
              justify-content: center;
              align-items: center;
              gap: 5px;
              margin: 2px 0;
            "
          >
            <div>
              <label for="shop-select" style="font-size: 14px"
                ><b style="width: 50px">Shop: </b></label
              >
              <select
                id="shop-select"
                style="font-size: 13px; border-radius: 3px; width: 100px"
              >
                <option value="all">Tất cả</option>
                <option value="SHOPEE">Shopee</option>
                <option value="TIKTOK">TikTok</option>
                <option value="OTISShop">OTISShop</option>
              </select>
            </div>

            <b
              style="
                font-size: 14px;
                display: flex;
                align-items: center;
                justify-content: center;
                width: 40px;
                margin: 0 0 0 3px;
              "
            >
              Còn:
            </b>

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

          <div
            style="
              height: auto;
              display: flex;
              align-items: flex-start;
              gap: 10px;
              margin: 2px 0;
            "
          >
            <label for="category-select" style="font-size: 14px"
              ><b>Loại: </b></label
            >
            <select
              id="category-select"
              style="font-size: 13px; border-radius: 3px; width: 190px"
            >
              <option value="all">Tất cả</option>
              <option value="AO">Thời Trang</option>
              <option value="BO">Sức Khỏe & Làm Đẹp</option>
              <option value="CO">Điện Tử</option>
              <option value="DO">Nhà Cửa & Đời Sống</option>
              <option value="EO">Mẹ & Bé</option>
              <option value="FO">Thể Thao & Du Lịch</option>
              <option value="GO">Tiêu Dùng & Thực Phẩm</option>
              <option value="HO">Văn Phòng & Đồ Chơi</option>
              <option value="IO">Xe & Phụ Kiện</option>
              <option value="JO">Thẻ & Thẻ Cào</option>
              <option value="LO">Đồ Lưu Niệm</option>
              <option value="KO">Khác</option>
            </select>
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
          {
            imgSrc: "Link SP",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "Mô Tả",
          },
          {
            imgSrc: "Link SP",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "Mô Tả",
          },
          {
            imgSrc: "Link SP",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "Mô Tả",
          },
        ],
        TIKTOK: [
          {
            imgSrc: "Link SP",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "Mô Tả",
          },
        ],
        OTISShop: [
          {
            imgSrc: "Link SP",
            name: "Tên SP",
            price: "Giá SP",
            code: "Mã SP",
            category: "Phân Loại",
            link: "Link Liên Kết",
            description: "Mô Tả",
          },
        ],
      };

      // Tạo HTML cho sản phẩm SHOPEE
      function generateShopeeHTML(product) {
        return `
          <div class="product-column">
            <div class="product-row2">
              <img src="${product.imgSrc}" alt="${product.name}" />
              <div class="product-column2">
                <div class="name">${product.name}</div>
                <div class="price">Giá: ${product.price} VNĐ</div>
                <div class="product-actions">
                  <button class="save" onclick="copyProductInfo('${product.code}')">${product.code}</button>
                  <img src="https://i.pinimg.com/474x/66/84/3d/66843d89fb9a0e9770a18a02ed6261ce.jpg" alt="SHOPEE" />
                  <button class="link" onclick="window.open('${product.link}', '_blank')">Liên Kết</button>
                </div>
              </div>
            </div>
            <div class="product-description">
              <a href="javascript:void(0)" onclick="toggleDescription(this)"><u><b>Mô tả:</b></u></a>
              <div class="description-text">${product.description}</div>
            </div>
          </div>
        `;
      }

      // Tạo HTML cho sản phẩm TIKTOK
      function generateTiktokHTML(product) {
        return `
          <div class="product-column">
            <div class="product-row2">
              <img src="${product.imgSrc}" alt="${product.name}" />
              <div class="product-column2">
                <div class="name">${product.name}</div>
                <div class="price">Giá: ${product.price} VNĐ</div>
                <div class="product-actions">
                  <button class="save" onclick="copyProductInfo('${product.code}')">${product.code}</button>
                  <img src="https://i.pinimg.com/474x/05/8b/7c/058b7cd1e3a6d8e14d5b5906e84cb37a.jpg" alt="TIKTOK" />
                  <button class="link" onclick="window.open('${product.link}', '_blank')">Liên Kết</button>
                </div>
              </div>
            </div>
            <div class="product-description">
              <a href="javascript:void(0)" onclick="toggleDescription(this)"><u><b>Mô tả:</b></u></a>
              <div class="description-text">${product.description}</div>
            </div>
          </div>
        `;
      }

      // Tạo HTML cho sản phẩm OTISShop
      function generateOtisHTML(product) {
        return `
          <div class="product-column">
            <div class="product-row2">
              <img src="${product.imgSrc}" alt="${product.name}" />
              <div class="product-column2">
                <div class="name">${product.name}</div>
                <div class="price">Giá: ${product.price} VNĐ</div>
                <div class="product-actions">
                  <button class="save" onclick="copyProductInfo('${product.code}')">${product.code}</button>
                  <img src="https://i.pinimg.com/474x/ea/24/e1/ea24e1a0ed40857020ab39336b9fc78c.jpg" alt="OTISShop" />
                  <button class="oder" onclick="window.open('${product.link}', '_blank')">Mua Hàng</button>
                </div>
              </div>
            </div>
            <div class="product-description">
              <a href="javascript:void(0)" onclick="toggleDescription(this)"><u><b>Mô tả:</b></u></a>
              <div class="description-text">${product.description}</div>
            </div>
          </div>
        `;
      }

      // Hàm toggle mô tả sản phẩm
      function toggleDescription(element) {
        const descriptionText =
          element.parentElement.querySelector(".description-text");

        // Chuyển đổi trạng thái hiển thị của mô tả
        if (descriptionText.style.display === "none") {
          descriptionText.style.display = "block";
        } else {
          descriptionText.style.display = "none";
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
    <div class="icon-container">
      <!-- Icon Facebook -->
      <a href="https://www.facebook.com/OtisSeller" target="_blank">
        <div class="icon" style="width: 35px; height: 35px">
          <img
            src="https://i.pinimg.com/474x/c6/75/4f/c6754f858018877052f6b25bb2918b83.jpg"
            alt="Facebook"
          />
        </div>
      </a>

      <!-- Icon Instagram -->
      <a href="https://www.instagram.com/otisshopvn" target="_blank">
        <div class="icon" style="width: 35px; height: 35px">
          <img
            src="https://i.pinimg.com/474x/f6/bc/ca/f6bccaf046f990955aa739ade2f390b9.jpg"
            alt="Instagram"
          />
        </div>
      </a>

      <!-- Icon Threads -->
      <a href="https://www.threads.net/@otisshopvn" target="_blank">
        <div class="icon" style="width: 35px; height: 35px">
          <img
            src="https://i.pinimg.com/474x/b4/e7/c2/b4e7c21b60917993b65259e40bab277e.jpg"
            alt="Threads"
          />
        </div>
      </a>

      <!-- Home -->
      <a href="#">
        <div class="icon" style="width: 50px; height: 50px">
          <img
            src="https://i.pinimg.com/474x/6e/b7/72/6eb77283d62316f2b66bc1f7e3abdbb1.jpg"
            alt="Home"
          />
        </div>
      </a>

      <!-- Logo để mở/ẩn phần Shopping-->
      <div
        class="icon"
        style="width: 35px; height: 35px"
        onclick="toggleContact('contactShopping')"
      >
        <img
          src="https://i.pinimg.com/474x/f7/22/3e/f7223e8daaee44645802955532e1c372.jpg"
          alt="shopping"
        />
      </div>
      <!-- Nội dung Shopping-->
      <div class="contact-Shopping" id="contactShopping">
        <h3 style="text-align: center">
          Đặt Hàng!
          <button class="OUT" onclick="toggleContact('contactShopping')">
            X
          </button>
          <button class="oder" onclick="sendMessageWithClipboard()">
            Mua Hàng
          </button>
        </h3>
        <li>
          Để đặt hàng vui lòng chọn <b>Mua Hàng</b>, sao đó gửi mã sản phẩm và
          thông tin cho chúng tôi thông qua Fanpage của OTISShop!
        </li>
        <li>
          Shop chỉ tư vấn - <b>không</b> bán sản phẩm thuộc <b>Shopee</b>,
          <b>TikTok</b>! Vui lòng liên hệ <b>Shop bán hàng</b> bằng
          <b>Liên Kết</b> có trên sản phẩm!
        </li>
        <p style="text-align: center">❤️ Chân Thành Cảm Ơn Quý Khách! ❤️</p>
      </div>

      <!-- Logo để mở/ẩn phần Chatting -->
      <div
        class="icon"
        style="width: 35px; height: 35px"
        onclick="toggleContact('contactChatting')"
      >
        <img
          src="https://i.pinimg.com/474x/e8/9b/26/e89b26c7cc12836e637c7ce3ea36c9bb.jpg"
          alt="chatting"
        />
      </div>
      <!-- Nội dung Chatting -->
      <div class="contact-Chatting" id="contactChatting">
        <h3 style="text-align: center">
          Liên hệ!
          <button class="OUT" onclick="toggleContact('contactChatting')">
            X
          </button>
        </h3>
        <p>
          <li>Liên kết bán hàng - Tiếp thị - Tư vấn - Quảng Cáo.</li>
          <li>
            Hotline: <a href="tel:0329022431" target="_blank">0329022431</a>.
          </li>
          <li>
            Email:
            <a href="mailto:thinhkvtm2006@gmail.com">thinhkvtm2006@gmail.com</a
            >.
          </li>
          <li>
            Fanpage:
            <a
              href="https://www.messenger.com/t/460099260527241?"
              target="_blank"
              >https://www.facebook.com/OtisSeller</a
            >.
          </li>
        </p>
      </div>

      <!-- Logo để mở/ẩn phần Hướng dẫn -->
      <div
        class="icon"
        style="width: 35px; height: 35px"
        onclick="toggleContact('contactContent')"
      >
        <img
          src="https://i.pinimg.com/474x/42/bc/f8/42bcf85126a5757cd190602a4952db32.jpg"
          alt="content"
        />
      </div>
      <!-- Nội dung Hướng dẫn -->
      <div class="contact-Content" id="contactContent">
        <h3 style="text-align: center">
          Hướng Dẫn!
          <button class="OUT" onclick="toggleContact('contactContent')">
            X
          </button>
        </h3>
        <p>
          <li>
            Khi click vào mã sản phẩm (<b>SP-AB00</b>), mã sẽ được lưu vào
            <b>Clipboard</b> của bạn! Vui lòng gửi mã sản phẩm khi
            <a
              href="https://www.messenger.com/t/460099260527241?"
              target="_blank"
              ><b>Liên Hệ</b></a
            >
            với chúng tôi!
          </li>
          <li>
            Shop chỉ tư vấn - <b>không</b> bán sản phẩm thuộc <b>Shopee</b>,
            <b>TikTok</b>! Vui lòng liên hệ <b>Shop bán hàng</b> bằng
            <b>Liên Kết</b> có trên sản phẩm!
          </li>
        </p>
      </div>
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
              alert("Lưu mã thành công! Vui lòng chọn 'Giỏ Hàng'!");
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
        console.log("Vui lòng lưu mã sản phẩm trước!");
      };

      // Hàm để chuyển đổi hiển thị của các phần nội dung liên lạc
      function toggleContact(contentID) {
        var content = document.getElementById(contentID);
        var content1 = document.getElementById("contactContent");
        var content2 = document.getElementById("contactChatting");
        var content3 = document.getElementById("contactShopping");

        // Ẩn tất cả các phần tử khác trước khi hiển thị phần tử mới
        if (contentID === "contactContent") {
          content2.style.display = "none";
          content3.style.display = "none";
        }
        if (contentID === "contactChatting") {
          content1.style.display = "none";
          content3.style.display = "none";
        }
        if (contentID === "contactShopping") {
          content1.style.display = "none";
          content2.style.display = "none";
        }

        // Chuyển đổi trạng thái hiển thị của phần tử được chọn
        if (content.style.display !== "block") {
          content.style.display = "block";
        } else {
          content.style.display = "none";
        }
      }

      // Hàm gửi tin nhắn với nội dung sao chép từ clipboard
      async function sendMessageWithClipboard() {
        try {
          // Đọc nội dung từ clipboard
          const clipboardText = await navigator.clipboard.readText();

          // Kiểm tra nếu clipboard không có nội dung
          if (!clipboardText.trim()) {
            alert("Vui lòng lưu mã sản phẩm trước!");
            return;
          }

          // Soạn nội dung tin nhắn
          const message = `Tôi muốn biết thông tin về các sản phẩm sau: ${clipboardText}.`;

          // Tạo URL Messenger với nội dung tin nhắn
          const url = `https://www.messenger.com/t/460099260527241?text=${encodeURIComponent(
            message
          )}`;

          // Mở URL trong tab mới
          window.open(url, "_blank");

          // Lý do không thể gửi tự động:
          // Trình duyệt hiện nay yêu cầu có sự tương tác của người dùng để gửi tin nhắn.
          // Để gửi tin nhắn trực tiếp mà không cần người dùng nhấn, cần sử dụng API của Messenger (không thể qua link đơn giản).
        } catch (err) {
          console.error("Không thể đọc dữ liệu: ", err);
          alert("Không thể truy cập clipboard. Hãy đảm bảo bạn đã cấp quyền.");
        }
      }
    </script>
  </body>
</html>
