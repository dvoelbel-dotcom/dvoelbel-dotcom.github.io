<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Barbara Weinold – Ergotherapie</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
    }

    html{
      scroll-behavior:smooth;
    }

    body{
      font-family:'Inter',sans-serif;
      background:#f7f9f8;
      color:#1e293b;
      line-height:1.6;
    }

    a{
      text-decoration:none;
      color:inherit;
    }

    img{
      width:100%;
      display:block;
    }

    .container{
      width:min(1200px, 92%);
      margin:auto;
    }

    /* NAVBAR */

    nav{
      position:fixed;
      top:0;
      width:100%;
      z-index:1000;
      background:rgba(255,255,255,0.9);
      backdrop-filter:blur(12px);
      border-bottom:1px solid rgba(0,0,0,0.05);
    }

    .nav-wrapper{
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:18px 0;
    }

    .logo{
      font-size:1.3rem;
      font-weight:700;
      color:#1c6b63;
    }

    .nav-links{
      display:flex;
      gap:30px;
      font-weight:500;
      color:#475569;
    }

    .nav-links a:hover{
      color:#1c6b63;
    }

    /* HERO */

    .hero{
      min-height:100vh;
      display:flex;
      align-items:center;
      background:
      linear-gradient(to right, rgba(255,255,255,0.92), rgba(255,255,255,0.65)),
      url('1779267828490.jpg') center/cover;
    }

    .hero-content{
      max-width:700px;
      padding-top:80px;
    }

    .hero h1{
      font-size:4rem;
      line-height:1.1;
      margin-bottom:24px;
      color:#0f172a;
    }

    .hero h1 span{
      color:#1c6b63;
    }

    .hero p{
      font-size:1.15rem;
      color:#475569;
      margin-bottom:35px;
    }

    .btn{
      display:inline-block;
      padding:16px 30px;
      border-radius:999px;
      background:#1c6b63;
      color:white;
      font-weight:600;
      transition:0.3s;
    }

    .btn:hover{
      background:#14524c;
      transform:translateY(-2px);
    }

    /* SECTION */

    section{
      padding:110px 0;
    }

    .section-title{
      text-align:center;
      margin-bottom:70px;
    }

    .section-title h2{
      font-size:2.5rem;
      margin-bottom:15px;
      color:#0f172a;
    }

    .section-title p{
      max-width:700px;
      margin:auto;
      color:#64748b;
    }

    /* ABOUT */

    .about-grid{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:60px;
      align-items:center;
    }

    .about-img img{
      border-radius:28px;
      box-shadow:0 20px 40px rgba(0,0,0,0.08);
    }

    .about-text h3{
      font-size:2rem;
      margin-bottom:20px;
      color:#1c6b63;
    }

    .about-text p{
      margin-bottom:18px;
      color:#475569;
    }

    /* SERVICES */

    .services-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:30px;
    }

    .service-card{
      background:white;
      border-radius:24px;
      overflow:hidden;
      box-shadow:0 10px 30px rgba(0,0,0,0.05);
      transition:0.3s;
    }

    .service-card:hover{
      transform:translateY(-8px);
    }

    .service-content{
      padding:28px;
    }

    .service-content h3{
      margin-bottom:12px;
      color:#1c6b63;
      font-size:1.35rem;
    }

    .service-content p{
      color:#64748b;
      font-size:0.98rem;
    }

    /* GALLERY */

    .gallery-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:20px;
    }

    .gallery-grid img{
      border-radius:20px;
      height:260px;
      object-fit:cover;
      transition:0.4s;
    }

    .gallery-grid img:hover{
      transform:scale(1.03);
    }

    /* CONTACT */

    .contact-wrapper{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:60px;
      align-items:start;
    }

    .contact-box{
      background:white;
      padding:40px;
      border-radius:28px;
      box-shadow:0 10px 30px rgba(0,0,0,0.05);
    }

    .contact-box h3{
      margin-bottom:20px;
      color:#1c6b63;
      font-size:1.6rem;
    }

    .contact-info{
      display:flex;
      flex-direction:column;
      gap:18px;
      color:#475569;
    }

    form{
      display:flex;
      flex-direction:column;
      gap:18px;
    }

    input,
    textarea{
      padding:16px;
      border-radius:16px;
      border:none;
      background:#f1f5f9;
      font-family:inherit;
      font-size:1rem;
    }

    textarea{
      min-height:140px;
      resize:vertical;
    }

    button{
      border:none;
      cursor:pointer;
    }

    /* FOOTER */

    footer{
      background:#0f172a;
      color:white;
      padding:40px 0;
      text-align:center;
    }

    footer p{
      opacity:0.8;
    }

    /* RESPONSIVE */

    @media(max-width:900px){

      .hero h1{
        font-size:2.8rem;
      }

      .about-grid,
      .contact-wrapper{
        grid-template-columns:1fr;
      }

      .nav-links{
        display:none;
      }
    }

  </style>
</head>
<body>

  <!-- NAVIGATION -->

  <nav>
    <div class="container nav-wrapper">
      <div class="logo">Barbara Weinold</div>

      <div class="nav-links">
        <a href="#about">Über mich</a>
        <a href="#services">Angebot</a>
        <a href="#orga">Ablauf und Organisatorisches</a>
        <a href="#gallery">Was ist Ergotherapie</a>
        <a href="#contact">Kontakt</a>
      </div>
    </div>
  </nav>

  <!-- HERO -->

  <section class="hero">
    <div class="container">
      <div class="hero-content">

        <h1>
          Ergotherapie mit <span>Herz, Ruhe und Vertrauen</span>
        </h1>

        <p>
          Willkommen bei Barbara Weinold – Ihrer modernen Praxis für Ergotherapie.
          Individuelle Betreuung, persönliche Begleitung und ganzheitliche Therapie
          für Kinder, Erwachsene und Senior:innen.
        </p>

        <a href="#contact" class="btn">
          Termin vereinbaren
        </a>

      </div>
    </div>
  </section>

  <!-- ABOUT -->

  <section id="about">
    <div class="container">

      <div class="section-title">
        <h2>Über mich</h2>
        <p>
          Ich bin Barbara Weinold, Ergotherapeutin mit Herz und Seele. Ich weiß aus eigener Erfahrung wie es ist, die Welt anders zu erleben, und wie schwierig es sein kann, darin den eigenen Weg zu finden. Gemeinsam mit meiner fachlichen Erfahrung aus zahlreichen Jobs in psychiatrischen Settings gelingt es mir dadurch, auf jede:n Klient:in ganz individuell einzugehen – mit Verständnis und Motivation zur Veränderung. Ich gehe die Ergotherapie an wie alles andere in meinem Leben: mit Energie, Authentizität und einer ordentlichen Prise Humor, auch und trotz belastender Themen, die mitgebracht werden. Ich arbeite mit Jugendlichen und Erwachsenen, die im Alltag an ihre Grenzen kommen und bereit sind, gemeinsam etwas zu verändern – egal, wo diese Grenzen liegen.  
        </p>
      </div>
      <div class="about-grid">

        <div class="about-img">
          <img src="https://img-getpocket.cdn.mozilla.net/296x160/smart/filters:format(webp):quality(75):no_upscale():strip_exif()/https%3A%2F%2Fs3.us-east-1.amazonaws.com%2Fpocket-curatedcorpusapi-prod-images%2F0c988eed-37ad-4f13-b06e-8b6ce392f4ac.jpeg" alt="">
        </div>

        <div class="about-text">
          <h3>Beruflicher Werdegang</h3>

          <p>
•	Seit 2025 Psychotherapie Station Hall, ehem. B5 <br>
•	2024-2025 Caravan, pro mente (Tagesstruktur für Menschen mit Suchterkrankung) - Karenzstelle <br>
•	2024 VAMED Innsbruck (ambulante psychosoziale Reha) <br>
•	2023-2024 Sonnenpark Lans (stationäre psychosoziale Reha) - Karenzstelle <br>
•	2021-2023 Psychiatrie Innsbruck (v.a. Station für psychosomatische Medizin) - Karenzstelle <br>
•	2020-2021 PKA Innsbruck (Orthopädie, Neurologie, Pädiatrie) <br>
•	2017-2020 FH Studium Ergotherapie

          </p>

           <div class="about-text">
          <h3>Fortbildungen</h3>

          <p>
•	Handeln ermöglichen – Trägheit überwinden (ergotherapie austria, 2022) <br>
•	Traumasensibles Arbeiten in der Ergotherapie (ergotherapie austria, 2024)<br>
•	Angst- und Panikstörungen (pro mente akademie, 2024)<br>
•	Schlafcoaching (pro mente akademie, 2024)<br>
•	Selbstwert – Selbstvertrauen – Selbstwirksamkeit (ergotherapie austria, 2025)<br>
•	Kreativ-Therapeutisches Schreiben in der Psychiatrie und Psychosomatik (tirol kliniken, 2026)<br>
•	Neurodivergenz in der Ergotherapie (ergotherapie austria, 2026)


          </p>


        </div>

      </div>
    </div>
  </section>

  <!-- SERVICES -->

  <section id="services">

    <div class="container">

      <div class="section-title">
        <h2>Angebot</h2>
        <p>
          Individuelle Therapiekonzepte für verschiedene Lebenssituationen und Herausforderungen.
        </p>
      </div>

      <div class="services-grid">

        <div class="service-card">
          <img src="1779265210135.jpg" alt="">

          <div class="service-content">
            <h3>Einzeltherapie</h3>
            <p>
              Im Einzelsetting bekommen Sie die Zeit, die Sie brauchen, um sich mit Ihrem Alltag auseinanderzusetzen. Persönliche Schwierigkeiten, aber vor allem persönliche Stärken und Ressourcen stehen im Vordergrund. Die Einzeltherapie findet in der Regel in meiner Praxis statt, und beinhaltet u.a. Gespräche, kreative Betätigungen und Alltagstätigkeiten. 
            </p>
          </div>
        </div>

        <div class="service-card">
          <img src="1779265617877.jpg" alt="">

          <div class="service-content">
            <h3>Hausbesuche</h3>
            <p>
           Bei Bedarf kann die Therapie auch zu Hause bei Ihnen stattfinden oder unterwegs bei Tätigkeiten ihres täglichen Lebens. Wichtig: Hausbesuche müssen von Ihrer Ärztin/Ihrem Arzt bereits auf der Überweisung vermerkt werden. 
            </p>
          </div>
        </div>

        <div class="service-card">
          <img src="1779265674001.jpg" alt="">

          <div class="service-content">
            <h3>Angehörigenarbeit und Vernetzung mit anderen Berufsgruppen</h3>
            <p>
              Als Ergotherapeutin weiß ich, dass Veränderung nicht isoliert bei meinen Klient:innen stattfindet, sondern auch das soziale Umfeld beeinflusst und umgekehrt. Daher beziehe ich bei Bedarf auch die Angehörigen mit ein. Eine Vernetzung mit anderen involvierten Berufsgruppen, z.B. behandelnden Ärzt:innen, Psychotherapeut:innen oder Sozialarbeiter:innen ist mir ebenfalls wichtig.
            </p>
          </div>
        </div>

        <div class="service-card">
          <img src="1779265552205.jpg" alt="">

          <div class="service-content">
            <h3>Ergotherapie auf Englisch</h3>
            <p>
              Mit einem geprüften C2 Englisch Sprachniveau (nach CAE = Cambridge Certificate in Advanced English) biete ich Ergotherapie auch auf Englisch an.
            </p>
          </div>
        </div>

        <div class="service-card">
          <img src="1779265258690.jpg" alt="">
          </div>
        </div>

      </div>

    </div>

  </section>

  <!-- GALLERY -->

  <section id="gallery">

    <div class="container">

      <div class="section-title">
        <h2>Was ist Ergotherapie</h2>
        <p>
          Ergotherapie hilft dabei, die eigene Handlungsfähigkeit wiederherzustellen. Denn wir Menschen sind im Grunde gerne tätig – wir haben Spaß an unseren alltäglichen Betätigungen (wenn auch an manchen mehr als an anderen), wir TUN gerne. Sind diese Betätigungen nicht (mehr) möglich, kommt es zu gesundheitlichen Einschränkungen. Gemeinsam finden wir also Mittel und Wege, wie Sie Ihren Alltag so meistern können, dass Sie wieder mehr Zufriedenheit und Lebensqualität erleben können. Das beinhaltet neben dem Training von persönlichen Fähigkeiten auch Adaptierungen Ihrer Betätigungen und Ihrer Umwelt, denn das alles spielt bei Beeinträchtigungen eine Rolle. 
        </p>



      </div>



    </div>

  </section>


  <!-- ORGA -->

  <section id="orga">

    <div class="container">

      <div class="section-title">
        <h2>Ablauf und Organisatorisches</h2>
        <p>
          Bevor Sie zu mir kommen, benötigen Sie eine Überweisung von Ihrer/Ihrem Haus- oder Facharzt/-ärztin. Auf der Überweisung steht die Anzahl der Ergotherapie Einheiten, die Dauer einer Einheit und ob Sie diese als Hausbesuche benötigen. <br>
Mit dieser Überweisung melden Sie sich bei mir und wir vereinbaren einen Termin für das Erstgespräch. Darin entscheiden wir gemeinsam, woran wir in der Ergotherapie arbeiten und in welchem Abstand die Einheiten stattfinden. <br>
Ich bin Wahltherapeutin, das bedeutet, dass Sie am Ende jeder Einheit direkt bei mir in der Praxis bezahlen (in bar oder mit Karte) und die Rechnung im Anschluss selbst bei Ihrer Krankenkassa einreichen. Von der Krankenkassa erhalten Sie dann einen Anteil der Kosten rückerstattet. 
        </p>
        <div class="orga-text">


          <h3>Kosten</h3>
          <p>
Die Dauer einer Ergotherapie Einheit wird von der/vom zuständigen Arzt/Ärztin bereits auf die Überweisung geschrieben. Üblich sind v.a. 45 und 60 Minuten Einheiten. Bei geringer Konzentrationsfähigkeit können manchmal auch 30 Minuten Einheiten sinnvoll sein.<br>
Für eine 45 Minuten Einheit verrechne ich 75€, für 60 Minuten 100€. <br>
Für Hausbesuche verrechne ich zusätzlich zum oben genannten Honorar einen Pauschalbetrag von 30€ pro Termin. <br>
Angehörigengespräche, Vernetzungen mit anderen Berufsgruppen oder dem schulischen/beruflichen Umfeld kann ich nach Absprache mit Ihnen ohne selbstständig ärztliche Zuweisung durchführen und werden ebenfalls verrechnet (20€ pro 15 Minuten). Auch dafür gibt es eine teilweise Kostenrückerstattung von der Krankenkasse. 
          </p>

          <h3>Was passiert in den einzelnen Einheiten?</h3>
          <p>
Die erste Einheit verwende ich für ein ausführliches Gespräch, in dem ich mir ein Bild von Ihnen, Ihrem Alltag und Ihrem Umfeld mache. Wir suchen gemeinsam nach den Betätigungen, die Ihnen nicht (mehr) gelingen wollen und einigen uns auf ein Therapieziel. 
Die folgenden Therapieeinheiten arbeiten wir gemeinsam daran, dieses Ziel zu erreichen. Das kann durch Gespräche und Beratung erfolgen, durch eine Analyse der Betätigungen, die Ihnen wichtig sind, oder durch kreative Prozesse. Ergotherapie heißt Tun, daher fokussiere ich mich immer wieder mit Ihnen auf die Betätigungen, die Ihnen wichtig sind. Das kann manchmal auch bedeuten, dass wir gemeinsam genau diese Betätigungen durchführen, um sie zu üben oder auf eventuelle Hindernisse zu untersuchen. 
          </p>
           <div class="orga-text">


      </div>



    </div>

  </section>



  <!-- CONTACT -->

  <section id="contact">

    <div class="container">

      <div class="section-title">
        <h2>Kontakt</h2>
        <p>
          Ich freue mich auf Ihre Anfrage und berate Sie gerne persönlich.
        </p>
      </div>

      <div class="contact-wrapper">

        <div class="contact-box">

          <h3>Praxisinformationen</h3>

          <div class="contact-info">
            <p><strong>Barbara Weinold – Ergotherapie</strong></p>
            <p>Musterstraße 24<br>1010 Wien</p>
            <p>+43 660 1234567</p>
            <p>kontakt@barbara-weinold.at</p>
            <p>Mo – Fr: 08:00 – 18:00 Uhr</p>
          </div>

        </div>

        <div class="contact-box">

          <h3>Nachricht senden</h3>

          <form>

            <input type="text" placeholder="Ihr Name">

            <input type="email" placeholder="Ihre E-Mail">

            <textarea placeholder="Ihre Nachricht"></textarea>

            <button class="btn">
              Anfrage senden
            </button>

          </form>

        </div>

      </div>

    </div>

  </section>

  <!-- FOOTER -->

  <footer>
    <div class="container">
      <p>
        © 2026 Barbara Weinold – Ergotherapie | Moderne Praxis für Ergotherapie
      </p>
    </div>
  </footer>

</body>
</html>
