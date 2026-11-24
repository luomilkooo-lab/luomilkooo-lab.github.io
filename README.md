# -luomilkooo-lab.github.io
<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>LUO DIMENSION | 3D CREATIVE SPACE</title>

<style>

:root {
  --bg: #F3F1EA;
  --card: #E8E6DD;
  --text: #252820;
  --muted: #85857C;
  --accent: #78836A;
  --line: rgba(37,40,32,0.15);
  --white: #FFFFFF;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  background: var(--bg);
  color: var(--text);
  font-family: Arial, "Noto Sans TC", sans-serif;
  overflow-x: hidden;
}

a {
  color: inherit;
  text-decoration: none;
}

/* =========================
   NAVIGATION
========================= */

header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 100;
  padding: 23px 7%;

  display: flex;
  align-items: center;
  justify-content: space-between;

  background: rgba(243,241,234,0.92);
  backdrop-filter: blur(15px);

  border-bottom: 1px solid var(--line);
}

.logo {
  font-size: 20px;
  font-weight: 800;
  letter-spacing: 3px;
}

.logo span {
  color: var(--accent);
}

nav {
  display: flex;
  gap: 30px;
}

nav a {
  font-size: 11px;
  letter-spacing: 2px;
  color: var(--muted);
  transition: 0.3s;
}

nav a:hover {
  color: var(--accent);
}

/* =========================
   HERO
========================= */

.hero {
  min-height: 100vh;
  position: relative;
  display: flex;
  align-items: center;
  padding: 120px 7% 80px;

  background-color: #F3F1EA;

  background-image:
    linear-gradient(
      90deg,
      rgba(243,241,234,0.98) 0%,
      rgba(243,241,234,0.88) 28%,
      rgba(243,241,234,0.35) 55%,
      rgba(243,241,234,0.00) 100%
    ),
    url("https://drive.google.com/thumbnail?id=1CSYEtEK5ME8ZRXPTu4wSJYuwycvO1VIs&sz=w2000");

  background-size:
    cover,
    auto 85%;

  background-position:
    center,
    center 25%;

  background-repeat: no-repeat;
}

.hero-content {
  max-width: 650px;
  position: relative;
  z-index: 2;
}

.eyebrow {
  color: var(--accent);
  font-size: 11px;
  letter-spacing: 4px;
  margin-bottom: 25px;
}

.hero h1 {
  font-size: clamp(48px, 8vw, 100px);
  line-height: 0.95;
  letter-spacing: -3px;
  margin-bottom: 22px;
  font-weight: 800;
}

.hero h2 {
  font-size: 16px;
  font-weight: 400;
  letter-spacing: 7px;
  color: var(--accent);
  margin-bottom: 35px;
}

.hero p {
  color: #68695F;
  line-height: 2.1;
  font-size: 14px;
  max-width: 480px;
  margin-bottom: 35px;
}

.hero-button {
  display: inline-block;
  padding: 15px 28px;

  border: 1px solid var(--accent);
  color: var(--accent);

  font-size: 11px;
  letter-spacing: 2px;

  transition: 0.3s;
}

.hero-button:hover {
  background: var(--accent);
  color: var(--white);
}

/* =========================
   COMMON SECTION
========================= */

section {
  padding: 110px 7%;
}

.section-label {
  color: var(--accent);
  font-size: 11px;
  letter-spacing: 4px;
  margin-bottom: 18px;
}

.section-title {
  font-size: clamp(32px, 5vw, 55px);
  margin-bottom: 18px;
  letter-spacing: 1px;
}

.section-description {
  color: var(--muted);
  line-height: 1.9;
  font-size: 14px;
  margin-bottom: 55px;
}

/* =========================
   CREATIVE STUDIO
========================= */

.studio {
  background: #EAE8DF;
}

.studio-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 18px;
}

.studio-card {
  min-height: 210px;
  padding: 30px 24px;

  background: #F3F1EA;
  border: 1px solid var(--line);

  transition: 0.35s;
  position: relative;
}

.studio-card:hover {
  transform: translateY(-7px);
  border-color: var(--accent);
}

.studio-card .number {
  color: var(--accent);
  font-size: 11px;
  margin-bottom: 45px;
  letter-spacing: 2px;
}

.studio-card h3 {
  font-size: 16px;
  letter-spacing: 1px;
  margin-bottom: 12px;
}

.studio-card p {
  color: var(--muted);
  font-size: 12px;
  line-height: 1.8;
}

/* =========================
   SOFTWARE
========================= */

.software {
  background: var(--bg);
}

.software-heading {
  display: flex;
  justify-content: space-between;
  align-items: end;
  gap: 30px;
  margin-bottom: 55px;
}

.software-heading .section-description {
  margin-bottom: 0;
}

.software-tag {
  color: var(--accent);
  font-size: 10px;
  letter-spacing: 3px;
  white-space: nowrap;
  padding-bottom: 5px;
}

.software-list {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.software-card {
  min-height: 280px;
  padding: 35px 30px;

  background: #EAE8DF;
  border: 1px solid var(--line);

  position: relative;
  overflow: hidden;
  transition: 0.35s;
}

.software-card:hover {
  transform: translateY(-8px);
  border-color: var(--accent);
}

.software-number {
  color: var(--accent);
  font-size: 11px;
  letter-spacing: 3px;
  margin-bottom: 45px;
}

.software-card h3 {
  font-size: 27px;
  letter-spacing: 1px;
  margin-bottom: 15px;
}

.software-card .chinese {
  font-size: 14px;
  color: var(--text);
  margin-bottom: 8px;
}

.software-card .english {
  font-size: 11px;
  color: var(--muted);
  letter-spacing: 1px;
}

.software-line {
  width: 35px;
  height: 2px;
  background: var(--accent);
  margin-top: 25px;
}

/* =========================
   PROJECTS
========================= */

.projects {
  background: #EAE8DF;
}

.project-placeholder {
  min-height: 260px;

  border: 1px dashed rgba(120,131,106,0.5);

  display: flex;
  align-items: center;
  justify-content: center;

  text-align: center;
  color: var(--muted);
  padding: 30px;
}

.project-placeholder h3 {
  color: var(--accent);
  font-size: 15px;
  letter-spacing: 3px;
  margin-bottom: 15px;
}

.project-placeholder p {
  font-size: 13px;
  line-height: 2;
}

/* =========================
   ABOUT
========================= */

.about {
  background: var(--bg);
}

.about-content {
  max-width: 750px;
}

.about-content p {
  color: #68695F;
  line-height: 2.2;
  font-size: 14px;
}

/* =========================
   FOOTER
========================= */

footer {
  padding: 35px 7%;

  border-top: 1px solid var(--line);

  display: flex;
  justify-content: space-between;
  gap: 20px;

  color: var(--muted);
  font-size: 10px;
  letter-spacing: 2px;
}

/* =========================
   RESPONSIVE
========================= */

@media (max-width: 900px) {

  .studio-grid {
    grid-template-columns: repeat(2, 1fr);
  }

  .software-list {
    grid-template-columns: 1fr;
  }

  .software-card {
    min-height: 230px;
  }

}

@media (max-width: 600px) {

  header {
    padding: 18px 5%;
  }

  .logo {
    font-size: 14px;
    letter-spacing: 2px;
  }

  nav {
    gap: 10px;
  }

  nav a {
    font-size: 8px;
    letter-spacing: 0.5px;
  }

  .hero {
    min-height: 100vh;
    padding: 120px 7% 70px;

    background-size:
      cover,
      auto 58%;

    background-position:
      center,
      center 25%;
  }

  .hero h1 {
    font-size: 48px;
  }

  .hero h2 {
    font-size: 12px;
    letter-spacing: 4px;
  }

  section {
    padding: 80px 7%;
  }

  .studio-grid {
    grid-template-columns: 1fr;
  }

  .software-heading {
    display: block;
  }

  .software-tag {
    display: inline-block;
    margin-top: 20px;
  }

  footer {
    flex-direction: column;
    line-height: 1.8;
  }

}

</style>
</head>

<body>

<!-- NAVIGATION -->

<header>

  <a href="#home" class="logo">
    LUO DIMENSION<span>.</span>
  </a>

  <nav>
    <a href="#home">HOME</a>
    <a href="#studio">STUDIO</a>
    <a href="#software">SOFTWARE</a>
    <a href="#projects">PROJECTS</a>
    <a href="#about">ABOUT</a>
  </nav>

</header>


<main>

<!-- HOME -->

<section class="hero" id="home">

  <div class="hero-content">

    <div class="eyebrow">
      WELCOME TO MY CREATIVE WORLD
    </div>

    <h1>
      LUO<br>DIMENSION
    </h1>

    <h2>
      3D CREATIVE SPACE
    </h2>

    <p>
      探索立體世界，創造無限可能。<br>
      從設計、機械結構到 3D 建模，<br>
      將每一個想法轉化為真實作品。
    </p>

    <a href="#studio" class="hero-button">
      EXPLORE MORE ↗
    </a>

  </div>

</section>


<!-- CREATIVE STUDIO -->

<section class="studio" id="studio">

  <div class="section-label">
    01 — CREATIVE STUDIO
  </div>

  <h2 class="section-title">
    CREATIVE STUDIO
  </h2>

  <p class="section-description">
    從創意發想到實際製作，探索不同領域的設計可能。
  </p>

  <div class="studio-grid">

    <div class="studio-card">
      <div class="number">01 / DESIGN</div>
      <h3>3D MODELING</h3>
      <p>三維建模與產品外觀設計。</p>
    </div>

    <div class="studio-card">
      <div class="number">02 / STRUCTURE</div>
      <h3>MECHANICAL</h3>
      <p>機械結構、零件與機構設計。</p>
    </div>

    <div class="studio-card">
      <div class="number">03 / MAKING</div>
      <h3>3D PRINTING</h3>
      <p>將數位模型轉化為實體作品。</p>
    </div>

    <div class="studio-card">
      <div class="number">04 / EXPLORE</div>
      <h3>DIGITAL LAB</h3>
      <p>數位工具、創意實驗與技術探索。</p>
    </div>

  </div>

</section>


<!-- SOFTWARE -->

<section class="software" id="software">

  <div class="software-heading">

    <div>

      <div class="section-label">
        02 — SOFTWARE & ENGINEERING
      </div>

      <h2 class="section-title">
        TOOLS & SKILLS
      </h2>

      <p class="section-description">
        設計、建模與工程領域使用的軟體工具。
      </p>

    </div>

    <div class="software-tag">
      DESIGN / MODELING / ENGINEERING
    </div>

  </div>


  <div class="software-list">

    <div class="software-card">

      <div class="software-number">
        SOFTWARE — 01
      </div>

      <h3>AutoCAD</h3>

      <div class="chinese">
        機構設計
      </div>

      <div class="english">
        2D ENGINEERING DRAWING
      </div>

      <div class="software-line"></div>

    </div>


    <div class="software-card">

      <div class="software-number">
        SOFTWARE — 02
      </div>

      <h3>SOLIDWORKS</h3>

      <div class="chinese">
        數位模型
      </div>

      <div class="english">
        3D MODELING
      </div>

      <div class="software-line"></div>

    </div>


    <div class="software-card">

      <div class="software-number">
        SOFTWARE — 03
      </div>

      <h3>Creo</h3>

      <div class="chinese">
        產品設計
      </div>

      <div class="english">
        PRODUCT DESIGN
      </div>

      <div class="software-line"></div>

    </div>

  </div>

</section>


<!-- PROJECTS -->

<section class="projects" id="projects">

  <div class="section-label">
    03 — PROJECTS
  </div>

  <h2 class="section-title">
    MY PROJECTS
  </h2>

  <p class="section-description">
    IDEAS INTO REALITY
  </p>

  <div class="project-placeholder">

    <div>

      <h3>COMING SOON</h3>

      <p>
        這裡將展示我的 3D 建模、機械設計與列印作品。
      </p>

    </div>

  </div>

</section>


<!-- ABOUT -->

<section class="about" id="about">

  <div class="section-label">
    04 — ABOUT
  </div>

  <h2 class="section-title">
    ABOUT LUO
  </h2>

  <div class="about-content">

    <p>
      LUO DIMENSION 是一個結合創意設計、工程技術與 3D 列印的個人創作空間。
      <br><br>
      我相信每個想法都能透過設計與實作，逐漸轉化為真實的作品。
      從一個簡單的構想開始，不斷學習、嘗試與創造。
    </p>

  </div>

</section>

</main>


<!-- FOOTER -->

<footer>

  <div>
    © 2026 LUO DIMENSION.
  </div>

  <div>
    ALL RIGHTS RESERVED.
  </div>

</footer>

</body>
</html>
