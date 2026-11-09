<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>MohaPhoto | Edición de Fotos y Diseño Gráfico Profesional</title>

  <meta name="description" content="Servicio profesional de edición de fotos, retoque fotográfico, eliminación de fondos, diseño de logotipos, flyers y diseño gráfico personalizado.">
  <meta name="robots" content="index, follow">
  <link rel="canonical" href="https://mohamedsali4000-a11y.github.io/Mohaphotoshop/">
  <meta property="og:title" content="MohaPhoto - Edición de Fotos y Diseño Gráfico">
  <meta property="og:description" content="Transformamos tus ideas en diseños increíbles.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://mohamedsali4000-a11y.github.io/Mohaphotoshop/">

  <style>
    :root{
      --bg:#f6f7fb;
      --white:#ffffff;
      --ink:#201d2f;
      --muted:#625f7a;
      --line:#e9e8f1;
      --primary:#5d4bd1;
      --primary-2:#7d68f7;
      --accent:#ff8d5d;
      --green:#1fa86d;
      --shadow:0 18px 48px rgba(26,22,50,.10);
      --radius:20px;
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family: Arial, Helvetica, sans-serif;
      background:var(--bg);
      color:var(--ink);
      line-height:1.7;
    }

    a{color:inherit;text-decoration:none}
    img{display:block;max-width:100%}
    button,select{font:inherit}
    :focus-visible{
      outline:3px solid #ffc857;
      outline-offset:3px;
    }

    .container{
      width:min(1120px, 92%);
      margin:0 auto;
    }

    .sr-only{
      position:absolute; width:1px; height:1px; padding:0; margin:-1px;
      overflow:hidden; clip:rect(0,0,0,0); white-space:nowrap; border:0;
    }

    .skip{
      position:absolute;
      top:-52px;
      inset-inline-start:14px;
      background:#fff;
      padding:10px 14px;
      border-radius:10px;
      z-index:50;
    }
    .skip:focus{top:14px}

    header{
      position:sticky;
      top:0;
      z-index:30;
      background: rgba(255,255,255,.88);
      backdrop-filter: blur(12px);
      border-bottom:1px solid var(--line);
    }

    .nav{
      display:flex;
      align-items:center;
      justify-content:space-between;
      min-height:72px;
      gap:16px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:12px;
      font-weight:800;
      font-size:1.1rem;
    }

    .brand-mark{
      width:42px; height:42px;
      border-radius:14px;
      display:grid; place-items:center;
      color:#fff;
      font-weight:900;
      background:linear-gradient(135deg, var(--primary), var(--accent));
      box-shadow:0 12px 24px rgba(93,75,209,.26);
    }

    .nav-group{
      display:flex;
      align-items:center;
      gap:18px;
      flex-wrap:wrap;
    }

    .nav-links{
      display:flex;
      gap:18px;
      color:var(--muted);
      font-size:14px;
    }

    .lang-select{
      background:#fff;
      border:1px solid var(--line);
      border-radius:10px;
      padding:10px 12px;
      min-width:120px;
    }

    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:8px; padding:12px 18px; border:0; border-radius:12px;
      cursor:pointer; font-weight:700; transition:.2s ease;
      text-decoration:none;
    }

    .btn:hover{transform:translateY(-1px)}
    .btn.primary{
      background:linear-gradient(135deg, var(--primary), var(--primary-2));
      color:#fff;
      box-shadow:0 12px 25px rgba(93,75,209,.20);
    }
    .btn.outline{
      background:#fff;border:1px solid var(--line);color:var(--ink);
    }
    .btn.green{
      background:var(--green);color:#fff;
    }
    .btn.light{
      background:rgba(255,255,255,.85); border:1px solid var(--line);
      color:var(--ink);
    }

    .hero{
      padding:72px 0 58px;
      background:
        radial-gradient(circle at 15% 15%, rgba(125,104,247,.20), transparent 28%),
        radial-gradient(circle at 85% 30%, rgba(255,141,93,.18), transparent 28%),
        linear-gradient(135deg, #fffefb 0%, #f8f7fd 100%);
    }

    .hero-grid{
      display:grid;
      grid-template-columns:1.15fr .85fr;
      gap:28px;
      align-items:center;
    }

    .tag{
      display:inline-block;
      background:#eeeaff;
      color:#4c3fd3;
      padding:8px 14px;
      border-radius:999px;
      font-size:13px;
      font-weight:700;
    }

    h1{
      margin:18px 0 14px;
      font-size: clamp(34px, 5vw, 60px);
      line-height:1.12;
      letter-spacing:-1.5px;
    }

    .hero p{
      margin:0;
      font-size:17px;
      color:var(--muted);
      max-width:560px;
      line-height:1.9;
    }

    .hero-actions{
      display:flex; flex-wrap:wrap; gap:12px;
      margin-top:24px;
    }

    .hero-photo-wrap{
      position:relative; display:grid; place-items:center;
      min-height:360px;
    }

    .hero-glow{
      position:absolute; width:300px; height:300px; border-radius:50%;
      background:linear-gradient(135deg, rgba(93,75,209,.22), rgba(255,141,93,.22));
      filter:blur(4px);
    }

    .hero-photo{
      position:relative;
      width:min(100%, 430px);
      height:360px;
      object-fit:cover;
      border-radius:28px;
      box-shadow:var(--shadow);
      border:1px solid rgba(255,255,255,.35);
    }

    section{
      padding:56px 0;
    }

    .heading{
      margin-bottom:18px;
    }

    .heading h2{
      margin:0 0 8px;
      font-size:clamp(28px, 3vw, 40px);
    }

    .heading p{
      margin:0;
      color:var(--muted);
      line-height:1.8;
      max-width:700px;
    }

    .services-grid{
      display:grid; grid-template-columns:repeat(3, minmax(0,1fr)); gap:18px;
    }

    .card{
      background:#fff;
      border:1px solid var(--line);
      border-radius:var(--radius);
      overflow:hidden;
      box-shadow:0 8px 22px rgba(21,17,36,.03);
    }

    .card img{
      width:100%; height:220px; object-fit:cover;
    }

    .card-body{
      padding:18px;
    }

    .card h3{
      margin:0 0 8px;
      font-size:22px;
    }

    .card p{
      margin:0 0 12px;
      color:var(--muted);
      line-height:1.7;
      font-size:14px;
    }

    .price{
      font-size:20px; font-weight:800;
    }

    .portfolio-grid{
      display:grid;
      grid-template-columns:repeat(3, minmax(0,1fr)); gap:18px;
    }

    .portfolio-item{
      position:relative;
      overflow:hidden;
      border-radius:var(--radius);
      height:280px;
      border:1px solid var(--line);
    }

    .portfolio-item img{
      width:100%; height:100%; object-fit:cover;
      transition:.35s ease;
    }

    .portfolio-item:hover img{
      transform:scale(1.05);
    }

    .overlay{
      position:absolute; inset:0;
      display:flex; align-items:end; padding:16px;
      background:linear-gradient(180deg, transparent 20%, rgba(17,16,27,.6) 100%);
      color:#fff;
      font-weight:700;
    }

    .process{
      display:grid; grid-template-columns:repeat(4, minmax(0,1fr)); gap:18px;
    }

    .step{
      background:#fff; border:1px solid var(--line);
      border-radius:18px; padding:22px 18px;
    }

    .step-badge{
      width:42px; height:42px; display:grid; place-items:center;
      background:#f0ebff; color:var(--primary); border-radius:12px; font-weight:800;
      margin-bottom:12px;
    }

    .stats{
      display:grid; grid-template-columns:repeat(3, minmax(0,1fr)); gap:18px;
      margin-top:18px;
    }

    .stat{
      background:#fff; border:1px solid var(--line); border-radius:18px; padding:24px 18px; text-align:center;
    }
    .stat strong{
      display:block; font-size:28px; margin-bottom:4px;
    }
    .stat span{
      color:var(--muted); font-size:14px;
    }

    .cta{
      padding:28px 30px; border-radius:24px;
      background:linear-gradient(135deg, #231f35, #503ecb);
      color:#fff;
      display:flex; align-items:center; justify-content:space-between; gap:18px;
      box-shadow:0 18px 50px rgba(39,32,73,.18);
    }

    .cta h3{margin:0 0 6px;font-size:clamp(24px,3vw,34px)}
    .cta p{margin:0;color:#e1dcff;line-height:1.7}

    .contact-grid{
      display:grid; grid-template-columns:1.1fr .9fr; gap:18px;
    }

    .contact-box, .form-box{
      background:#fff; border:1px solid var(--line); border-radius:20px; padding:22px;
    }

    .contact-box{
      display:flex; flex-direction:column; gap:14px;
    }

    .contact-item{
      display:flex; align-items:flex-start; gap:12px;
      padding:14px 12px; border:1px solid var(--line); border-radius:14px;
      background:#faf9ff;
    }

    .icon{
      width:42px; height:42px; display:grid; place-items:center; border-radius:12px;
      background:#f0ebff; color:var(--primary); font-size:20px; font-weight:700;
    }

    .form-box form{
      display:grid; gap:14px;
    }

    .input, .textarea{
      width:100%; border:1px solid var(--line); background:#fff;
      border-radius:12px; padding:12px 14px; font:inherit; color:var(--ink);
    }
    .textarea{min-height:120px; resize:vertical}

    footer{
      padding:22px 0 34px; color:var(--muted); text-align:center;
      font-size:13px;
    }

    @media (max-width: 760px){
      .nav-links{display:none}
      .nav{min-height:64px}
      .hero-grid, .services-grid, .portfolio-grid, .process, .stats, .contact-grid{
        grid-template-columns:1fr;
      }
      .hero{padding-top:48px}
      .hero-photo{height:280px}
      .cta{flex-direction:column; align-items:flex-start}
    }
  </style>
</head>
<body>
  <a class="skip" href="#main-content">تجاوز إلى المحتوى</a>

  <header>
    <div class="container nav">
      <a class="brand" href="#" aria-label="MohaPhoto home">
        <span class="brand-mark">M</span>
        <span>MohaPhoto</span>
      </a>

      <div class="nav-group">
        <nav class="nav-links" aria-label="Main navigation">
          <a href="#services" data-i18n="navServices">الخدمات</a>
          <a href="#portfolio" data-i18n="navPortfolio">الأعمال</a>
          <a href="#process" data-i18n="navProcess">العملية</a>
          <a href="#contact" data-i18n="navContact">تواصل</a>
        </nav>

        <label class="sr-only" for="languageSelect">Language</label>
        <select id="languageSelect" class="lang-select" aria-label="Select language">
          <option value="ar">العربية</option>
          <option value="es">Español</option>
          <option value="en">English</option>
        </select>

        <a class="btn primary" href="#contact" data-i18n="navCta">طلب تصميم</a>
      </div>
    </div>
  </header>

  <main id="main-content">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="tag">MohaPhoto • Photo Editing</span>
          <h1 data-i18n="heroTitle">نحوّل الصور إلى أعمال احترافية</h1>
          <p data-i18n="heroText">
            نقدم خدمات تحرير الصور، إزالة الخلفية، تصميم الشعارات، البروشورات، والهوية البصرية
            لكل المشاريع الشخصية والتجارية.
          </p>

          <div class="hero-actions">
            <a class="btn primary" href="#contact" data-i18n="heroBtnPrimary">احجز الآن</a>
            <a class="btn outline" href="#portfolio" data-i18n="heroBtnSecondary">معرض الأعمال</a>
          </div>
        </div>

        <div class="hero-photo-wrap">
          <div class="hero-glow" aria-hidden="true"></div>
          <img
            class="hero-photo"
            src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1200&q=85"
            alt="Professional photo editing workspace"
          />
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <div class="heading">
          <h2 data-i18n="servicesTitle">خدماتنا الاحترافية</h2>
          <p data-i18n="servicesText">
            نساعدكَ في تحويل الصور إلى قطع جذابة ومهنية تناسب علامتك التجارية أو مشروعك الشخصي.
          </p>
        </div>

        <div class="services-grid">
          <article class="card">
            <img src="https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?auto=format&fit=crop&w=900&q=85" alt="retouch photo">
            <div class="card-body">
              <h3 data-i18n="service1Title">تعديل الصور</h3>
              <p data-i18n="service1Text">تجميل البشرة، إزالة العيوب، تعديل الألوان، وأجواء احترافية لكل الصور.</p>
              <span class="price" data-i18n="service1Price">من 20€</span>
            </div>
          </article>

          <article class="card">
            <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=900&q=85" alt="graphic design">
            <div class="card-body">
              <h3 data-i18n="service2Title">تصميم جرافيكي</h3>
              <p data-i18n="service2Text">تصميم لوجو، منشورات، بطاقات أعمال، وبروشورات بشكل أنيق واحترافي.</p>
              <span class="price" data-i18n="service2Price">من 30€</span>
            </div>
          </article>

          <article class="card">
            <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&w=900&q=85" alt="background removal">
            <div class="card-body">
              <h3 data-i18n="service3Title">إزالة الخلفية</h3>
              <p data-i18n="service3Text">تحويل الصور إلى صور جاهزة للمنتجات، السوشال ميديا، أو المتاجر الإلكترونية.</p>
              <span class="price" data-i18n="service3Price">من 10€</span>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section id="portfolio">
      <div class="container">
        <div class="heading">
          <h2 data-i18n="portfolioTitle">معرض الأعمال</h2>
          <p data-i18n="portfolioText">أمثلة على تصميماتنا وفيديوهات/صور نهتم بتقديمها بمستوى احترافي.</p>
        </div>

        <div class="portfolio-grid">
          <div class="portfolio-item">
            <img src="https://images.unsplash.com/photo-1521572267360-ee0c2909d518?auto=format&fit=crop&w=900&q=85" alt="portfolio item 1">
            <div class="overlay" data-i18n="work1">تصميم علامة تجارية</div>
          </div>

          <div class="portfolio-item">
            <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?auto=format&fit=crop&w=900&q=85" alt="portfolio item 2">
            <div class="overlay" data-i18n="work2">بروشور تسويقي</div>
          </div>

          <div class="portfolio-item">
            <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=900&q=85" alt="portfolio item 3">
            <div class="overlay" data-i18n="work3">محتوى سوشال ميديا</div>
          </div>
        </div>
      </div>
    </section>

    <section id="process">
      <div class="container">
        <div class="heading">
          <h2 data-i18n="processTitle">كيف نشتغل؟</h2>
          <p data-i18n="processText">نحافظ على سهولة التواصل وسرعة التنفيذ مع الجودة العالية.</p>
        </div>

        <div class="process">
          <div class="step">
            <div class="step-badge">1</div>
            <h3 data-i18n="step1Title">تحديد الطلب</h3>
            <p data-i18n="step1Text">نراجع الفكرة أو الصورة أو النمط المطلوب.</p>
          </div>

          <div class="step">
            <div class="step-badge">2</div>
            <h3 data-i18n="step2Title">التخطيط</h3>
            <p data-i18n="step2Text">نحدد الخيارات وتفاصيل التصميم المطلوبة.</p>
          </div>

          <div class="step">
            <div class="step-badge">3</div>
            <h3 data-i18n="step3Title">التنفيذ</h3>
            <p data-i18n="step3Text">نقوم بتعديل أو تصميم المخرجات احترافياً.</p>
          </div>

          <div class="step">
            <div class="step-badge">4</div>
            <h3 data-i18n="step4Title">التسليم</h3>
            <p data-i18n="step4Text">نقدّم النتيجة النهائية بصيغة مناسبة للتحميل.</p>
          </div>
        </div>

        <div class="stats">
          <div class="stat">
            <strong>500+</strong>
            <span data-i18n="stat1">مشروع تم إنجازه</span>
          </div>

          <div class="stat">
            <strong>24h</strong>
            <span data-i18n="stat2">متوسط الاستجابة</span>
          </div>

          <div class="stat">
            <strong>100%</strong>
            <span data-i18n="stat3">رضا العملاء</span>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="cta">
          <div>
            <h3 data-i18n="ctaTitle">جاهز تبدأ مشروعك التالي؟</h3>
            <p data-i18n="ctaText">تواصل معنا الآن للحصول على تصميم احترافي يلائم علامتك التجارية.</p>
          </div>
          <a class="btn green" href="https://wa.me/34666784846?text=Salam%2C%20bghit%20n3araf%20b7al%20service%20MohaPhoto" data-i18n="ctaBtn">تواصل عبر واتساب</a>
        </div>

        <div class="contact-grid" style="margin-top:22px;">
          <div class="contact-box">
            <div class="contact-item">
              <div class="icon">✉</div>
              <div>
                <strong data-i18n="contactEmailTitle">البريد الإلكتروني</strong>
                <div><a href="mailto:mohammedsalhi4000@gmail.com">mohammedsalhi4000@gmail.com</a></div>
              </div>
            </div>

            <div class="contact-item">
              <div class="icon">☏</div>
              <div>
                <strong data-i18n="contactPhoneTitle">واتساب</strong>
                <div><a href="https://wa.me/34666784846">+34 666 784 846</a></div>
              </div>
            </div>

            <div class="contact-item">
              <div class="icon">📍</div>
              <div>
                <strong data-i18n="contactLocationTitle">الموقع</strong>
                <div data-i18n="contactLocationText">برشلونة، إسبانيا</div>
              </div>
            </div>
          </div>

          <div class="form-box">
            <h3 data-i18n="formTitle">أرسل طلبك</h3>
            <form>
              <input class="input" type="text" placeholder="الاسم الكامل" data-i18n-placeholder="namePlaceholder" />
              <input class="input" type="email" placeholder="البريد الإلكتروني" data-i18n-placeholder="emailPlaceholder" />
              <textarea class="textarea" placeholder="اكتب مشروعك هنا..." data-i18n-placeholder="messagePlaceholder"></textarea>
              <button class="btn primary" type="button" data-i18n="formBtn">إرسال الطلب</button>
            </form>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    © 2026 MohaPhoto — Barcelona
  </footer>

  <script>
    const translations = {
      ar: {
        navServices: "الخدمات",
        navPortfolio: "الأعمال",
        navProcess: "العملية",
        navContact: "تواصل",
        navCta: "طلب تصميم",
        heroTitle: "نحوّل الصور إلى أعمال احترافية",
        heroText: "نقدم خدمات تحرير الصور، إزالة الخلفية، تصميم الشعارات، البروشورات، والهوية البصرية لكل المشاريع الشخصية والتجارية.",
        heroBtnPrimary: "احجز الآن",
        heroBtnSecondary: "معرض الأعمال",
        servicesTitle: "خدماتنا الاحترافية",
        servicesText: "نساعدكَ في تحويل الصور إلى قطع جذابة ومهنية تناسب علامتك التجارية أو مشروعك الشخصي.",
        service1Title: "تعديل الصور",
        service1Text: "تجميل البشرة، إزالة العيوب، تعديل الألوان، وأجواء احترافية لكل الصور.",
        service1Price: "من 20€",
        service2Title: "تصميم جرافيكي",
        service2Text: "تصميم لوجو، منشورات، بطاقات أعمال، وبروشورات بشكل أنيق واحترافي.",
        service2Price: "من 30€",
        service3Title: "إزالة الخلفية",
        service3Text: "تحويل الصور إلى صور جاهزة للمنتجات، السوشال ميديا، أو المتاجر الإلكترونية.",
        service3Price: "من 10€",
        portfolioTitle: "معرض الأعمال",
        portfolioText: "أمثلة على تصميماتنا وفيديوهات/صور نهتم بتقديمها بمستوى احترافي.",
        work1: "تصميم علامة تجارية",
        work2: "بروشور تسويقي",
        work3: "محتوى سوشال ميديا",
        processTitle: "كيف نشتغل؟",
        processText: "نحافظ على سهولة التواصل وسرعة التنفيذ مع الجودة العالية.",
        step1Title: "تحديد الطلب",
        step1Text: "نراجع الفكرة أو الصورة أو النمط المطلوب.",
        step2Title: "التخطيط",
        step2Text: "نحدد الخيارات وتفاصيل التصميم المطلوبة.",
        step3Title: "التنفيذ",
        step3Text: "نقوم بتعديل أو تصميم المخرجات احترافياً.",
        step4Title: "التسليم",
        step4Text: "نقدّم النتيجة النهائية بصيغة مناسبة للتحميل.",
        stat1: "مشروع تم إنجازه",
        stat2: "متوسط الاستجابة",
        stat3: "رضا العملاء",
        ctaTitle: "جاهز تبدأ مشروعك التالي؟",
        ctaText: "تواصل معنا الآن للحصول على تصميم احترافي يلائم علامتك التجارية.",
        ctaBtn: "تواصل عبر واتساب",
        contactEmailTitle: "البريد الإلكتروني",
        contactPhoneTitle: "واتساب",
        contactLocationTitle: "الموقع",
        contactLocationText: "برشلونة، إسبانيا",
        formTitle: "أرسل طلبك",
        formBtn: "إرسال الطلب",
        namePlaceholder: "الاسم الكامل",
        emailPlaceholder: "البريد الإلكتروني",
        messagePlaceholder: "اكتب مشروعك هنا..."
      },
      es: {
        navServices: "Servicios",
        navPortfolio: "Portafolio",
        navProcess: "Proceso",
        navContact: "Contacto",
        navCta: "Solicitar diseño",
        heroTitle: "Transformamos tus fotos en trabajos profesionales",
        heroText: "Ofrecemos edición de fotos, eliminación de fondos, diseño de logotipos, flyers y branding para proyectos personales y empresariales.",
        heroBtnPrimary: "Reservar ahora",
        heroBtnSecondary: "Ver portafolio",
        servicesTitle: "Nuestros servicios",
        servicesText: "Te ayudamos a convertir tus imágenes en piezas atractivas y profesionales que se adapten a tu marca.",
        service1Title: "Edición de fotos",
        service1Text: "Retocado de piel, corrección de color, limpieza y mejoras profesionales.",
        service1Price: "Desde 20€",
        service2Title: "Diseño gráfico",
        service2Text: "Logos, publicaciones, tarjetas de presentación y flyers con un estilo elegante.",
        service2Price: "Desde 30€",
        service3Title: "Eliminación de fondo",
        service3Text: "Preparamos tus imágenes para comercio, redes sociales y tiendas online.",
        service3Price: "Desde 10€",
        portfolioTitle: "Portafolio",
        portfolioText: "Ejemplos de trabajos y piezas visuales con un nivel profesional.",
        work1: "Diseño de marca",
        work2: "Flyer promocional",
        work3: "Contenido para redes",
        processTitle: "Cómo trabajamos",
        processText: "Mantener la comunicación fácil y la entrega rápida sin perder calidad.",
        step1Title: "Definición",
        step1Text: "Revisamos la idea, la imagen o el estilo requerido.",
        step2Title: "Planificación",
        step2Text: "Determinamos opciones y detalles del diseño.",
        step3Title: "Ejecución",
        step3Text: "Realizamos la edición o diseño profesionalmente.",
        step4Title: "Entrega",
        step4Text: "Entregamos el resultado final en formato listo para usar.",
        stat1: "proyectos completados",
        stat2: "respuesta promedio",
        stat3: "satisfacción",
        ctaTitle: "¿Listo para tu próximo proyecto?",
        ctaText: "Contáctanos para obtener un diseño profesional según tu marca.",
        ctaBtn: "Contactar por WhatsApp",
        contactEmailTitle: "Correo electrónico",
        contactPhoneTitle: "WhatsApp",
        contactLocationTitle: "Ubicación",
        contactLocationText: "Barcelona, España",
        formTitle: "Envíanos tu proyecto",
        formBtn: "Enviar solicitud",
        namePlaceholder: "Nombre completo",
        emailPlaceholder: "Correo electrónico",
        messagePlaceholder: "Escribe tu proyecto aquí..."
      },
      en: {
        navServices: "Services",
        navPortfolio: "Portfolio",
        navProcess: "Process",
        navContact: "Contact",
        navCta: "Request design",
        heroTitle: "Turn your photos into professional work",
        heroText: "We provide photo editing, background removal, logo design, flyers, and branding for personal and business projects.",
        heroBtnPrimary: "Book now",
        heroBtnSecondary: "Portfolio",
        servicesTitle: "Our services",
        servicesText: "We help turn your images into attractive, professional pieces that fit your brand and goals.",
        service1Title: "Photo editing",
        service1Text: "Skin retouching, color correction, blemish removal, and premium finishes.",
        service1Price: "From €20",
        service2Title: "Graphic design",
        service2Text: "Logos, posts, business cards, and brochures with a polished and elegant style.",
        service2Price: "From €30",
        service3Title: "Background removal",
        service3Text: "We prepare images for products, social media, and online stores.",
        service3Price: "From €10",
        portfolioTitle: "Portfolio",
        portfolioText: "Examples of our work and visual pieces delivered at a professional level.",
        work1: "Brand design",
        work2: "Promotional flyer",
        work3: "Social media content",
        processTitle: "How we work",
        processText: "We keep communication easy and delivery fast without losing quality.",
        step1Title: "Brief",
        step1Text: "We review the idea, image, or required style.",
        step2Title: "Planning",
        step2Text: "We define the options and design details.",
        step3Title: "Execution",
        step3Text: "We edit or design the final output professionally.",
        step4Title: "Delivery",
        step4Text: "We provide the final result in a ready-to-use format.",
        stat1: "projects completed",
        stat2: "average response",
        stat3: "customer satisfaction",
        ctaTitle: "Ready to start your next project?",
        ctaText: "Contact us now to get a professional design that matches your brand.",
        ctaBtn: "WhatsApp us",
        contactEmailTitle: "Email",
        contactPhoneTitle: "WhatsApp",
        contactLocationTitle: "Location",
        contactLocationText: "Barcelona, Spain",
        formTitle: "Send your project",
        formBtn: "Send request",
        namePlaceholder: "Full name",
        emailPlaceholder: "Email",
        messagePlaceholder: "Write your project here..."
      }
    };

    const langSelect = document.getElementById("languageSelect");

    function setLanguage(lang) {
      const selected = translations[lang] ? lang : "ar";
      document.documentElement.lang = selected;
      document.documentElement.dir = selected === "ar" ? "rtl" : "ltr";

      document.querySelectorAll("[data-i18n]").forEach((el) => {
        const key = el.dataset.i18n;
        if (translations[selected][key]) {
          el.textContent = translations[selected][key];
        }
      });

      document.querySelectorAll("[data-i18n-placeholder]").forEach((el) => {
        const key = el.dataset.i18nPlaceholder;
        if (translations[selected][key]) {
          el.placeholder = translations[selected][key];
        }
      });

      langSelect.value = selected;
      localStorage.setItem("siteLang", selected);
    }

    langSelect.addEventListener("change", (e) => {
      setLanguage(e.target.value);
    });

    setLanguage(localStorage.getItem("siteLang") || "ar");
  </script>
</body>
</html>
