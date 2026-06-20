<!DOCTYPE html>
<html lang="mn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CŌHI HAUS — Гар Урлалын Кофе</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Playfair+Display:ital@1&family=Space+Grotesk:wght@400;500;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">

    <style>
        :root {
            --bg: #0d0d0d;
            --ink: #f5f0e8;
            --ink-dim: #a39e96;
            --amber: #ff6a00;
            --amber-soft: #ffb070;
            --rule: #2a2622;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }
        *:focus-visible { outline: 2px solid var(--amber); outline-offset: 3px; }

        html { scroll-behavior: smooth; }
        body {
            background-color: var(--bg);
            color: var(--ink);
            font-family: 'Space Grotesk', sans-serif;
            overflow-x: hidden;
        }
        img { display: block; max-width: 100%; }
        ::selection { background: var(--amber); color: #0d0d0d; }

        .film-grain {
            position: fixed; inset: 0;
            background: url('https://assets.codepen.io/13471/noise.png');
            opacity: 0.04; pointer-events: none; z-index: 999;
        }

        .progress-rail { position: fixed; top: 0; left: 0; height: 2px; width: 100%; background: var(--rule); z-index: 50; }
        .progress-fill { height: 100%; width: 0%; background: var(--amber); transition: width 0.1s linear; }

        #canvas-container { position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; z-index: 1; transition: opacity 0.6s ease; }

        .brand-mark {
            font-family: 'Archivo Black', sans-serif;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            line-height: 0.95;
        }
        .script-tag {
            font-family: 'Playfair Display', serif;
            font-style: italic;
            color: var(--ink-dim);
        }

        header {
            position: fixed; top: 0; left: 0; right: 0;
            display: flex; justify-content: space-between; align-items: center;
            padding: 30px 5%; z-index: 20; mix-blend-mode: difference;
        }
        .logo { font-size: 1.3rem; color: var(--ink); }
        nav.primary-nav { display: flex; gap: 32px; align-items: center; }
        nav.primary-nav a {
            color: var(--ink); text-decoration: none; font-size: 0.76rem;
            letter-spacing: 1.5px; text-transform: uppercase; opacity: 0.7;
            transition: opacity 0.25s ease;
        }
        nav.primary-nav a:hover { opacity: 1; }
        .nav-tag {
            color: var(--ink); opacity: 0.55; letter-spacing: 1px;
            font-size: 0.72rem; font-family: 'JetBrains Mono', monospace;
            display: flex; align-items: center; gap: 6px;
        }

        .scroller { height: 420vh; position: relative; z-index: 2; pointer-events: none; }
        .section { height: 100vh; display: flex; flex-direction: column; justify-content: center; padding: 0 8%; position: relative; }

        .eyebrow {
            font-family: 'JetBrains Mono', monospace; font-size: 0.76rem;
            letter-spacing: 3px; text-transform: uppercase; color: var(--amber);
            margin-bottom: 18px; display: flex; align-items: center; gap: 8px;
        }

        .section-1 { max-width: 680px; }
        .section-1 h1 { font-size: clamp(2.6rem, 7vw, 5.6rem); }
        .section-1 .script-tag { font-size: clamp(1.15rem, 2.2vw, 1.6rem); margin-top: 20px; max-width: 480px; line-height: 1.5; }
        .scroll-cue {
            position: absolute; bottom: 52px; left: 8%;
            display: flex; align-items: center; gap: 10px;
            font-family: 'JetBrains Mono', monospace; font-size: 0.7rem;
            letter-spacing: 2px; color: var(--ink-dim); text-transform: uppercase;
        }
        .scroll-cue::before { content: ''; width: 22px; height: 1px; background: var(--ink-dim); display: inline-block; animation: cuepulse 1.8s ease-in-out infinite; }
        @keyframes cuepulse { 0%,100%{opacity:.3} 50%{opacity:1} }

        .photo-pair {
            display: flex; align-items: center; gap: 48px;
            pointer-events: auto;
        }
        .pair-photo {
            width: 230px; flex-shrink: 0;
            border: 6px solid var(--ink);
            transform: rotate(-3deg);
            box-shadow: 0 18px 40px rgba(0,0,0,0.55);
        }
        .pair-photo img { width: 100%; aspect-ratio: 4/5; object-fit: cover; }
        .pair-photo figcaption {
            font-family: 'JetBrains Mono', monospace; font-size: 0.68rem;
            color: #0d0d0d; background: var(--ink); padding: 6px 0 2px;
            text-align: center; letter-spacing: 1px; text-transform: uppercase;
        }
        .pair-text { max-width: 380px; }
        .pair-text h2 { font-family: 'Archivo Black', sans-serif; text-transform: uppercase; font-size: 2.1rem; line-height: 1.08; margin-bottom: 16px; }
        .pair-text p { color: var(--ink-dim); line-height: 1.75; font-size: 1rem; }

        .section-3 .photo-pair { flex-direction: row-reverse; }
        .section-3 .pair-photo { transform: rotate(3deg); }
        .section-3 .pair-text { text-align: right; }
        .section-3 .pair-text h2 { font-size: clamp(1.8rem, 4vw, 2.8rem); }

        .call-btn {
            display: inline-flex; align-items: center; gap: 10px;
            padding: 14px 28px; background: var(--amber); color: #0d0d0d;
            font-weight: 700; text-transform: uppercase; letter-spacing: 1.5px;
            text-decoration: none; font-size: 0.8rem;
            margin-top: 22px; transition: all 0.3s ease; pointer-events: auto;
            font-family: 'Space Grotesk', sans-serif;
        }
        .call-btn:hover { background: var(--ink); transform: translateY(-2px); }

        main.body-content { position: relative; z-index: 5; background: var(--bg); }
        .wrap { max-width: 1180px; margin: 0 auto; padding: 0 6%; }

        .section-head {
            display: flex; justify-content: space-between; align-items: flex-end; gap: 24px;
            margin-bottom: 56px; border-bottom: 1px solid var(--rule); padding-bottom: 26px; flex-wrap: wrap;
        }
        .section-head h2 { font-family: 'Archivo Black', sans-serif; text-transform: uppercase; font-size: clamp(1.6rem, 3.2vw, 2.3rem); }
        .section-head .tally { font-family: 'JetBrains Mono', monospace; font-size: 0.78rem; color: var(--ink-dim); letter-spacing: 1px; }

        .opening-band { padding: 130px 0 0; }
        .opening-grid {
            display: grid; grid-template-columns: 0.85fr 1.15fr; gap: 0;
            border: 1px solid var(--rule);
        }
        .opening-grid img { width: 100%; height: 100%; object-fit: cover; aspect-ratio: 4/5; }
        .opening-copy { padding: 56px; display: flex; flex-direction: column; justify-content: center; gap: 18px; }
        .opening-copy h2 { font-family: 'Archivo Black', sans-serif; text-transform: uppercase; font-size: clamp(1.8rem, 4vw, 3rem); line-height: 1.05; }
        .opening-copy .dates { font-family: 'JetBrains Mono', monospace; color: var(--amber); font-size: 1rem; letter-spacing: 1px; }
        .opening-copy p { color: var(--ink-dim); line-height: 1.7; max-width: 440px; }

        .process { padding: 130px 0; }
        .process-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1px; background: var(--rule); border: 1px solid var(--rule); }
        .process-step { background: var(--bg); padding: 40px 32px; display: flex; flex-direction: column; gap: 18px; }
        .process-step .num { font-family: 'JetBrains Mono', monospace; font-size: 0.85rem; color: var(--amber); letter-spacing: 1px; }
        .process-step h3 { font-family: 'Archivo Black', sans-serif; text-transform: uppercase; font-size: 1.25rem; line-height: 1.25; }
        .process-step p { color: var(--ink-dim); font-size: 0.94rem; line-height: 1.7; }

        .gallery { padding: 0 0 130px; }
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            grid-auto-rows: 150px;
            gap: 14px;
        }
        .gallery-item { position: relative; overflow: hidden; cursor: pointer; background: #000; }
        .gallery-item img, .gallery-item video { width: 100%; height: 100%; object-fit: cover; transition: transform 0.5s ease; }
        .gallery-item:hover img, .gallery-item:hover video { transform: scale(1.04); }
        .g-tall { grid-row: span 3; }
        .g-mid { grid-row: span 2; }
        .g-wide { grid-column: span 2; grid-row: span 2; }
        .play-badge {
            position: absolute; inset: 0; display: flex; align-items: center; justify-content: center;
            background: rgba(13,13,13,0.25);
        }
        .play-badge svg { width: 46px; height: 46px; filter: drop-shadow(0 4px 10px rgba(0,0,0,0.6)); }
        .gallery-item.is-playing .play-badge { display: none; }
        .g-label {
            position: absolute; left: 14px; bottom: 12px;
            font-family: 'JetBrains Mono', monospace; font-size: 0.68rem;
            letter-spacing: 1.5px; text-transform: uppercase; color: var(--ink);
            text-shadow: 0 2px 6px rgba(0,0,0,0.8);
        }

        footer { border-top: 1px solid var(--rule); padding: 70px 0 36px; }
        .footer-grid { display: grid; grid-template-columns: 1.4fr 1fr 1fr; gap: 48px; padding-bottom: 56px; }
        footer .logo { font-size: 1.5rem; margin-bottom: 16px; color: var(--amber); }
        footer .tagline { color: var(--ink-dim); font-size: 0.95rem; line-height: 1.7; max-width: 320px; }
        footer h4 { font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; letter-spacing: 2px; text-transform: uppercase; color: var(--ink-dim); margin-bottom: 16px; }
        footer ul { list-style: none; display: flex; flex-direction: column; gap: 10px; }
        footer a, footer address { color: var(--ink); text-decoration: none; font-size: 0.94rem; font-style: normal; line-height: 1.6; }
        footer a:hover { color: var(--amber); }
        .footer-base {
            display: flex; justify-content: space-between; align-items: center;
            padding-top: 26px; border-top: 1px solid var(--rule);
            font-family: 'JetBrains Mono', monospace; font-size: 0.7rem; color: var(--ink-dim);
            letter-spacing: 1px; flex-wrap: wrap; gap: 12px;
        }

        @media (max-width: 860px) {
            header { padding: 22px 6%; }
            nav.primary-nav { display: none; }
            .scroller { height: 460vh; }
            .section { padding: 0 6%; }
            .photo-pair, .section-3 .photo-pair { flex-direction: column; align-items: flex-start; gap: 24px; }
            .section-3 .pair-text { text-align: left; }
            .pair-photo { width: 170px; }
            .opening-grid { grid-template-columns: 1fr; }
            .opening-grid img { aspect-ratio: 16/10; }
            .opening-copy { padding: 36px 28px; }
            .process-grid { grid-template-columns: 1fr; }
            .gallery-grid { grid-template-columns: repeat(2, 1fr); grid-auto-rows: 160px; }
            .g-wide { grid-column: span 2; }
            .footer-grid { grid-template-columns: 1fr; gap: 32px; }
            .section-head { flex-direction: column; align-items: flex-start; }
        }

        @media (prefers-reduced-motion: reduce) {
            html { scroll-behavior: auto; }
            .scroll-cue::before { animation: none; }
        }
    </style>
</head>
<body>

    <div class="film-grain"></div>
    <div class="progress-rail"><div class="progress-fill" id="progressFill"></div></div>
    <div id="canvas-container"></div>

    <header>
        <div class="logo brand-mark">Cōhi Haus</div>
        <nav class="primary-nav">
            <a href="#opening">Soft Opening</a>
            <a href="#process">Цэс</a>
            <a href="#gallery">Дотроос нь</a>
            <a href="#visit">Хаяг</a>
        </nav>
        <div class="nav-tag">📍 Циркийн баруун талд</div>
    </header>

    <div class="scroller">
        <section class="section section-1">
            <div class="eyebrow">// Handcrafted Coffee — Ulaanbaatar</div>
            <h1 class="brand-mark">ГАР УРЛАЛЫН<br><span style="color:var(--amber)">КОФЕНЫ</span> УРСГАЛ</h1>
            <p class="script-tag">"We invite you to experience our first brew, crafted by hand and shared with heart."</p>
            <div class="scroll-cue">Доош гүйлгэнэ үү</div>
        </section>

        <section class="section section-2">
            <div class="photo-pair">
                <figure class="pair-photo">
                    <img src="assets/img-02.jpg" alt="Бариста зэс саванд боргиосон Туркийн кофег цутгаж байгаа нь" loading="lazy">
                    <figcaption>Turkish Sand Coffee</figcaption>
                </figure>
                <div class="pair-text">
                    <h2>Хамгийн Эртний Арга</h2>
                    <p>Халуун элсэн дээр гуулин саванд аажмаар боргилуулсан, хамгийн эртний Туркийн уламжлалт кофег Япон баристагийн нарийн мэдрэмжээр бэлдэнэ. Шилэн S-хоолой болон мушгиа спиралиар уруудах дусал бүр өтгөн, хөөстэй.</p>
                </div>
            </div>
        </section>

        <section class="section section-3">
            <div class="photo-pair">
                <figure class="pair-photo">
                    <img src="assets/img-06.jpg" alt="Cōhi Haus дотор тайван ширээ, дэнлүүний гэрэл" loading="lazy">
                    <figcaption>Quiet Corner</figcaption>
                </figure>
                <div class="pair-text">
                    <h2 class="brand-mark">НЭГ УРСГАЛ.<br>НЭГ ШИЛ.<br>ТАЙВАН ОРЧИН.</h2>
                    <a href="#visit" class="call-btn">Хаяг харах →</a>
                </div>
            </div>
        </section>
    </div>

    <main class="body-content">

        <section class="opening-band" id="opening">
            <div class="wrap">
                <div class="opening-grid">
                    <img src="assets/img-01.jpg" alt="Cōhi Haus Soft Opening зар, 2025 оны 10-р сарын 25, 26" loading="lazy">
                    <div class="opening-copy">
                        <div class="eyebrow">// We're Now Open</div>
                        <h2 class="brand-mark">Soft<br>Opening</h2>
                        <div class="dates">10-р сарын 25, 26 — 12:00 - 17:00</div>
                        <p>Анхны хандлагаа гараараа бэлдэж, сэтгэлээсээ үйлчилнэ. Эхний хоёр өдрийн зочдоо тайван, дулаахан орчинд хүлээж байна.</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="process" id="process">
            <div class="wrap">
                <div class="section-head">
                    <div>
                        <div class="eyebrow">// Science Meets Coffee</div>
                        <h2>Хандлалтын Төрлүүд</h2>
                    </div>
                    <div class="tally">03 АРГА БАРИЛ</div>
                </div>
                <div class="process-grid">
                    <div class="process-step">
                        <span class="num">01</span>
                        <h3>Pour Over</h3>
                        <p>Цаасан шүүлтүүрээр дусаж, шилэн S-хоолой болон спиралиар уруудах маш тунгалаг, цэвэр хандлалт. Жимсний болон цэцгийн нарийн амтыг дээд цэгт нь мэдрүүлнэ.</p>
                    </div>
                    <div class="process-step">
                        <span class="num">02</span>
                        <h3>Syphon Coffee</h3>
                        <p>Вакуум даралтаар нэрдэг, шинжлэх ухаан ба урлагийн төгс хослол. Биет нь арай хүнд бөгөөд кофены гүн баялаг амтыг хадгална.</p>
                    </div>
                    <div class="process-step">
                        <span class="num">03</span>
                        <h3>Turkish Sand Coffee</h3>
                        <p>Хамгийн эртний уламжлалт арга — халуун элсэн дээр гуулин саванд аажмаар боргилуулан чанадаг өтгөн, хөөстэй кофе.</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="gallery" id="gallery">
            <div class="wrap">
                <div class="section-head">
                    <div>
                        <div class="eyebrow">// Inside The Haus</div>
                        <h2>Дотроос Нь</h2>
                    </div>
                    <div class="tally">ДАРЖ ВИДЕО ҮЗНЭ ҮҮ</div>
                </div>
                <div class="gallery-grid">

                    <div class="gallery-item g-tall video-tile" data-video="assets/video-syphon.mp4">
                        <video muted loop playsinline preload="none" poster="assets/poster-syphon.jpg"></video>
                        <div class="play-badge"><svg viewBox="0 0 24 24" fill="white"><circle cx="12" cy="12" r="11" fill="rgba(13,13,13,0.55)"/><path d="M9.5 7.5l8 4.5-8 4.5z"/></svg></div>
                        <span class="g-label">Art of Syphon</span>
                    </div>

                    <div class="gallery-item g-wide">
                        <img src="assets/img-04.jpg" alt="Цонхны хажуугийн урт ширээ, ногоон ургамал" loading="lazy">
                        <span class="g-label">Window Bar</span>
                    </div>

                    <div class="gallery-item g-mid video-tile" data-video="assets/video-turkish-coffee.mp4">
                        <video muted loop playsinline preload="none" poster="assets/poster-turkish.jpg"></video>
                        <div class="play-badge"><svg viewBox="0 0 24 24" fill="white"><circle cx="12" cy="12" r="11" fill="rgba(13,13,13,0.55)"/><path d="M9.5 7.5l8 4.5-8 4.5z"/></svg></div>
                        <span class="g-label">Turkish Coffee</span>
                    </div>

                    <div class="gallery-item g-mid">
                        <img src="assets/img-08.jpg" alt="Улаан гэрэлтэй коридор, ногоон ургамал" loading="lazy">
                        <span class="g-label">Corner Light</span>
                    </div>

                    <div class="gallery-item g-wide video-tile" data-video="assets/video-best-coffee.mp4">
                        <video muted loop playsinline preload="none" poster="assets/poster-best.jpg"></video>
                        <div class="play-badge"><svg viewBox="0 0 24 24" fill="white"><circle cx="12" cy="12" r="11" fill="rgba(13,13,13,0.55)"/><path d="M9.5 7.5l8 4.5-8 4.5z"/></svg></div>
                        <span class="g-label">Cōhi Haus Reel</span>
                    </div>

                </div>
            </div>
        </section>

        <footer id="visit">
            <div class="wrap">
                <div class="footer-grid">
                    <div>
                        <div class="logo brand-mark">Cōhi Haus</div>
                        <p class="tagline script-tag">handcrafted coffee</p>
                        <p class="tagline" style="margin-top:14px;">Pour over, syphon, Turkish sand coffee. Гар урлалын кофе, Улаанбаатарт.</p>
                    </div>
                    <div>
                        <h4>Байршил & Цаг</h4>
                        <ul>
                            <li><address>📍 Циркийн баруун талд, Улаанбаатар</address></li>
                            <li style="color: var(--amber);">Soft Opening: 10-р сарын 25–26, 12:00–17:00</li>
                        </ul>
                    </div>
                    <div>
                        <h4>Холбоо Барих</h4>
                        <ul>
                            <li><a href="#">Instagram — @cohihaus</a></li>
                            <li style="color: var(--ink-dim); font-size: 0.85rem;">Утас / и-мэйл — захиалагчаас баталгаажуулна уу</li>
                        </ul>
                    </div>
                </div>
                <div class="footer-base">
                    <span>© 2026 CŌHI HAUS</span>
                    <span>handcrafted coffee //</span>
                </div>
            </div>
        </footer>
    </main>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/gsap.min.js"></script>

    <script>
        const container = document.getElementById('canvas-container');
        const scene = new THREE.Scene();
        scene.background = new THREE.Color(0x0d0d0d);
        scene.fog = new THREE.Fog(0x0d0d0d, 3.5, 8);

        const camera = new THREE.PerspectiveCamera(40, window.innerWidth / window.innerHeight, 0.1, 1000);
        camera.position.set(0.6, 0, 3.6);

        const renderer = new THREE.WebGLRenderer({ antialias: true, alpha: false });
        renderer.setSize(window.innerWidth, window.innerHeight);
        renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
        renderer.outputEncoding = THREE.sRGBEncoding;
        container.appendChild(renderer.domElement);

        const apparatus = new THREE.Group();
        apparatus.position.set(0.45, 0, 0);
        scene.add(apparatus);

        const amberGlass = new THREE.MeshPhysicalMaterial({
            color: 0xff6a00, transparent: true, opacity: 0.62,
            roughness: 0.18, metalness: 0, clearcoat: 0.6, clearcoatRoughness: 0.25,
            side: THREE.DoubleSide
        });
        const wireframeOrangeOverlay = new THREE.MeshBasicMaterial({ color: 0xffaa00, wireframe: true, transparent: true, opacity: 0.1 });
        const matteBlackMetal = new THREE.MeshStandardMaterial({ color: 0x222222, roughness: 0.55, metalness: 0.4 });
        const richWoodMat = new THREE.MeshStandardMaterial({ color: 0x5c3116, roughness: 0.7, metalness: 0 });
        const premiumFilterMat = new THREE.MeshStandardMaterial({ color: 0xfffae8, roughness: 0.9, metalness: 0 });
        const steamParticleMat = new THREE.MeshBasicMaterial({ color: 0xffffff, transparent: true, opacity: 0.08 });

        class HelixCurve extends THREE.Curve {
            constructor(radius = 0.52, turns = 4.5, height = 1.4) { super(); this.radius = radius; this.turns = turns; this.height = height; }
            getPoint(t) {
                const angle = t * Math.PI * 2 * this.turns;
                return new THREE.Vector3(Math.cos(angle) * this.radius, -0.22 - (t * this.height), Math.sin(angle) * this.radius);
            }
        }
        const spiralCurve = new HelixCurve();
        const spiralGeo = new THREE.TubeGeometry(spiralCurve, 120, 0.045, 16, false);
        apparatus.add(new THREE.Mesh(spiralGeo, amberGlass));
        apparatus.add(new THREE.Mesh(spiralGeo, wireframeOrangeOverlay));

        const funnelGeo = new THREE.ConeGeometry(0.62, 0.6, 24, 1, true);
        funnelGeo.rotateX(Math.PI);
        const funnel = new THREE.Mesh(funnelGeo, amberGlass);
        funnel.position.y = 0.72;
        apparatus.add(funnel);

        const paperFilter = new THREE.Mesh(new THREE.ConeGeometry(0.59, 0.56, 24, 1, false), premiumFilterMat);
        paperFilter.position.y = 0.75; paperFilter.rotateX(Math.PI); apparatus.add(paperFilter);

        const connPoints = [
            new THREE.Vector3(0, 0.42, 0), new THREE.Vector3(0, 0.2, 0),
            new THREE.Vector3(0.05, 0.05, 0), new THREE.Vector3(0.25, -0.12, 0), new THREE.Vector3(0.52, -0.22, 0)
        ];
        const connectorCurve = new THREE.CatmullRomCurve3(connPoints);
        const connectorGeo = new THREE.TubeGeometry(connectorCurve, 32, 0.045, 24, false);
        apparatus.add(new THREE.Mesh(connectorGeo, amberGlass));
        apparatus.add(new THREE.Mesh(connectorGeo, wireframeOrangeOverlay));

        const standGroup = new THREE.Group();
        for (let i = 0; i < 3; i++) {
            const angle = (i / 3) * Math.PI * 2;
            const leg = new THREE.Mesh(new THREE.CylinderGeometry(0.012, 0.012, 2.2, 8), matteBlackMetal);
            leg.position.set(Math.cos(angle) * 0.72, -0.4, Math.sin(angle) * 0.72);
            standGroup.add(leg);
        }
        const topRing = new THREE.Mesh(new THREE.TorusGeometry(0.68, 0.015, 6, 24), matteBlackMetal);
        topRing.position.y = 0.62; topRing.rotateX(Math.PI / 2); standGroup.add(topRing);
        apparatus.add(standGroup);

        const kettleGroup = new THREE.Group();
        const kettleBody = new THREE.Mesh(new THREE.CylinderGeometry(0.18, 0.32, 0.52, 24), matteBlackMetal);
        kettleGroup.add(kettleBody);
        const kettleLid = new THREE.Mesh(new THREE.ConeGeometry(0.18, 0.08, 24), matteBlackMetal);
        kettleLid.position.y = 0.3; kettleGroup.add(kettleLid);
        const lidKnob = new THREE.Mesh(new THREE.CylinderGeometry(0.035, 0.025, 0.05, 8), richWoodMat);
        lidKnob.position.y = 0.36; kettleGroup.add(lidKnob);

        const spoutPoints = [];
        for (let i = 0; i <= 15; i++) { let p = i / 15; spoutPoints.push(new THREE.Vector3(0.15 + p * 0.62, -0.15 + Math.sin(p * Math.PI) * 0.32 + p * 0.22, 0)); }
        const kettleSpout = new THREE.Mesh(new THREE.TubeGeometry(new THREE.CatmullRomCurve3(spoutPoints), 20, 0.015, 8, false), matteBlackMetal);
        kettleGroup.add(kettleSpout);

        const handlePoints = [];
        for (let i = 0; i <= 10; i++) { let p = i / 10; handlePoints.push(new THREE.Vector3(-0.22 - Math.sin(p * Math.PI) * 0.1, 0.1 - p * 0.3, 0)); }
        const kettleHandle = new THREE.Mesh(new THREE.TubeGeometry(new THREE.CatmullRomCurve3(handlePoints), 10, 0.03, 8, false), richWoodMat);
        kettleGroup.add(kettleHandle);

        kettleGroup.scale.setScalar(1.25);
        kettleGroup.position.set(-1.05, 1.15, 0);
        kettleGroup.rotation.z = -0.22;
        apparatus.add(kettleGroup);

        const waterPoints = [new THREE.Vector3(-0.02, 1.28, 0), new THREE.Vector3(0.06, 1.05, 0), new THREE.Vector3(0, 0.82, 0)];
        const waterCurve = new THREE.CatmullRomCurve3(waterPoints);
        const waterGeo = new THREE.TubeGeometry(waterCurve, 12, 0.008, 4, false);
        const waterStream = new THREE.Mesh(waterGeo, new THREE.MeshBasicMaterial({ color: 0xffffff, transparent: true, opacity: 0.35 }));
        apparatus.add(waterStream);

        const steamCount = 12; const steamParticles = [];
        for (let i = 0; i < steamCount; i++) {
            const size = 0.01 + Math.random() * 0.02;
            const particle = new THREE.Mesh(new THREE.SphereGeometry(size, 4, 4), steamParticleMat);
            particle.position.set((Math.random() - 0.5) * 0.4, 0.7 + Math.random() * 0.3, (Math.random() - 0.5) * 0.4);
            apparatus.add(particle);
            steamParticles.push({ mesh: particle, vSpeed: 0.003 + Math.random() * 0.005, initialY: 0.7 });
        }

        scene.add(new THREE.AmbientLight(0xfff1e0, 0.35));
        const keyLight = new THREE.DirectionalLight(0xffb070, 1.4); keyLight.position.set(2.2, 2.5, 2.2); scene.add(keyLight);
        const rimLight = new THREE.PointLight(0x6fa8ff, 1.1, 8); rimLight.position.set(-1.8, 0.5, -1.5); scene.add(rimLight);
        const fillLight = new THREE.PointLight(0xff6a00, 0.6, 6); fillLight.position.set(0.4, -0.6, 1.8); scene.add(fillLight);

        let targetX = 0, targetY = 0;
        window.addEventListener('mousemove', (e) => { targetX = (e.clientX / window.innerWidth) * 2 - 1; targetY = -(e.clientY / window.innerHeight) * 2 + 1; });

        const progressFill = document.getElementById('progressFill');
        let scrollProgress = 0, baseSpeed = 0.0015;
        window.addEventListener('scroll', () => {
            const maxScroll = document.documentElement.scrollHeight - window.innerHeight;
            const heroMax = document.querySelector('.scroller').offsetHeight - window.innerHeight;
            if (maxScroll > 0) progressFill.style.width = (window.scrollY / maxScroll) * 100 + '%';

            if (heroMax > 0) {
                scrollProgress = Math.min(window.scrollY / heroMax, 1);
                baseSpeed = 0.0015 + (scrollProgress * 0.006);
                gsap.to(camera.position, { x: 0.6 - (scrollProgress * 1.2), z: 3.6 - (scrollProgress * 0.2), duration: 1.5, ease: "power1.out" });
                gsap.to(apparatus.rotation, { y: scrollProgress * Math.PI * 1.0, duration: 1.2, ease: "power1.out" });

                const fadeStart = heroMax * 0.92;
                const opacity = window.scrollY > fadeStart ? Math.max(0, 1 - (window.scrollY - fadeStart) / (window.innerHeight * 0.6)) : 1;
                container.style.opacity = opacity;
            }
        });

        const clock = new THREE.Clock();
        function animate() {
            requestAnimationFrame(animate);
            const elapsedTime = clock.getElapsedTime();
            kettleGroup.position.y = 1.15 + Math.sin(elapsedTime * 1.8) * 0.01;

            steamParticles.forEach(p => {
                p.mesh.position.y += p.vSpeed;
                p.mesh.position.x += Math.sin(elapsedTime * 2 + p.mesh.position.y) * 0.0015;
                let life = (p.mesh.position.y - p.initialY) / 0.7;
                p.mesh.material.opacity = 0.08 * (1 - life);
                if (p.mesh.position.y > p.initialY + 0.7) {
                    p.mesh.position.y = p.initialY;
                    p.mesh.position.x = (Math.random() - 0.5) * 0.4;
                    p.mesh.position.z = (Math.random() - 0.5) * 0.4;
                }
            });

            baseSpeed += (0.0012 - baseSpeed) * 0.03;
            apparatus.position.y = Math.sin(elapsedTime * 0.7) * 0.01;
            apparatus.rotation.y += (targetX * 0.08 - apparatus.rotation.y) * 0.02;
            apparatus.rotation.x += (targetY * 0.05 - apparatus.rotation.x) * 0.02;

            renderer.render(scene, camera);
        }
        animate();

        window.addEventListener('resize', () => {
            camera.aspect = window.innerWidth / window.innerHeight;
            camera.updateProjectionMatrix();
            renderer.setSize(window.innerWidth, window.innerHeight);
        });

        document.querySelectorAll('.video-tile').forEach(tile => {
            const video = tile.querySelector('video');
            const src = tile.dataset.video;
            let loaded = false;
            tile.addEventListener('click', () => {
                if (!loaded) { video.src = src; loaded = true; }
                if (video.paused) { video.play(); tile.classList.add('is-playing'); }
                else { video.pause(); tile.classList.remove('is-playing'); }
            });
        });
    </script>
</body>
</html>
