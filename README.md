<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Cambios y Soluciones</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    :root {
      --bg: #0f172a;
      --card: #1e293b;
      --text: #e2e8f0;
      --accent: #60a5fa;
      --muted: #94a3b8;
      --radius: 12px;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      padding: 1.5rem;
      font-family: Inter, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.6;
    }

    .container {
      max-width: 920px;
      margin: auto;
      padding: 1.5rem;
      background: rgba(255,255,255,0.03);
      border-radius: var(--radius);
      border: 1px solid rgba(255,255,255,0.05);
    }

    header {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      align-items: center;
      gap: 1rem;
    }

    .brand {
      display: flex;
      gap: .75rem;
      align-items: center;
    }

    .logo {
      width: 48px;
      height: 48px;
      border-radius: 8px;
      background: rgba(255,255,255,0.05);
      display: grid;
      place-items: center;
      font-weight: 700;
      color: var(--accent);
    }

    nav a {
      color: var(--text);
      text-decoration: none;
      padding: .4rem .7rem;
      border-radius: 8px;
      font-weight: 600;
      transition: .2s;
    }
    nav a:hover {
      background: rgba(255,255,255,0.06);
    }

    main {
      display: grid;
      grid-template-columns: 1fr 260px;
      gap: 1rem;
      margin-top: 1rem;
    }

    article, aside {
      background: var(--card);
      padding: 1rem;
      border-radius: var(--radius);
    }

    .media img {
      width: 100%;
      border-radius: 8px;
      margin-top: .75rem;
    }

    aside h3 {
      margin-top: 0;
      color: var(--accent);
    }

    footer {
      text-align: center;
      margin-top: 1rem;
      color: var(--muted);
      font-size: .9rem;
    }

    @media (max-width: 850px) {
      main { grid-template-columns: 1fr; }
      nav { width: 100%; text-align: center; }
    }
  </style>
</head>

<body>
  <div class="container">

    <header>
      <div class="brand">
        <div class="logo">CS</div>
        <div>
          <h1 style="margin:0;">Cambios y Soluciones</h1>
          <small style="color:var(--muted)">Reflexiones para un mundo mejor</small>
        </div>
      </div>

      <nav>
        <a href="https://youtu.be/SH5Hj7-Cxu0" target="_blank">Historia de V</a>
        <a href="https://youtu.be/dNbIBZnWam8" target="_blank">Rap sobre poder</a>
      </nav>
    </header>

    <main>
      <article>
        <h2 style="color:var(--accent)">Historia de Punisher</h2>

        <p>Frank Castle es un exmarine cuya vida cambió cuando su familia fue asesinada por la mafia. Tras sobrevivir, juró vengarse de sus responsables.</p>

        <p>Desde entonces libra una guerra personal contra el crimen, usando métodos extremos que lo colocan fuera de la ley.</p>

        <div class="media">
          <img src="imagenes/punisher.jpg" alt="Imagen representativa de Punisher">
        </div>

        <p>A menudo colabora o choca con héroes como Spider-Man o Daredevil, quienes critican sus métodos radicales.</p>

        <p>Para Castle, la lucha termina solo con su muerte. No busca fama ni seguidores: su misión es totalmente personal.</p>
      </article>

      <aside>
        <h3>Videos recomendados</h3>

        <p><a href="https://youtu.be/SH5Hj7-Cxu0" target="_blank" style="color:var(--text)">Historia de V de Venganza</a></p>
        <p><a href="https://youtu.be/dNbIBZnWam8" target="_blank" style="color:var(--text)">Rap sobre abuso de poder</a></p>

        <hr style="opacity:0.1">

        <h3>Consejos</h3>
        <ul style="color:var(--muted); padding-left:1rem;">
          <li>Usa rutas relativas para tus imágenes.</li>
          <li>Añade atributos <code>alt</code> para accesibilidad.</li>
          <li>Evita rutas locales de tu PC.</li>
        </ul>
      </aside>
    </main>

    <footer>
      © <span id="year"></span> Cambios y Soluciones
    </footer>

  </div>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>

</body>
</html>
