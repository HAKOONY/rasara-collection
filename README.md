# rasara-collection
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
    align-items: center;
    gap: 30px; /* ✅ 간격 통일 */
    flex-wrap: wrap;
  }

  .menu-item {
    position: relative;
    font-weight: bold;
    cursor: pointer;
  }

  .menu-item a {
    color: #111;
    text-decoration: none;
    font-weight: bold;
    padding: 8px 10px; /* ✅ 클릭 범위 확대 */
    display: inline-block;
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
      
       .menu-item a {
      color: #111; /* 검정색 텍스트 */
      text-decoration: none;
      font-weight: bold;
    }

    .menu-item a:hover {
      color: #a1001a; /* hover 시 와인색 강조 */
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
    
.image-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); /* 유동적으로 너비 조절 */
  gap: 24px; /* 사진 사이 여백 */
  max-width: 1000px;
  margin: 60px auto;
  padding: 0 20px;
}

.image-grid img {
  width: 100%;
  aspect-ratio: 1 / 1.2;  /* ✅ 통일된 세로 비율 */
  object-fit: cover;     /* ✅ 사진이 꽉 차게 */
  border-radius: 16px;   /* ✅ 부드러운 테두리 */
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.05); /* ✅ 고급스러운 그림자 */
  transition: transform 0.3s ease;

  /* 👇 여기에 추가하세요 */
  .image-item {
    text-align: center;
  }

  .image-title {
    font-size: 20px;
    font-weight: bold;
    margin-bottom: 10px;
  }


.image-grid img:hover {
  transform: scale(1.03); /* ✅ 확대 효과 */
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
        <div class="menu-item">
  					<a href="https://hakoony.github.io/rasara-collection/ovi.html">OVI</a>
          <div class="submenu">
        </div>
        </div>
 
        <div class="menu-item">
          		<a href="https://hakoony.github.io/rasara-collection/ville.html">Ville Lumière</a>       
          </div>
        </div>
      <div class="menu-item">
   			<a href="https://hakoony.github.io/rasara-collection/timelessabout.html">timelessabout</a>
					</div>          

         <div class="menu-item">
          <div class="submenu">
      </div>
    </div>
     <div class="menu-item">?
          <div class="submenu">
            <a href="#">모자</a>
            <a href="#">가방</a>
            <a href="#">양말</a>
  </div>
</div>
</div>
</div>

  <!-- 배너 -->
<!-- 슬라이드 배너 -->
<div class="slider">
  <img src="https://i.postimg.cc/VsM1Q9b9/image.jpg" class="slide active" />
  <img src="https://i.postimg.cc/pdCmfTRJ/1750925772270.png" class="slide" />
</div>

<style>
  .slider {
    width: 100%;
    height: 250px;
    position: relative;
    overflow: hidden;
    background-color: #fff;
  }

  .slider img {
  position: absolute;
  width: 100%;
  height: 100%;
  object-fit: scale-down; /* 또는 contain 유지 */
  padding: 10px;
  opacity: 0;
  transition: opacity 1s ease-in-out;
  background-color: transparent; /* ✅ 배경 투명하게 */
}

  .slider img.active {
    opacity: 1;
    z-index: 1;
  }
</style>

<script>
  const slides = document.querySelectorAll(".slide");
  let index = 0;

  function showNextSlide() {
    slides[index].classList.remove("active");
    index = (index + 1) % slides.length;
    slides[index].classList.add("active");
  }

  setInterval(showNextSlide, 3000); // 3초마다 전환
</script>
  <!-- 타이틀 -->
  <div class="title">25 RASARA X BRAND-ER COLLECTION </div>


<div style="max-width: 600px; margin: 50px auto; padding: 40px; background: #ffffff; box-shadow: 0 0 15px rgba(0,0,0,0.05); border-radius: 12px; text-align: center; display: flex; flex-direction: column; align-items: center;">
  <img src="https://i.postimg.cc/76k0stMf/image.png" alt="BRAND-ER 로고" style="height: 40px; margin-bottom: 20px;">
<h2 style="font-size: 36px; font-weight: bold; margin-bottom: 15px; width: 100%; text-align: center;">  BRAND-ER</h2>
  <p style="font-size: 25px; color: #555; margin-bottom: 25px;">당신만의 브랜드를 만들다.</p>
  <a href="https://brand-er.store/custom/index.html" target="_blank" style="display: inline-block; padding: 12px 30px; background-color: #f5f5f5; color:#a1001a;border-radius: 30px; text-decoration: none; font-weight: 500;">
make my brand    
  </a>
</div>
<div class="image-grid">
  <div class="image-item">
    <div class="image-title">OVI</div>
    <img src="https://i.postimg.cc/rphnQsRN/1750937125634.png" alt="ovi" />
  </div>
  <div class="image-item">
    <div class="image-title">TIMELESSABOUT</div>
    <img src="https://i.postimg.cc/zGs3WG3V/1750925772404.png" alt="timelessabout" />
</div>
 <div class="image-item">
    <div class="image-title">Ville Lumière</div>
    <img src="https://i.postimg.cc/TPCvr3b2/1751186179253.jpg" alt="Ville Lumière" />
</div>

</div>
</body>
</html>

