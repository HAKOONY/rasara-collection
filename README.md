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
  background: #f0f0f0; /* ✅ 전체 배경 라이트그레이 */
  color: #333;
}

.header-wrap {
  background-color: #a1001a; /* ✅ 와인색 */
  padding: 10px 0;
}

.menu-bar {
  display: flex;
  align-items: center;
  gap: 24px;
  flex-wrap: wrap;
  justify-content: center;
}

.menu-item a {
  color: #f0f0f0; /* ✅ 밝은 회색 텍스트 */
  text-decoration: none;
  font-weight: 600;
  padding: 6px 14px;
  border-radius: 20px;
  transition: background 0.3s ease;
}

.menu-item a:hover {
  background-color: rgba(255, 255, 255, 0.15); /* ✅ 자연스러운 호버 효과 */
  color: #fff;
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
  color: #d3d3d3 !important; /* ✅ 기본 라이트그레이 */
  text-decoration: none;
  font-weight: 600;
  padding: 6px 14px;
  border-radius: 20px;
  transition: background 0.3s ease;
}

  .menu-item a:hover {
  background-color: rgba(255, 255, 255, 0.15);
  color: #ffffff !important; /* ✅ 호버 시 흰색 */
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
}

 .image-item {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.image-title {
  font-size: 20px;
  font-weight: bold;
  margin-top: 10px;
  text-align: center;
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
  <div class="header" style="display:flex; justify-content: space-between; align-items: center; max-width: 1280px; margin: 0 auto; padding: 0 20px;">
    
    <!-- 🔻 라사라 로고만 표시 (텍스트 제거) -->
    <a href="https://hakoony.github.io/rasara-collection/" style="display: flex; align-items: center; text-decoration: none;">
      <img src="https://i.postimg.cc/sD4r1Vmv/rasara-oglogo.png" class="logo" alt="라사라 로고" style="height: 40px; mix-blend-mode: multiply; filter: contrast(1.2);" />
    </a>

 <div class="menu-bar">
      <div class="menu-item">
        <a href="https://hakoony.github.io/rasara-collection/ovi.html" style="color:#d3d3d3;">OVI</a>
      </div>
      <div class="menu-item">
        <a href="https://hakoony.github.io/rasara-collection/ville.html" style="color:#d3d3d3;">Ville Lumière</a>
      </div>
      <div class="menu-item">
        <a href="https://hakoony.github.io/rasara-collection/timelessabout.html" style="color:#d3d3d3;">timelessabout</a>
      </div>
    </div>
  </div>
</div>
    
  <!-- 배너 -->
<!-- 슬라이드 배너 -->
<div class="slider">
  <img src="https://i.postimg.cc/vmX9SnyW/ville.jpg" class="slide active" />
  <img src="https://i.postimg.cc/KvvCx7G5/1750933135843.jpg" class="slide" />
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

  setInterval(showNextSlide, 2000); // 2초마다 전환
</script>
  <!-- 타이틀 -->
  <div class="title">25 RASARA X BRAND-ER COLLECTION </div>

<!-- ✅ BRAND-ER 박스 수정본 (배경색만 유지하고 글자 삭제) -->
<div style="max-width: 600px; margin: 50px auto; padding: 40px; background: #ffffff; box-shadow: 0 0 15px rgba(0,0,0,0.05); border-radius: 12px; text-align: center; display: flex; flex-direction: column; align-items: center;">
  <img src="https://i.postimg.cc/76k0stMf/image.png" alt="BRAND-ER 로고" style="height: 40px; margin-bottom: 20px;">
  <a href="https://brand-er.store/custom/index.html" target="_blank" style="display: inline-block; padding: 12px 30px; background-color: #f5f5f5; color:#a1001a;border-radius: 30px; text-decoration: none; font-weight: 500;">
    make my brand    
  </a>
</div>    
<div class="image-grid">
  <div class="image-item">
    <div class="image-title">OVI</div>
    <div style="align-items:center;">
    <img src="https://i.postimg.cc/rphnQsRN/1750937125634.png" alt="ovi" />
  </div>
  </div>
  <div class="image-item">
    <div class="image-title">TIMELESSABOUT</div>
    <div style="align-items:center;">
			<img src="https://i.postimg.cc/zGs3WG3V/1750925772404.png" alt="timelessabout" />
</div>
 </div>
 <div class="image-item">
    <div class="image-title">Ville Lumière</div>
    <div style="align-items:center;">
			<img src="https://i.postimg.cc/TPCvr3b2/1751186179253.jpg" alt="Ville Lumière" />
</div>
</div>
</div>

</body>
</html>
