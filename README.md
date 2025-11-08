<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Protocolo Ciero Vientre</title>
  <meta name="description" content="Protocolo Ciero Vientre — Método natural para reducir grasa abdominal y recuperar la confianza.">
  
  <!-- Favicon (SVG data URI) -->
  <link rel="icon" href="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><path fill='%23ff9966' d='M50 10c-8 0-15 6-15 14s7 14 15 14 15-6 15-14S58 10 50 10z'/><path fill='%23ff5e99' d='M50 44c-12 0-22 10-22 22v6h44v-6c0-12-10-22-22-22z'/></svg>" />

  <style>
    /* Fonte base */
    :root{
      --pink:#ff5e99;
      --orange:#ff9966;
      --white: #ffffff;
      --card-bg: rgba(255,255,255,0.12);
      --glass: rgba(255,255,255,0.06);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: "Helvetica Neue", Arial, sans-serif;
      background: linear-gradient(180deg,var(--orange),var(--pink));
      color:var(--white);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    /* HEADER / LOGO */
    header{
      display:flex;
      align-items:center;
      gap:16px;
      padding:22px 20px;
      max-width:1100px;
      margin:0 auto;
    }
    .logo {
      display:flex;
      align-items:center;
      gap:12px;
      text-decoration:none;
      color:var(--white);
    }
    .logo svg{width:56px;height:56px;flex-shrink:0}
    .brand {
      display:flex;
      flex-direction:column;
      line-height:1;
    }
    .brand .title{font-weight:700;font-size:1.25rem;letter-spacing:0.2px}
    .brand .subtitle{font-weight:400;font-size:0.85rem;opacity:0.95;margin-top:2px}

    /* MAIN CONTAINER */
    .wrap{
      max-width:1100px;
      margin:18px auto 60px;
      padding:22px;
    }
    .card{
      background:var(--white);
      color:#222;
      border-radius:18px;
      padding:18px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.12);
    }

    /* VIDEO */
    .video-wrap{
      display:flex;
      justify-content:center;
      margin:0 auto;
      padding-top:10px;
    }
    /* Ensures video is responsive */
    vturb-smartplayer, .video-iframe {
      width:100%;
      max-width:900px;
      border-radius:12px;
      overflow:hidden;
      display:block;
    }

    /* CTA Button */
    .cta {
      display:flex;
      justify-content:center;
      margin-top:18px;
    }
    .btn-primary{
      background: linear-gradient(90deg,var(--orange),var(--pink));
      color:var(--white);
      border:none;
      padding:14px 28px;
      border-radius:999px;
      font-weight:700;
      font-size:1rem;
      cursor:pointer;
      box-shadow: 0 8px 20px rgba(255,94,153,0.22);
      transition: transform .14s ease, box-shadow .14s ease, opacity .12s;
      text-decoration:none;
      display:inline-flex;
      align-items:center;
      gap:10px;
    }
    .btn-primary:hover{transform:translateY(-3px)}
    .btn-secondary{
      background:transparent;
      color:var(--pink);
      border:2px solid var(--pink);
      padding:10px 18px;
      border-radius:999px;
      font-weight:700;
      cursor:pointer;
      margin-left:12px;
    }

    /* Benefits */
    .benefits{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
      gap:12px;
      margin-top:18px;
    }
    .benefit{
      background:var(--card-bg);
      padding:14px;
      border-radius:12px;
      text-align:left;
    }
    .benefit h4{margin:0 0 6px 0;color:#fff}
    .benefit p{margin:0;opacity:0.95;color:#fff;font-size:0.95rem}

    /* Testimonios (texto sólo) */
    .testimonios{
      margin-top:22px;
      padding:18px;
      background:var(--glass);
      border-radius:12px;
      color:var(--white);
    }
    .testimonios h3{margin:0 0 12px 0;font-size:1.25rem}
    .ts-grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(240px,1fr));
      gap:12px;
    }
    .ts{
      background:rgba(255,255,255,0.04);
      padding:12px 14px;
      border-radius:10px;
      text-align:left;
    }
    .ts p{margin:0 0 8px 0; font-style:italic; color: #fff;}
    .ts .who{font-weight:700;color:#fff;font-size:0.95rem;opacity:0.95}

    footer{
      max-width:1100px;
      margin:28px auto 60px;
      text-align:center;
      color:rgba(255,255,255,0.9);
      font-size:0.9rem;
      opacity:0.95;
    }

    /* Floating purchase button for mobile */
    .floating-buy{
      display:none;
      position:fixed;
      left:50%;
      transform:translateX(-50%);
      bottom:18px;
      z-index:9999;
      border-radius:999px;
      padding:12px 20px;
      background:linear-gradient(90deg,var(--orange),var(--pink));
      color:#fff;
      font-weight:700;
      box-shadow:0 12px 30px rgba(0,0,0,0.25);
      text-decoration:none;
    }
    @media (max-width:900px){
      header{padding:14px 16px}
      .brand .title{font-size:1.05rem}
      .video-wrap{padding:6px}
    }
    @media (max-width:700px){
      .floating-buy{display:inline-block}
    }
  </style>

  <!-- Meta Pixel Code (já com o seu ID) -->
  <script>
    !function(f,b,e,v,n,t,s)
    {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
    n.callMethod.apply(n,arguments):n.queue.push(arguments)};
    if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
    n.queue=[];t=b.createElement(e);t.async=!0;
    t.src=v;s=b.getElementsByTagName(e)[0];
    s.parentNode.insertBefore(t,s)}(window, document,'script',
    'https://connect.facebook.net/en_US/fbevents.js');
    fbq('init', '1752998905374672');
    fbq('track', 'PageView');
  </script>
  <noscript>
    <img height="1" width="1" style="display:none"
      src="https://www.facebook.com/tr?id=1752998905374672&ev=PageView&noscript=1"/>
  </noscript>
  <!-- End Meta Pixel Code -->

</head>
<body>

  <!-- HEADER com LOGO (ícone + texto) -->
  <header>
    <a class="logo" href="/">
      <!-- Ícone SVG similar ao favicon -->
      <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg" aria-hidden="true" focusable="false">
        <path fill="#ff9966" d="M50 10c-8 0-15 6-15 14s7 14 15 14 15-6 15-14S58 10 50 10z"/>
        <path fill="#ff5e99" d="M50 44c-12 0-22 10-22 22v6h44v-6c0-12-10-22-22-22z"/>
      </svg>
      <div class="brand">
        <div class="title">Protocolo Ciero Vientre</div>
        <div class="subtitle">21 días — método natural y comprobado</div>
      </div>
    </a>
  </header>

  <main class="wrap">
    <div class="card">

      <!-- VIDEO VTURB -->
      <div class="video-wrap">
        <vturb-smartplayer id="vid-690e2f041a078823fdadef1c" style="display:block;width:100%;max-width:960px;"></vturb-smartplayer>
        <script type="text/javascript">
          var s=document.createElement("script");
          s.src="https://scripts.converteai.net/b54b1210-b65c-436b-ae22-a4d4fda71a39/players/690e2f041a078823fdadef1c/v4/player.js";
          s.async=!0;document.head.appendChild(s);
        </script>
      </div>

      <!-- CTA -->
      <div class="cta" style="margin-top:20px;">
        <a class="btn-primary"
           href="https://pay.hotmart.com/X102804891T?off=27ogaj6g&checkoutMode=10"
           onclick="fbq('track','InitiateCheckout');">
           💥 QUIERO MI ACCESO AHORA
        </a>
        <a class="btn-secondary" href="#testimonios">Leer testimonios</a>
      </div>

      <!-- BENEFICIOS / RESUMEN -->
      <div class="benefits" style="margin-top:22px;">
        <div class="benefit">
          <h4>🔥 Resultados visibles</h4>
          <p>Reducción de centímetros en la cintura con un enfoque saludable.</p>
        </div>
        <div class="benefit">
          <h4>🥗 Alimentación inteligente</h4>
          <p>Comidas y recetas prácticas para acelerar tu metabolismo.</p>
        </div>
        <div class="benefit">
          <h4>⏱ Rutinas cortas</h4>
          <p>Ejercicios rápidos y efectivos que se adaptan a tu día a día.</p>
        </div>
      </div>

      <!-- Testimonios (texto) -->
      <section id="testimonios" class="testimonios" aria-label="Testimonios">
        <h3>Historias reales de transformación</h3>
        <div class="ts-grid">
          <div class="ts">
            <p>"Nunca imaginé que pudiera sentirme tan bien conmigo misma. Perdí 8 kilos en solo 4 semanas."</p>
            <div class="who">– María, 34 años</div>
          </div>
          <div class="ts">
            <p>"El Protocolo Ciero Vientre cambió mi vida. Mi abdomen está más plano y tengo más energía."</p>
            <div class="who">– Lucía, 29 años</div>
          </div>
          <div class="ts">
            <p>"Después de dos embarazos, logré volver a mi talla ideal sin dietas extremas."</p>
            <div class="who">– Carla, 38 años</div>
          </div>
          <div class="ts">
            <p>"Lo recomiendo totalmente. Es sencillo, efectivo y los resultados se notan rápido."</p>
            <div class="who">– Elena, 41 años</div>
          </div>
        </div>
      </section>

    </div> <!-- /card -->
  </main>

  <!-- Floating buy (mobile) -->
  <a class="floating-buy"
     href="https://pay.hotmart.com/X102804891T?off=27ogaj6g&checkoutMode=10"
     onclick="fbq('track','InitiateCheckout');">
     💥 OBTÉN ACCESO AHORA
  </a>

  <footer>
    © 2025 Protocolo Ciero Vientre — Todos los derechos reservados
  </footer>

  <script>
    /* Pequena melhoria: se o usuário clicar no botão principal, também enviar 'Purchase' se quiser
       (por enquanto 'InitiateCheckout' é rastreado para tráfego; o evento 'Purchase' deve ser enviado
       quando a venda efetiva acontecer — idealmente via webhook, Pixel no checkout ou integração da Hotmart) */
    // Se quiser enviar 'Purchase' no clique (menos preciso), substitua InitiateCheckout pelo evento 'Purchase'.
  </script>
</body>
</html>
