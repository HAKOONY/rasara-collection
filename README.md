# rasara-collection
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>RASARA 25 졸업기획전</title>
  <style>
    body {
      font-family: 'Noto Sans KR', sans-serif;
      margin: 0;
      padding: 0;
      background: #ffffff;
      color: #333;
    }

    .header-wrap {
      background-color: #fff;
      border-bottom: 1px solid #eee;
    }

    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 20px;
      max-width: 1280px;
      margin: 0 auto;
      flex-wrap: wrap;
    }

    .logo {
      height: 40px;
    }

    .menu-bar {
      display: flex;
      gap: 20px;
      position: relative;
      flex-wrap: wrap;
    }

    .menu-item {
      position: relative;
      font-weight: bold;
      cursor: pointer;
    }

    .menu-item:hover {
      color: #a1001a;
    }

    .submenu {
      display: none;
      position: absolute;
      top: 30px;
      left: 0;
      background-color: #fff;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      padding: 10px 0;
      border-radius: 6px;
      z-index: 1000;
      min-width: 140px;
    }

    .menu-item:hover .submenu {
      display: block;
    }

    .submenu a {
      display: block;
      padding: 8px 20px;
      text-decoration: none;
      font-size: 14px;
      color: #333;
    }

    .submenu a:hover {
      background-color: #f5f5f5;
    }

    .banner {
      width: 100%;
      height: auto;
    }

    .title {
      font-size: 24px;
      font-weight: bold;
      text-align: center;
      margin: 30px 0 20px;
      padding: 0 15px;
    }

    .product-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
      gap: 16px;
      max-width: 1200px;
      margin: auto;
      padding: 0 15px 40px;
    }

    .product-card {
      display: block;
      border: 1px solid #eee;
      border-radius: 10px;
      overflow: hidden;
      text-align: center;
      transition: transform 0.2s;
      text-decoration: none;
      color: inherit;
      background-color: #fff;
    }

    .product-card:hover {
      transform: scale(1.03);
    }

    .product-card img {
      width: 100%;
      height: auto;
      display: block;
    }

    .product-name {
      padding: 15px 10px 5px;
      font-size: 14px;
      font-weight: 500;
    }

    .product-price {
      color: #a1001a;
      font-weight: bold;
      padding-bottom: 15px;
      font-size: 13px;
    }

    @media (max-width: 480px) {
      .title {
        font-size: 20px;
      }

      .product-grid {
        grid-template-columns: 1fr;
      }

      .menu-bar {
        flex-direction: column;
        gap: 10px;
      }
    }
  </style>
</head>
<body>

  <!-- 상단 로고 & 카테고리 -->
  <div class="header-wrap">
    <div class="header">
      <img src="https://i.postimg.cc/sD4r1Vmv/rasara-oglogo.png" class="logo" alt="라사라 로고" />

      <div class="menu-bar">
        <div class="menu-item">WOMEN
          <div class="submenu">
            <a href="#">티셔츠</a>
            <a href="#">바지</a>
            <a href="#">원피스</a>
          </div>
        </div>
        <div class="menu-item">MEN
          <div class="submenu">
            <a href="#">셔츠</a>
            <a href="#">팬츠</a>
            <a href="#">자켓</a>
          </div>
        </div>
        <div class="menu-item">ACC
          <div class="submenu">
            <a href="#">모자</a>
            <a href="#">가방</a>
            <a href="#">양말</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- 배너 -->
  <img class="banner" src="https://i.postimg.cc/VsM1Q9b9/image.jpg" alt="썸머기획전 배너" />

  <!-- 타이틀 -->
  <div class="title">25 RASARA COLLECTION</div>

  <!-- 상품 리스트 -->
  <div class="product-grid">

    <a href="detail-ovi1.html" class="product-card">
      <img src="https://i.postimg.cc/XN9x0XNB/ovi.png" alt="상품1" />
      <div class="product-name">OVI_1</div>
      <div class="product-price">₩00,000</div>
    </a>

    <a href="detail-ovi2.html" class="product-card">
      <img src="https://i.postimg.cc/8CDNt7Cd/ovi-2.png" alt="상품2" />
      <div class="product-name">OVI_2</div>
      <div class="product-price">₩000,000</div>
    </a>

    <a href="detail-synth1.html" class="product-card">
      <img src="https://i.postimg.cc/k4LnNfRG/synth.png" alt="상품3" />
      <div class="product-name">SYNTH_1</div>
      <div class="product-price">₩00,000</div>
    </a>

    <a href="detail-4.html" class="product-card">
      <img src="https://i.postimg.cc/xd4YYtR5/image.png" alt="상품4" />
      <div class="product-name">---</div>
      <div class="product-price">₩00,000</div>
    </a>

    <a href="detail-5.html" class="product-card">
      <img src="https://i.postimg.cc/ZnkSvnXy/image.png" alt="상품5" />
      <div class="product-name">---</div>
      <div class="product-price">₩00,000</div>
    </a>

  </div>

</body>
</html>

