<!doctype html>
<html lang="tr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Doğa ve Yaşam Derneği — Samsun</title>
  <meta name="description" content="Doğa ve Yaşam Derneği; Türkiye’nin yaban hayatını ve yaşam alanlarını korumak, bilimsel araştırma, eğitim ve farkındalık çalışmaları yürütür." />
  <meta property="og:title" content="Doğa ve Yaşam Derneği — Samsun" />
  <meta property="og:description" content="Türkiye’nin yaban hayatını ve yaşam alanlarını korumak için çalışan sivil toplum kuruluşu." />
  <meta property="og:type" content="website" />
  <meta property="og:locale" content="tr_TR" />
  <link rel="icon" href="/favicon.ico" />
  <style>
    :root {
      --yesil-koyu: #085f3b;
      --yesil-acik: #1f9d55;
      --krem: #f5f5f0;
      --gri-koyu: #2f3b4c;
      --beyaz: #ffffff;
    }

    /* Basic reset + accessible skip link */
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif; }
    body { background: #f2f5f4; color: var(--gri-koyu); line-height: 1.6; }
    a { color: inherit; text-decoration: none; }
    .skip-link {
      position: absolute; left: -999px; top: auto; width: 1px; height: 1px; overflow: hidden;
    }
    .skip-link:focus {
      position: static; width: auto; height: auto; padding: 0.5rem 0.75rem; background: #000; color: #fff; border-radius: 6px; z-index: 999;
    }

    /* NAVBAR */
    header { position: sticky; top: 0; z-index: 50; background: rgba(8, 95, 59, 0.96); backdrop-filter: blur(6px); color: var(--beyaz); box-shadow: 0 2px 8px rgba(0,0,0,.2); }
    .nav { max-width: 1100px; margin: 0 auto; display:flex; align-items:center; justify-content:space-between; padding:0.6rem 1rem; }
    .nav-logo { display:flex; align-items:center; gap:0.5rem; font-weight:700; letter-spacing:0.04em; }
    .nav-logo-icon { width:34px; height:34px; border-radius:50%; border:2px solid var(--yesil-acik); display:flex; align-items:center; justify-content:center; font-size:18px; background: rgba(255,255,255,0.1); }
    .nav-logo img { display:block; max-width:34px; height:34px; border-radius:50%; }
    .nav-links { display:flex; gap:1rem; font-size:0.95rem; }
    .nav-links a { padding:0.3rem 0.6rem; border-radius:999px; transition: background .2s, transform .1s; }
    .nav-links a:hover { background: rgba(255,255,255,0.16); transform: translateY(-1px); }

    /* HERO */
    .hero { background: radial-gradient(circle at top left, #1f9d55 0, #085f3b 45%, #052b19 100%); color: var(--beyaz); padding:3.5rem 1.25rem 3rem; }
    .hero-inner { max-width:1100px; margin:0 auto; display:grid; grid-template-columns: minmax(0,2.1fr) minmax(0,1.4fr); gap:2.5rem; align-items:center; }
    @media (max-width:800px) { .hero-inner { grid-template-columns:1fr; text-align:center; } }
    .hero-title { font-size:clamp(1.9rem,3vw + 1rem,2.6rem); margin-bottom:0.75rem; font-weight:800; }
    .hero-subtitle { font-size:1.05rem; max-width:520px; opacity:0.95; margin:0 auto 0; }
    .hero-badges { margin:1.5rem 0; display:flex; flex-wrap:wrap; gap:0.5rem; justify-content:flex-start; }
    @media (max-width:800px) { .hero-badges { justify-content:center; } }
    .badge { font-size:0.8rem; padding:0.25rem 0.7rem; border-radius:999px; border:1px solid rgba(255,255,255,0.3); background: rgba(0,0,0,0.12); text-transform:uppercase; letter-spacing:0.06em; }
    .hero-actions { display:flex; flex-wrap:wrap; gap:0.8rem; margin-top:0.5rem; }
    @media (max-width:800px) { .hero-actions { justify-content:center; } }
    .btn { border-radius:999px; padding:0.6rem 1.1rem; font-size:0.95rem; border:none; cursor:pointer; display:inline-flex; align-items:center; gap:0.4rem; font-weight:600; transition: transform .1s ease, box-shadow .1s ease, background .2s ease; }
    .btn-primary { background:var(--beyaz); color:var(--yesil-koyu); box-shadow: 0 6px 18px rgba(0,0,0,.25); }
    .btn-primary:hover { transform: translateY(-1px); box-shadow:0 10px 30px rgba(0,0,0,.35); }
    .btn-outline { background:transparent; color:var(--beyaz); border:1px solid rgba(255,255,255,0.55); }
    .btn-outline:hover { background: rgba(0,0,0,0.1); transform: translateY(-1px); }
    .hero-card { background: rgba(245,245,240,0.98); color:var(--gri-koyu); border-radius:18px; padding:1.4rem 1.5rem; box-shadow:0 20px 40px rgba(0,0,0,.25); }

    /* MAIN */
    main { max-width:1100px; margin:0 auto; padding:2rem 1.25rem 3rem; }
    section { margin-bottom:2.8rem; }
    .section-title { font-size:1.5rem; margin-bottom:0.75rem; color:var(--yesil-koyu); display:inline-flex; align-items:center; gap:0.4rem; }
    .section-subtitle { font-size:0.98rem; color:#4b5563; margin-bottom:1.3rem; max-width:620px; }
    .grid-2 { display:grid; grid-template-columns: minmax(0,1.5fr) minmax(0,1.3fr); gap:1.8rem; }
    @media (max-width:900px) { .grid-2 { grid-template-columns:1fr; } }
    .card { background:var(--beyaz); border-radius:16px; padding:1.3rem 1.4rem; box-shadow:0 8px 22px rgba(15,23,42,0.12); }
    table { width:100%; border-collapse:collapse; font-size:0.9rem; }
    th, td { padding:0.5rem 0.65rem; border-bottom:1px solid #e5e7eb; text-align:left; }
    th { background:#e5f3eb; color:#064e3b; font-weight:600; font-size:0.86rem; text-transform:uppercase; letter-spacing:0.04em; }
    tr:nth-child(even) td { background:#f9fafb; }
    .tag { display:inline-block; padding:0.2rem 0.5rem; border-radius:999px; font-size:0.75rem; background:#ecfdf5; color:#166534; border:1px solid #bbf7d0; }

    /* TUZUK / DOWNLOAD */
    .download-buttons { display:flex; flex-wrap:wrap; gap:0.8rem; margin-top:0.8rem; }
    .btn-ghost { border-radius:999px; padding:0.5rem 0.9rem; font-size:0.9rem; border:1px solid #d1d5db; background:#ffffff; display:inline-flex; align-items:center; gap:0.4rem; cursor:pointer; transition: background .15s, transform .1s, box-shadow .1s; }
    .btn-ghost:hover { background:#f3f4f6; transform: translateY(-1px); box-shadow:0 4px 12px rgba(148,163,184,.4); }

    /* CONTACT */
    .contact-grid { display:grid; grid-template-columns:minmax(0,1.4fr) minmax(0,1.2fr); gap:1.5rem; align-items:flex-start; }
    @media (max-width:850px) { .contact-grid { grid-template-columns:1fr; } }
    .contact-item { margin-bottom:0.4rem; font-size:0.95rem; }
    .contact-label { font-weight:600; color:#374151; margin-right:0.4rem; }
    .contact-form { display:grid; gap:0.7rem; }
    .contact-form label { font-size:0.85rem; font-weight:600; color:#374151; margin-bottom:0.15rem; display:inline-block; }
    .contact-form input, .contact-form textarea { width:100%; padding:0.55rem 0.7rem; border-radius:10px; border:1px solid #d1d5db; font-size:0.9rem; resize:vertical; }
    .contact-form input:focus, .contact-form textarea:focus { outline:2px solid #a7f3d0; border-color:#34d399; }

    /* FOOTER */
    footer { background:#012315; color:#d1fae5; padding:1.2rem 1.25rem 1.5rem; font-size:0.8rem; }
    .footer-inner { max-width:1100px; margin:0 auto; display:flex; flex-wrap:wrap; justify-content:space-between; gap:0.6rem; align-items:center; }
    .sr-only { position:absolute; left:-9999px; width:1px; height:1px; overflow:hidden; }
  </style>
</head>
<body>
  <a class="skip-link" href="#main">İçeriğe atla</a>

  <!-- NAVBAR -->
  <header role="banner">
    <nav class="nav" role="navigation" aria-label="Ana navigasyon">
      <div class="nav-logo" aria-hidden="false">
        <div class="nav-logo-icon" aria-hidden="true">🌿</div>
        <div>
          <div>Doğa ve Yaşam Derneği</div>
          <small style="font-weight:400; opacity:0.8;">Samsun</small>
        </div>
      </div>
      <div class="nav-links">
        <a href="#hakkimizda">Hakkımızda</a>
        <a href="#tuzuk">Tüzük</a>
        <a href="#yonetim">Yönetim</a>
        <a href="#uyelik">Üyelik</a>
        <a href="#iletisim">İletişim</a>
      </div>
    </nav>
  </header>

  <!-- HERO -->
  <main id="main" role="main">
    <section class="hero" aria-labelledby="hero-title">
      <div class="hero-inner">
        <div>
          <h1 id="hero-title" class="hero-title">Türkiye’nin Yaban Hayatını ve Yaşam Alanlarını Korumak İçin Birlikteyiz.</h1>
          <p class="hero-subtitle">
            Doğa ve Yaşam Derneği, ülkemizin yabanî canlı türlerini ve yaşam alanlarını
            korumak, iyileştirmek ve sürekliliğini sağlamak amacıyla çalışan bir sivil toplum
            kuruluşudur.
          </p>

          <div class="hero-badges" aria-hidden="true">
            <span class="badge">Yaban hayatı</span>
            <span class="badge">Ekosistem koruma</span>
            <span class="badge">Bilimsel araştırma</span>
            <span class="badge">Eğitim ve farkındalık</span>
          </div>

          <div class="hero-actions">
            <a href="#uyelik" class="btn btn-primary" aria-label="Üye ol ve destek ver">Üye Ol &amp; Destek Ver</a>
            <a href="#tuzuk" class="btn btn-outline" aria-label="Tüzüğü görüntüle">Tüzüğü Görüntüle</a>
          </div>
        </div>

        <aside class="hero-card" aria-labelledby="calisma-baslik" role="complementary">
          <h3 id="calisma-baslik">Çalışma Alanlarımız</h3>
          <p>Doğa ve Yaşam Derneği olarak:</p>
          <ul>
            <li>Yabanî canlı türleri ve yaşam alanları üzerine bilimsel çalışmalar yürütürüz.</li>
            <li>Soyları tehlike altındaki türler için eylem planları hazırlarız.</li>
            <li>Koruma projeleri, eğitim ve topluluk çalışmaları yürütürüz.</li>
          </ul>
        </aside>
      </div>
    </section>

    <!-- HAKKIMIZDA -->
    <section id="hakkimizda" aria-labelledby="hakkimizda-baslik">
      <h2 id="hakkimizda-baslik" class="section-title">Hakkımızda</h2>
      <p class="section-subtitle">Doğa ve Yaşam Derneği, çevresel koruma ve yaban hayatı için çalışmalar yapar; yerel toplulukları güçlendirir ve bilimsel yaklaşımla projeler yürütür.</p>

      <div class="grid-2">
        <div class="card">
          <h3>Misyon</h3>
          <p>Ülkemizde yaban hayatını ve doğal yaşam alanlarını korumak, gelecek nesillere sağlıklı bir çevre bırakmak.</p>
        </div>

        <div class="card">
          <h3>Vizyon</h3>
          <p>Sürdürülebilir koruma modelleri ve topluluk tabanlı çalışmalarda öncü bir sivil toplum kuruluşu olmak.</p>
        </div>
      </div>
    </section>

    <!-- TUZUK -->
    <section id="tuzuk" aria-labelledby="tuzuk-baslik">
      <h2 id="tuzuk-baslik" class="section-title">Tüzük</h2>
      <p class="section-subtitle">Derneğimizin temel tüzük belgeleri aşağıdan indirilebilir.</p>

      <div class="card">
        <p>Dernek tüzüğü ve diğer resmi belgeler:</p>
        <div class="download-buttons" role="list">
          <a class="btn-ghost" role="listitem" href="/files/tuzuk.pdf" download>Dernek Tüzüğü (PDF)</a>
          <a class="btn-ghost" role="listitem" href="/files/faaliyet_raporu.pdf" download>Faaliyet Raporu (PDF)</a>
        </div>
      </div>
    </section>

    <!-- YÖNETİM -->
    <section id="yonetim" aria-labelledby="yonetim-baslik">
      <h2 id="yonetim-baslik" class="section-title">Yönetim Kurulu</h2>
      <p class="section-subtitle">Yönetim kurulu üyelerimiz ve görevleri.</p>

      <div class="card">
        <table aria-describedby="yonetim-aciklama">
          <caption id="yonetim-aciklama" class="sr-only">Yönetim kurulu üyeleri</caption>
          <thead>
            <tr><th>İsim</th><th>Görev</th><th>İletişim</th></tr>
          </thead>
          <tbody>
            <tr><td>Ahmet Yılmaz</td><td>Başkan</td><td><a href="mailto:ahmet@example.org">ahmet@example.org</a></td></tr>
            <tr><td>Mehmet Kaya</td><td>Başkan Yardımcısı</td><td><a href="mailto:mehmet@example.org">mehmet@example.org</a></td></tr>
          </tbody>
        </table>
      </div>
    </section>

    <!-- UYELIK -->
    <section id="uyelik" aria-labelledby="uyelik-baslik">
      <h2 id="uyelik-baslik" class="section-title">Üyelik &amp; Destek</h2>
      <p class="section-subtitle">Derneğimize üye olabilir veya bağış yaparak projelerimize destek olabilirsiniz.</p>

      <div class="grid-2">
        <div class="card">
          <h3>Nasıl Üye Olurum?</h3>
          <p>Üyelik formunu doldurarak ve aidatınızı yatırarak üye olabilirsiniz. Üyelik başvuru formu yakında burada olacak.</p>
        </div>

        <div class="card">
          <h3>Bağış</h3>
          <p>Bağış ve sponsorluk bilgileri için lütfen iletişime geçin.</p>
        </div>
      </div>
    </section>

    <!-- İLETİŞİM -->
    <section id="iletisim" aria-labelledby="iletisim-baslik">
      <h2 id="iletisim-baslik" class="section-title">İletişim</h2>
      <p class="section-subtitle">Bize ulaşmak için aşağıdaki kanalları kullanabilirsiniz.</p>

      <div class="contact-grid">
        <div>
          <p class="contact-item"><span class="contact-label">Adres:</span> Örnek Mah. Doğa Cad. No:1, Samsun</p>
          <p class="contact-item"><span class="contact-label">E-posta:</span> <a href="mailto:info@dogaveyasam.org">info@dogaveyasam.org</a></p>
          <p class="contact-item"><span class="contact-label">Telefon:</span> +90 362 000 0000</p>
        </div>

        <form class="contact-form card" action="#" method="post" aria-label="İletişim formu">
          <label for="name">İsim</label>
          <input id="name" name="name" type="text" placeholder="Adınız" required />

          <label for="email">E-posta</label>
          <input id="email" name="email" type="email" placeholder="you@example.com" required />

          <label for="message">Mesaj</label>
          <textarea id="message" name="message" rows="5" placeholder="Mesajınızı yazın..." required></textarea>

          <div style="display:flex; gap:0.6rem; margin-top:0.4rem;">
            <button type="submit" class="btn btn-primary">Gönder</button>
            <a href="mailto:info@dogaveyasam.org" class="btn btn-outline">E-posta ile Gönder</a>
          </div>
        </form>
      </div>
    </section>
  </main>

  <footer role="contentinfo">
    <div class="footer-inner">
      <div>© <span id="year"></span> Doğa ve Yaşam Derneği — Tüm hakları saklıdır.</div>
      <div><a href="#iletisim">İletişim</a> · <a href="#tuzuk">Tüzük</a></div>
    </div>
  </footer>

  <script>
    // Set copyright year
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>