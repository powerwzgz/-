# -<!-- 樂澄專業清洗企業社 完整網站程式碼 (含Icon、背景圖、SEO架構) -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

<style>
  .lc-wrapper {
    font-family: "PingFang TC", "Microsoft JhengHei", sans-serif;
    color: #1e293b;
    line-height: 1.7;
    background-color: #ffffff;
    width: 100%;
    overflow-x: hidden;
  }
  .lc-wrapper * { box-sizing: border-box; margin: 0; padding: 0; }
  
  /* 1. 首屏主視覺背景圖 */
  .lc-hero {
    background: linear-gradient(135deg, rgba(15, 23, 42, 0.8), rgba(2, 132, 199, 0.75)),
                url('https://images.unsplash.com/photo-1581578731548-c64695cc6952?auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
    color: #ffffff;
    text-align: center;
    padding: 100px 20px;
  }
  .lc-badge {
    display: inline-block;
    background: rgba(255, 255, 255, 0.2);
    border: 1px solid rgba(255, 255, 255, 0.4);
    padding: 6px 18px;
    border-radius: 50px;
    font-size: 0.95rem;
    margin-bottom: 20px;
    letter-spacing: 1px;
  }
  .lc-hero h1 {
    font-size: clamp(2rem, 4vw, 3rem);
    font-weight: 800;
    margin-bottom: 18px;
    line-height: 1.3;
  }
  .lc-hero p {
    font-size: clamp(1rem, 2vw, 1.25rem);
    max-width: 780px;
    margin: 0 auto 35px;
    opacity: 0.95;
  }
  .lc-btn-line {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background-color: #06c755;
    color: #ffffff !important;
    text-decoration: none;
    padding: 16px 36px;
    border-radius: 50px;
    font-size: 1.15rem;
    font-weight: bold;
    box-shadow: 0 8px 20px rgba(6, 199, 85, 0.35);
    transition: transform 0.2s, background-color 0.2s;
  }
  .lc-btn-line:hover {
    transform: translateY(-3px);
    background-color: #05b34c;
  }

  /* 通用區塊 */
  .lc-section {
    padding: 80px 20px;
    max-width: 1180px;
    margin: 0 auto;
  }
  .lc-bg-soft {
    background-color: #f0f9ff;
    background-image: radial-gradient(#bae6fd 1px, transparent 1px);
    background-size: 24px 24px;
  }
  .lc-title {
    text-align: center;
    font-size: clamp(1.75rem, 3vw, 2.25rem);
    color: #0369a1;
    margin-bottom: 14px;
    font-weight: 800;
  }
  .lc-subtitle {
    text-align: center;
    color: #475569;
    max-width: 760px;
    margin: 0 auto 50px;
    font-size: 1.05rem;
  }

  /* 2. 關於樂澄 & 四大保證 */
  .lc-features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 24px;
  }
  .lc-feature-card {
    background: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 16px;
    padding: 32px 24px;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.04);
  }
  .lc-feature-icon {
    width: 68px;
    height: 68px;
    margin: 0 auto 18px;
    background: #e0f2fe;
    color: #0284c7;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.8rem;
  }
  .lc-feature-card h3 {
    font-size: 1.25rem;
    margin-bottom: 10px;
    color: #0f172a;
  }
  .lc-feature-card p {
    color: #64748b;
    font-size: 0.95rem;
  }

  /* 3. 六大清潔服務卡片 */
  .lc-services {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 28px;
  }
  .lc-service-card {
    background: #ffffff;
    border-radius: 16px;
    padding: 32px;
    border-top: 5px solid #0284c7;
    box-shadow: 0 10px 25px rgba(2, 132, 199, 0.08);
  }
  .lc-service-icon {
    width: 56px;
    height: 56px;
    border-radius: 12px;
    background: #0284c7;
    color: #ffffff;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.6rem;
    margin-bottom: 20px;
  }
  .lc-service-card h3 {
    font-size: 1.35rem;
    margin-bottom: 8px;
    color: #0f172a;
  }
  .lc-tag {
    display: inline-block;
    background: #e0f2fe;
    color: #0369a1;
    font-size: 0.85rem;
    font-weight: 700;
    padding: 4px 12px;
    border-radius: 6px;
    margin-bottom: 14px;
  }
  .lc-service-card p {
    color: #475569;
    font-size: 0.95rem;
  }

  /* 4. 客戶評價區 */
  .lc-reviews {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 24px;
  }
  .lc-review-card {
    background: #f8fafc;
    border-left: 5px solid #0284c7;
    padding: 28px;
    border-radius: 12px;
  }
  .lc-stars { color: #f59e0b; margin-bottom: 12px; font-size: 1.1rem; }
  .lc-review-card p { font-size: 1rem; color: #334155; margin-bottom: 14px; }
  .lc-reviewer { font-weight: bold; color: #0369a1; font-size: 0.95rem; }

  /* 5. 聯絡與台灣地圖區 */
  .lc-contact-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
    gap: 32px;
    align-items: center;
  }
  .lc-contact-info {
    background: #0f172a;
    color: #ffffff;
    padding: 40px;
    border-radius: 16px;
  }
  .lc-contact-info h3 { font-size: 1.6rem; margin-bottom: 20px; color: #38bdf8; }
  .lc-info-item {
    display: flex;
    align-items: flex-start;
    gap: 14px;
    margin-bottom: 18px;
    font-size: 1.05rem;
  }
  .lc-info-item i { color: #38bdf8; font-size: 1.3rem; margin-top: 4px; }
  .lc-map iframe {
    width: 100%;
    height: 360px;
    border: 0;
    border-radius: 16px;
    box-shadow: 0 8px 25px rgba(0,0,0,0.1);
  }

  /* 6. 頁尾 */
  .lc-footer {
    background: #090d16;
    color: #94a3b8;
    text-align: center;
    padding: 40px 20px;
    font-size: 0.95rem;
  }
  .lc-footer strong { color: #ffffff; }
</style>

<div class="lc-wrapper">
  <!-- 首屏主視覺 -->
  <section class="lc-hero">
    <div class="lc-badge"><i class="fa-solid fa-sparkles"></i> 雙北、桃園家電與軟裝深層水洗專家</div>
    <h1>看不見的髒污，交給專業真水洗！<br>還原居家潔淨健康的呼吸與睡眠</h1>
    <p>【樂澄專業清洗企業社】創辦人小林先生親自領軍｜堅持專業安全洗劑搭配徹底物理水洗，全場禁菸酒檳榔、多層防水防護、提供 14 天安心售後保固。</p>
    <a href="https://line.me/R/ti/p/@749rgenw" target="_blank" class="lc-btn-line">
      <i class="fa-brands fa-line fa-xl"></i> 立即加 LINE 免費估價 (@749rgenw)
    </a>
  </section>

  <!-- 關於樂澄與四大堅持 -->
  <section class="lc-section">
    <h2 class="lc-title">關於樂澄專業清洗企業社</h2>
    <p class="lc-subtitle">
      現代居家與商辦空間長期累積灰塵、黴菌與數百萬塵蟎，冷氣、洗衣機、床墊與沙發往往成為過敏與異味的隱形源頭。小林先生以誠實、細膩的職人精神，服務涵蓋一般家庭住宅、商業辦公室、補習班、幼兒園、政府機關與渡假飯店，給您最安心可靠的清潔體驗。
    </p>
    <div class="lc-features">
      <div class="lc-feature-card">
        <div class="lc-feature-icon"><i class="fa-solid fa-droplet"></i></div>
        <h3>專業洗劑＋徹底物理水洗</h3>
        <p>絕不玩誇大行銷話術，堅持採用安全專業清潔液分解頑垢，再以高壓物理水洗徹底沖淨，確保零殘留。</p>
      </div>
      <div class="lc-feature-card">
        <div class="lc-feature-icon"><i class="fa-solid fa-shield-halved"></i></div>
        <h3>多層次嚴密防水防護</h3>
        <p>施工前針對周邊家電、牆面與裝潢進行多層次養生膠帶包覆防護，軟裝清洗搭配專業蝸牛風機加速乾燥。</p>
      </div>
      <div class="lc-feature-card">
        <div class="lc-feature-icon"><i class="fa-solid fa-ban-smoking"></i></div>
        <h3>高標準職人現場紀律</h3>
        <p>全場嚴格禁止吸菸、飲酒與嚼食檳榔，報價公開透明、不亂加價，給家人與孩子最放心的入室服務。</p>
      </div>
      <div class="lc-feature-card">
        <div class="lc-feature-icon"><i class="fa-solid fa-award"></i></div>
        <h3>兩週 14 天安心保固</h3>
        <p>每次清洗皆由客戶現場檢查驗收，完工後更享有長達兩週（14天）的售後服務保固，洗後有問題隨時處理。</p>
      </div>
    </div>
  </section>

  <!-- 六大服務項目 -->
  <div class="lc-bg-soft">
    <section class="lc-section">
      <h2 class="lc-title">全方位深層清潔服務方案</h2>
      <p class="lc-subtitle">
        同戶（同一門牌地址）多台設備同時預約享組合優惠價（各戶獨立計算），歡迎居家與商辦企業預約諮詢
      </p>
      <div class="lc-services">
        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-snowflake"></i></div>
          <h3>冷氣深度清潔</h3>
          <span class="lc-tag">分離式 / 窗型 / 吊隱式 / 四方吹</span>
          <p>深層拆洗散熱鰭片、風鼓與排水盤，徹底清除內部黑黴與果凍狀污垢，解決冷氣滴水、酸臭異味並大幅提升冷房省電效率。</p>
        </div>

        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-soap"></i></div>
          <h3>洗衣機完全拆洗</h3>
          <span class="lc-tag">直立式洗衣機 / 滾筒式洗衣機</span>
          <p>專業拆解內外筒與底盤，以高壓水柱徹底刷洗夾層長年累積的頑固污垢、海苔狀棉絮與皂垢殘留，避免衣物二次污染。</p>
        </div>

        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-bed"></i></div>
          <h3>床墊除蟎深層清潔</h3>
          <span class="lc-tag">高溫噴抽水洗 / 深層除蟎去污</span>
          <p>採用高溫噴抽水洗技術，深入床墊拔除陳年汗漬、尿漬、黃斑與塵蟎過敏原，搭配 Dri-Eaz 專業蝸牛風機快速吹乾。</p>
        </div>

        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-couch"></i></div>
          <h3>布沙發深層清潔</h3>
          <span class="lc-tag">高溫抽取式水洗 / 各類布質沙發</span>
          <p>針對布質纖維進行高溫抽取水洗，有效分解食物醬汁、寵物尿漬、汗垢與異味，恢復沙發蓬鬆清爽觸感。</p>
        </div>

        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-fan"></i></div>
          <h3>抽油煙機拆洗</h3>
          <span class="lc-tag">機體與風輪專業拆解去油</span>
          <p>針對抽油煙機內部風輪（葉輪）、集油槽與機體陳年厚重油垢進行深層拆解去油，恢復強勁吸力並維護廚房安全。</p>
        </div>

        <div class="lc-service-card">
          <div class="lc-service-icon"><i class="fa-solid fa-wind"></i></div>
          <h3>浴室排風扇 / 暖風機清潔</h3>
          <span class="lc-tag">防潮除黴 / 恢復換氣效率</span>
          <p>細部拆洗面板與內部風扇葉片，徹底清除潮濕環境積累的黑黴與厚重灰塵毛屑，維持衛浴空間空氣流通乾爽。</p>
        </div>
      </div>
    </section>
  </div>

  <!-- 客戶好評見證 -->
  <section class="lc-section">
    <h2 class="lc-title">雙北與桃園客戶真實好評</h2>
    <p class="lc-subtitle">來自家庭主婦、上班族與商業空間客戶的親身分享</p>
    <div class="lc-reviews">
      <div class="lc-review-card">
        <div class="lc-stars"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
        <p>「冷氣跟滾筒洗衣機洗完像新的一樣！施工前防護膠帶貼得非常仔細，地板完全沒弄髒，小林先生專業又客氣，大推！」</p>
        <div class="lc-reviewer">— 新北土城 王小姐（家庭主婦）</div>
      </div>
      <div class="lc-review-card">
        <div class="lc-stars"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
        <p>「家裡布沙發跟床墊被小孩弄髒，經過高溫水洗跟蝸牛風機吹乾後，異味跟污漬完全消失，晚上睡覺也不再一直打噴嚏了！」</p>
        <div class="lc-reviewer">— 新北板橋 陳女士（上班族）</div>
      </div>
      <div class="lc-review-card">
        <div class="lc-stars"><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i></div>
        <p>「公司辦公室的吊隱式與四方吹冷氣交給樂澄處理，動作俐落、不抽菸不吃檳榔，洗後冷房效果明顯變強，每年固定回訪！」</p>
        <div class="lc-reviewer">— 台北商辦 林經理（企業客戶）</div>
      </div>
    </div>
  </section>

  <!-- 聯絡資訊與新北土城地圖 -->
  <section class="lc-section" style="padding-top: 20px;">
    <div class="lc-contact-grid">
      <div class="lc-contact-info">
        <h3>聯絡樂澄專業清洗</h3>
        <div class="lc-info-item">
          <i class="fa-solid fa-user-check"></i>
          <div><strong>負責人：</strong>小林先生（樂澄專業清洗企業社）</div>
        </div>
        <div class="lc-info-item">
          <i class="fa-brands fa-line"></i>
          <div><strong>官方 LINE 預約：</strong>@749rgenw（點擊下方按鈕直接加入）</div>
        </div>
        <div class="lc-info-item">
          <i class="fa-solid fa-map-location-dot"></i>
          <div><strong>服務區域：</strong>新北市（土城、板橋、中和、永和、三峽、樹林、新莊、蘆洲等全區）、台北市全區、桃園市</div>
        </div>
        <div class="lc-info-item">
          <i class="fa-solid fa-building"></i>
          <div><strong>服務對象：</strong>一般家庭住宅、商業辦公室、補習班、幼兒園、政府機關、渡假飯店專案合作</div>
        </div>
        <div style="margin-top: 28px;">
          <a href="https://line.me/R/ti/p/@749rgenw" target="_blank" class="lc-btn-line" style="width: 100%; justify-content: center;">
            <i class="fa-brands fa-line fa-lg"></i> 點此加 LINE 傳照片免費估價
          </a>
        </div>
      </div>
      <div class="lc-map">
        <iframe src="https://www.google.com/maps?q=新北市土城區青雲路&output=embed" allowfullscreen="" loading="lazy"></iframe>
      </div>
    </div>
  </section>

  <!-- 頁尾 -->
  <footer class="lc-footer">
    <p><strong>樂澄專業清洗企業社</strong>｜冷氣清洗・洗衣機拆洗・床墊沙發水洗除蟎・抽油煙機清洗・浴室排風扇清潔</p>
    <p style="margin-top: 8px;">服務地區：新北市・台北市・桃園市 ｜ 官方 LINE：@749rgenw ｜ Copyright © 2026 樂澄專業清洗企業社 版權所有</p>
  </footer>
</div>
