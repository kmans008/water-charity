<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Next Generation Charity — Water Edition</title>
  <!-- Google Fonts (free) -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    /* =============================
       Beginner-friendly CSS only
       ============================= */
    :root{
      /* Teal brand taken from your Canva mock */
      --teal: #6c9aa5;        /* card background */
      --teal-dark: #3f6c76;   /* accents */
      --ink: #0e1c22;         /* heading/body text on teal */
      --paper: #f3f6f7;       /* page background */
      --accent: #ffd028;      /* donate yellow */
      --muted: #6b7b83;       /* helper text */
      --radius-lg: 24px;
    }

    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body{
      margin:0;
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      background: var(--paper);
      color: var(--ink);
      display:grid;
      place-items:center;
      padding: 28px 16px;
    }

    /* Phone-first canvas that matches your tall design */
    .card{
      width: 100%;
      max-width: 420px; /* close to an IG story width */
      background: var(--teal);
      border-radius: var(--radius-lg);
      box-shadow: 0 20px 40px rgba(7,33,44,.18);
      overflow: hidden;
    }

    .card-inner{ padding: 28px 24px 24px; }

    .eyebrow{
      letter-spacing: .06em;
      text-transform: uppercase;
      font-weight: 700;
      color: var(--ink);
      opacity:.95;
      font-size: 13px;
    }

    h1{
      font-family: "Playfair Display", serif;
      font-weight: 700;
      font-size: 28px;
      line-height: 1.15;
      margin: 8px 0 4px;
      color: var(--ink);
      text-transform: uppercase;
      text-align:center;
    }

    .subhead{
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing:.06em;
      font-size: 12px;
      color: var(--ink);
      text-align:center;
      margin-top: 6px;
    }

    .lede{ 
      margin: 14px auto 10px;
      max-width: 35ch;
      font-size: 13.5px;
      line-height: 1.4;
      text-align:center;
      color: #0f2229; /* darker for contrast on teal */
    }

    .media{
      position: relative;
      display:flex;
      justify-content:center;
      margin: 14px 0 4px;
    }

    /* Circular image mask like your Canva layout */
    .media .photo{
      width: 70%;
      aspect-ratio: 1/1;
      background: #cfd8dc;
      border-radius: 50%;
      overflow: hidden;
      box-shadow: 0 12px 28px rgba(0,0,0,.18);
    }
    .media .photo img{
      width:100%;
      height:100%;
      object-fit: cover;
      display:block;
      filter: grayscale(100%);
    }

    /* Yellow callout badge that overlaps the circle */
    .cta-badge{
      position: absolute;
      right: 12%;
      bottom: 10%;
      background: var(--accent);
      color: #1a1600;
      font-weight: 800;
      text-transform: uppercase;
      font-size: 12px;
      letter-spacing: .06em;
      padding: 12px 14px;
      border-radius: 28px;
      box-shadow: 0 8px 18px rgba(0,0,0,.18);
      border: 2px solid rgba(0,0,0,.05);
      text-align:center;
      white-space: nowrap;
    }

    /* Primary donate button */
    .cta{
      display:block;
      width: fit-content;
      margin: 10px auto 0;
      background: var(--ink);
      color: white;
      text-decoration: none;
      font-weight: 700;
      letter-spacing: .02em;
      padding: 12px 18px;
      border-radius: 999px;
      box-shadow: 0 10px 20px rgba(0,0,0,.18);
    }
    .cta:hover{ filter: brightness(1.03); }

    /* Tagline + tiny url like your footer line */
    .tagline{
      text-align:center;
      margin: 16px 0 6px;
      font-weight: 700;
      letter-spacing: .06em;
      text-transform: uppercase;
      font-size: 11px;
      color: #0c1a21;
    }
    .tiny-url{
      text-align:center;
      font-size: 11px;
      color: #12313a;
      margin-bottom: 6px;
      opacity:.9;
    }

    /* Simple footer with secondary links (optional) */
    footer{
      padding: 14px 18px 22px;
      text-align:center;
      color: var(--muted);
      font-size: 12px;
    }
    footer a{ color: var(--muted); text-decoration: none; }

    /* Small screens are default; give the hero a bit more air on larger ones */
    @media (min-width: 720px){
      .card{ max-width: 520px; }
      h1{ font-size: 32px; }
      .lede{ font-size: 14px; }
    }
  </style>
</head>
<body>

  <main class="card" role="main">
    <div class="card-inner">
      <p class="eyebrow" aria-hidden="true">Next Generation Charity</p>
      <h1>NEXT GENERATION<br/>CHARITY</h1>
      <p class="subhead">WATER EDITION</p>

      <p class="lede">
        We provide clean water to less fortunate people who don’t have access to safe, reliable water. Your gift builds wells, installs filters, and funds local jobs.
      </p>

      <div class="media" aria-hidden="true">
        <div class="photo">
          <!-- Placeholder image — replace with your own asset -->
          <img src="https://images.unsplash.com/photo-1488521787991-ed7bbaae773c?q=80&w=1200&auto=format&fit=crop" alt="Children smiling near a water source" />
        </div>
        <span class="cta-badge">Donate Now</span>
      </div>

      <a class="cta" href="#donate">Give Clean Water</a>

      <p class="tagline">Be the Difference</p>
      <p class="tiny-url">www.reallygreatsite.com</p>
    </div>

    <footer>
      <small>
        © <span id="y">2025</span> Next Generation Charity · <a href="#impact">Impact</a> · <a href="#about">About</a> · <a href="#contact">Contact</a>
      </small>
    </footer>
  </main>

  <script>
    // purely cosmetic: keep the year current without any libraries
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
