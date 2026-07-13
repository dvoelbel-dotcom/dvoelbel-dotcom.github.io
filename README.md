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
    .hero-container{
      min-width:40%;
      margin:auto;
    }
    p{
      text-align: left;
    }


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
      color:#045680;
    }

    .nav-links{
      display:flex;
      gap:30px;
      font-weight:500;
      color:#475569;
    }

    .nav-links a:hover{
      color:#045680;
    }

    h2{
      color:#045680;
    }


    .hero{
      display:flex;
      align-items:center;
      
    }

    .hero-content{
      max-width:800px;
    }

    .hero h1{
      font-size:4rem;
      line-height:1.1;
      margin-bottom:24px;
      color:#0f172a;
    }

    .hero h1 span{
      color:#045680;
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
      background:#045680;
      color:white;
      font-weight:600;
      transition:0.3s;
    }
    .btn:hover{
      background:#14524c;
      transform:translateY(-2px);
    }


    section{
      padding:40px 0;
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
      color:#045680;
    }

    .about-text p{
      margin-bottom:18px;
      color:#475569;
    }


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



    .service-content{
      padding:28px;
    }

    .service-content h3{
      margin-bottom:12px;
      color:#045680;
      font-size:1.35rem;
    }

    .service-content p{
      color:#64748b;
      font-size:0.98rem;
    }


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
      color:#045680;
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


    footer{
      background:#79398c;
      color:white;
      padding:40px 0;
      text-align:center;
    }

    footer p{
      opacity:0.8;
    }


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

  <nav>
    <div class="container nav-wrapper">
       <img src="file_000000008848724698d5424efc359949.png" style="width: 110px; height: 50px;">
      <div class="nav-links">
        <a href="#services">Therapie</a>
        <a href="#about">Über mich</a>
        <a href="#gallery">Was ist Ergotherapie</a>
        <a href="#orga">Ablauf und Organisatorisches</a>
        <a href="#contact">Kontakt</a>
      </div>
    </div>
  </nav>

  <section class="hero" style="margin-top:50px">
    <div class="hero-container">
      <div class="hero-content">
        <img src="file_000000006c30720aa4b7f2697db9f352.png" style="min-width: 300px;">
      </div>
    </div>
  </section>
  


  <section id="services">
    <div class="container" style="max-width: 800px;">
      <div class="services-grid">
        <div class="service-card">
          <img src="Aeste.jpg" alt="">
          <div class="service-content">
            <h3>Therapieschwerpunkte</h3>
            <p>
              Ich arbeite mit Menschen mit psychischen Beschwerden aller Art ab ca. 18 Jahren. Zu den häufigsten Diagnosen, mit denen ich arbeite, zählen u.a. <br>
              •	ADHS <br>
              •	Autismus <br>
              •	Depressionen <br>
              •	Angst- und Panikstörungen <br>
              •	Suchterkrankungen <br>
              •	Psychosomatische Erkrankungen
            </p>
          </div>
        </div>
        <div class="service-card">
          <img src="SteinhaufenSee.jpg" alt="">
          <div class="service-content">
            <h3>Inhaltliche Schwerpunkte in der Ergotherapie</h3>
            <p>
            •	Emotionsregulierung erarbeiten und üben <br>
            •	Struktur im Alltag finden und beibehalten <br>
            •	Routinen erarbeiten <br>
            •	Bedeutungsvolle Aktivitäten im Alltag finden <br>
            •	Selbstwert und Selbstwirksamkeit stärken <br>
            •	Identitätsfindung <br>
            •	Umgang mit neuen Rollen und Lebensbereichen <br>
            •	Soziale Kompetenzen trainieren <br>
            •	Arbeitsfähigkeiten trainieren <br>
            •	Eigene Grenzen und Belastungen kennenlernen <br>
            •	Umgang mit Ansprüchen und Perfektionismus <br>
            •	Kennenlernen der eigenen Diagnose und Psychoedukation <br>
            •	…
            </p>
          </div>
        </div>
        <div class="service-card">
          <img src="Strand.jpg" alt="">
          <div class="service-content">
            <h3>Einzeltherapie</h3>
            <p>
              Im Einzelsetting bekommen Sie die Zeit, die Sie brauchen, um sich mit Ihrem Alltag auseinanderzusetzen. Persönliche Schwierigkeiten, aber vor allem persönliche Stärken und Ressourcen stehen im Vordergrund. Die                 Einzeltherapie findet in der Regel in meiner Praxis statt und beinhaltet u.a. Gespräche, kreative Betätigungen und Alltagstätigkeiten. 
            </p>
          </div>
        </div>
        <div class="service-card">
          <img src="Tau.jpg" alt="">
          <div class="service-content">
            <h3>Hausbesuche</h3>
            <p>
            Bei Bedarf kann die Therapie auch zu Hause bei Ihnen stattfinden oder unterwegs bei Tätigkeiten Ihres täglichen Lebens. Wichtig: Hausbesuche müssen von Ihrer Ärztin/Ihrem Arzt bereits auf der Überweisung vermerkt werden.
            </p>
          </div>
        </div>
        <div class="service-card">
          <img src="Pflanzbuch.jpg" style="height: 200px;" alt="">
          <div class="service-content">
            <h3>Angehörigenarbeit und Vernetzung mit anderen Berufsgruppen</h3>
            <p>
              Als Ergotherapeutin weiß ich, dass Veränderung nicht isoliert bei meinen Klient:innen stattfindet, sondern auch das soziale Umfeld beeinflusst und umgekehrt. Daher beziehe ich bei Bedarf auch die Angehörigen mit ein. Eine Vernetzung mit anderen involvierten Berufsgruppen, z.B. behandelnden Ärzt:innen, Psychotherapeut:innen oder Sozialarbeiter:innen, ist mir ebenfalls wichtig und kann bei Bedarf jederzeit erfolgen.
            </p>
          </div>
        </div>
        <div class="service-card">
          <img src="Hofgarten.jpg" alt="">
          <div class="service-content">
            <h3>Ergotherapie auf Englisch</h3>
            <p>
              Mit einem geprüften C2 Englisch Sprachniveau (nach CAE = Cambridge Certificate in Advanced English) biete ich Ergotherapie auch auf Englisch an.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section id="about">
    <div class="container">
      <div class="section-title">
        <h2 style="color: #045680">Über mich</h2>
        <p>
          Ich bin Barbara Weinold, Ergotherapeutin mit Herz und Seele. Ich weiß aus eigener Erfahrung, wie es ist, die Welt anders zu erleben, und wie schwierig es sein kann, darin den eigenen Weg zu finden. 
        </p>
        <p>
          Gemeinsam mit meiner fachlichen Erfahrung aus zahlreichen Jobs in psychiatrischen Settings gelingt es mir dadurch, auf jede:n Klient:in ganz individuell einzugehen – mit Verständnis und Motivation zur Veränderung.
        </p>
        <p>
           Ich gehe die Ergotherapie an wie alles andere in meinem Leben: mit Energie, Authentizität und einer ordentlichen Prise Humor, auch und trotz belastender Themen, die mitgebracht werden. 
        </p>
        <p>
          Ich arbeite mit Jugendlichen und Erwachsenen, die im Alltag an ihre Grenzen kommen und bereit sind, gemeinsam etwas zu verändern – egal, wo diese Grenzen liegen. 
        </p>
      </div>
      <div class="about-grid">
        <div class="about-img">
          <img src="Schmetterling.jpg" alt="">
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
        </div>
        <div class="about-img">
          <img src="Wasserfall.jpg" alt="">
        </div>
        <div class="about-text">
          <h3>Fortbildungen</h3>
          <p>
•	Neurodivergenz in der Ergotherapie (ergotherapie austria, 2026) <br>
•	Kreativ-Therapeutisches Schreiben in der Psychiatrie und Psychosomatik (tirol kliniken, 2026)<br>
•	Selbstwert – Selbstvertrauen – Selbstwirksamkeit (ergotherapie austria, 2025)<br>
•	Schlafcoaching (pro mente akademie, 2024)<br>
•	Traumasensibles Arbeiten in der Ergotherapie (ergotherapie austria, 2024)<br>
•	Angst- und Panikstörungen (pro mente akademie, 2024) <br>
•	Handeln ermöglichen – Trägheit überwinden (ergotherapie austria, 2022)
          </p>
        </div>
      </div>
    </div>
  </section>
  <section id="gallery">
    <div class="container">
      <div class="section-title">
        <h2 style="color: #045680">Was ist Ergotherapie</h2>
        <p>
          Ergotherapie hilft dabei, die eigene Handlungsfähigkeit wiederherzustellen. Denn wir Menschen sind im Grunde gerne tätig – wir haben Spaß an unseren alltäglichen Betätigungen (wenn auch an manchen mehr als an anderen), wir TUN gerne. 
        </p>
        <p>
          Sind diese bedeutungsvollen Aktivitäten nicht (mehr) möglich, kommt es zu gesundheitlichen Einschränkungen. Gemeinsam finden wir also Mittel und Wege, wie Sie Ihren Alltag so meistern können, dass Sie wieder mehr Zufriedenheit und Lebensqualität erleben können. 
        </p>
        <p>
          Das beinhaltet neben dem Training von persönlichen Fähigkeiten auch Adaptierungen Ihrer Betätigungen und Ihrer Umwelt, denn das alles spielt bei Beeinträchtigungen eine Rolle. 
        </p>
      </div>
    </div>
  </section>
  <section id="orga" style="text-align:left">
    <div class="container">
      <div class="section-title">
        <h2 style="color: #045680">Ablauf und Organisatorisches</h2>
        <p>
          Bevor Sie zu mir kommen, benötigen Sie eine Überweisung von Ihrer/Ihrem Haus- oder besser Ihrer/Ihrem Facharzt/-ärztin. Auf der Überweisung steht die Anzahl der Ergotherapie-Einheiten, die Dauer einer Einheit und ob Sie diese als Hausbesuche benötigen. 
        </p>
        <p>
          Mit dieser Überweisung melden Sie sich bei mir und wir vereinbaren einen Termin für das Erstgespräch. Darin entscheiden wir gemeinsam, woran wir in der Ergotherapie arbeiten und in welchem Abstand die Einheiten stattfinden. 
        </p>
        <p>
          Ich bin Wahltherapeutin, das bedeutet, dass Sie am Ende jeder Einheit direkt bei mir in der Praxis bezahlen (in bar oder mit Karte) und die Rechnung im Anschluss selbst bei Ihrer Krankenkassa einreichen. Von der Krankenkassa erhalten Sie dann einen Anteil der Kosten rückerstattet. 
        </p><br>
        <div class="orga-text">
          <h3>Kosten</h3>
          <p>Die Dauer einer Ergotherapie-Einheit wird von der/vom zuständigen Arzt/Ärztin bereits auf die Überweisung geschrieben. Üblich sind v.a. 45 und 60 Minuten Einheiten. Bei geringer Konzentrationsfähigkeit können manchmal auch 30 Minuten Einheiten sinnvoll sein.</p>
          <p>Für eine 45 Minuten Einheit verrechne ich 75€, für 60 Minuten 100€. </p>
          <p>Für Hausbesuche verrechne ich zusätzlich zum oben genannten Honorar einen Pauschalbetrag von 30€ pro Termin.</p> 
          <p>Angehörigengespräche, Vernetzungen mit anderen Berufsgruppen oder dem schulischen/beruflichen Umfeld kann ich nach Absprache mit Ihnen ohne selbstständig ärztliche Zuweisung durchführen und werden ebenfalls verrechnet (20€ pro 15 Minuten). Auch dafür gibt es eine teilweise Kostenrückerstattung von der Krankenkasse. </p>
          <br>
          <h3>Was passiert bei den einzelnen Terminen?</h3>
          <p>Die erste Einheit verwende ich für ein ausführliches Gespräch, in dem ich mir ein Bild von Ihnen, Ihrem Alltag und Ihrem Umfeld mache. Wir suchen gemeinsam nach den Betätigungen, die Ihnen nicht (mehr) gelingen wollen, und einigen uns auf ein Therapieziel. </p>
          <p>Die folgenden Therapieeinheiten arbeiten wir gemeinsam daran, dieses Ziel zu erreichen. Das kann durch Gespräche und Beratung erfolgen, durch eine Analyse der Betätigungen, die Ihnen wichtig sind, oder durch kreative Prozesse. Ergotherapie heißt Tun, daher fokussiere ich mich immer wieder mit Ihnen auf die Betätigungen, die Ihnen wichtig sind. Das kann manchmal auch bedeuten, dass wir gemeinsam genau diese Aktivitäten durchführen, um sie zu üben oder auf eventuelle Hindernisse zu untersuchen. 
          </p>
        </div>
      </div>
    </div>
  </section>
  <section id="contact">
    <div class="container">
      <div class="section-title">
        <h2 style="color: #045680">Kontakt</h2>
        <p>
          Ich freue mich auf Ihre Anfrage und berate Sie gerne persönlich.
        </p>
      </div>
      <div class="contact-wrapper">
        <div class="contact-box">
          <h3>Praxisinformationen</h3>
          <div class="contact-info">
            <p><strong>Barbara Weinold – Ergotherapie | praxis andersrum</strong></p>
            <p>Musterstraße 24<br>1010 Wien</p>
            <p>+43 660 1234567</p>
            <p>kontakt@barbara-weinold.at</p>
            <p>Mo – Fr: 08:00 – 18:00 Uhr</p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <footer>
    <div class="container">
      <p>
        © 2026 Barbara Weinold – Ergotherapie | praxis andersrum
      </p>
    </div>
  </footer>
</body>
</html>
