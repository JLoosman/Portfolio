<script>
  import { Lightbox } from "svelte-lightbox";
  import { reveal } from "svelte-reveal";

  let revealConfig = {
    preset: "slide",
    y: 40,
    x: 0,
    opacity: 0,
    duration: 600,
    blur: 0,
  };
</script>

<section class="hero">
  <h1>Projekte</h1>
</section>

<section class="projects">
  <div class="project">
    <div use:reveal={revealConfig} class="title">
      <h2>Todo</h2>
      <a href="https://jloosman.github.io/todo-svelte/" target="_blank">
        <svg
          width="30px"
          height="30px"
          viewBox="0 0 1024 1024"
          fill="currentColor"
          x="128"
          y="128"
          role="img"
          style="display:inline-block;vertical-align:middle"
          xmlns="http://www.w3.org/2000/svg"
          ><g fill="currentColor"
            ><path
              fill="#eee"
              d="M574 665.4a8.03 8.03 0 0 0-11.3 0L446.5 781.6c-53.8 53.8-144.6 59.5-204 0c-59.5-59.5-53.8-150.2 0-204l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3l-39.8-39.8a8.03 8.03 0 0 0-11.3 0L191.4 526.5c-84.6 84.6-84.6 221.5 0 306s221.5 84.6 306 0l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3L574 665.4zm258.6-474c-84.6-84.6-221.5-84.6-306 0L410.3 307.6a8.03 8.03 0 0 0 0 11.3l39.7 39.7c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c53.8-53.8 144.6-59.5 204 0c59.5 59.5 53.8 150.2 0 204L665.3 562.6a8.03 8.03 0 0 0 0 11.3l39.8 39.8c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c84.5-84.6 84.5-221.5 0-306.1zM610.1 372.3a8.03 8.03 0 0 0-11.3 0L372.3 598.7a8.03 8.03 0 0 0 0 11.3l39.6 39.6c3.1 3.1 8.2 3.1 11.3 0l226.4-226.4c3.1-3.1 3.1-8.2 0-11.3l-39.5-39.6z"
            /></g
          ></svg
        >
      </a>
    </div>
    <div use:reveal={revealConfig} class="line"></div>
    <p use:reveal={revealConfig}>
      Für das Informatik-Modul M294 mussten wir mithilfe von JavaScript eine
      CRUD-Webapplikation schreiben. Um dies möglichst effizient zu erledigen,
      habe ich mir vorgenommen, ein JavaScript-Framework zu benutzen.
      Entschieden habe ich mich schlussendlich für Svelte, welches ich mir dann
      auch in kürzester Zeit angeeignet habe. Die App ist insgesamt nicht
      sonderlich kompliziert, ist meiner Meinung nach aber trotzdem eine schöne
      App geworden, welche ideal funktioniert.
    </p>
  </div>
  <div class="project">
    <div use:reveal={revealConfig} class="title">
      <h2>Music Finder</h2>
      <a
        href="https://github.com/JLoosman/Spotify-Music-Finder"
        target="_blank"
      >
        <svg
          width="30px"
          height="30px"
          viewBox="0 0 1024 1024"
          fill="currentColor"
          x="128"
          y="128"
          role="img"
          style="display:inline-block;vertical-align:middle"
          xmlns="http://www.w3.org/2000/svg"
          ><g fill="currentColor"
            ><path
              fill="#eee"
              d="M574 665.4a8.03 8.03 0 0 0-11.3 0L446.5 781.6c-53.8 53.8-144.6 59.5-204 0c-59.5-59.5-53.8-150.2 0-204l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3l-39.8-39.8a8.03 8.03 0 0 0-11.3 0L191.4 526.5c-84.6 84.6-84.6 221.5 0 306s221.5 84.6 306 0l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3L574 665.4zm258.6-474c-84.6-84.6-221.5-84.6-306 0L410.3 307.6a8.03 8.03 0 0 0 0 11.3l39.7 39.7c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c53.8-53.8 144.6-59.5 204 0c59.5 59.5 53.8 150.2 0 204L665.3 562.6a8.03 8.03 0 0 0 0 11.3l39.8 39.8c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c84.5-84.6 84.5-221.5 0-306.1zM610.1 372.3a8.03 8.03 0 0 0-11.3 0L372.3 598.7a8.03 8.03 0 0 0 0 11.3l39.6 39.6c3.1 3.1 8.2 3.1 11.3 0l226.4-226.4c3.1-3.1 3.1-8.2 0-11.3l-39.5-39.6z"
            /></g
          ></svg
        >
      </a>
    </div>
    <div use:reveal={revealConfig} class="line"></div>
    <p use:reveal={revealConfig}>
      Music Finder ist eine Idee, die ich privat unbedingt ausprobieren wollte.
      Ich bediene mich dabei der Spotify API, um dem User basierend auf seinen
      Interessen neue Song- und Künstlervorschläge zu generieren. Dafür habe ich
      das Metaframework SvelteKit benutzt, um für meine App ein Backend zu
      erstellen. Dies ist das erste Mal, dass ich in solchem Umfang mit APIs
      gearbeitet habe, und ich hatte zunächst Probleme mit der
      Authentifizierung, die jedoch nun wunderbar funktioniert. Momentan kann
      ich diese Applikation leider noch nicht hosten, da ich bei Spotify zuerst
      eine Veröffentlichung beantragen müsste und dafür noch einige
      Design-Guidelines beachten müsste. Finde ich dafür in der Zukunft Zeit,
      werde ich dies allerdings mit Sicherheit erledigen.
    </p>
    <div use:reveal={revealConfig} class="images">
      <Lightbox>
        <img src="./SpotifyApp.png" alt="A screenshot of my application" />
      </Lightbox>
      <Lightbox>
        <img src="./SpotifyApp2.png" alt="A screenshot of my application" />
      </Lightbox>
    </div>
    <p use:reveal={revealConfig}>
      Wie Sie hier sehen können, basiert meine Applikation auf einem einfachen
      Design, inspiriert von Tinder, um dem Nutzer neue Songs und Künstler
      vorzuschlagen. Einerseits werden die momentan bekanntesten Songs
      vorgeschlagen, andererseits werden Liedervorschläge auf Grundlage Ihrer
      Lieblingssongs generiert.
    </p>
  </div>
  <div class="project last">
    <div use:reveal={revealConfig} class="title">
      <h2>Web Hosting</h2>
      <a href="https://github.com/JLoosman/Portfolio" target="_blank">
        <svg
          width="30px"
          height="30px"
          viewBox="0 0 1024 1024"
          fill="currentColor"
          x="128"
          y="128"
          role="img"
          style="display:inline-block;vertical-align:middle"
          xmlns="http://www.w3.org/2000/svg"
          ><g fill="currentColor"
            ><path
              fill="#eee"
              d="M574 665.4a8.03 8.03 0 0 0-11.3 0L446.5 781.6c-53.8 53.8-144.6 59.5-204 0c-59.5-59.5-53.8-150.2 0-204l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3l-39.8-39.8a8.03 8.03 0 0 0-11.3 0L191.4 526.5c-84.6 84.6-84.6 221.5 0 306s221.5 84.6 306 0l116.2-116.2c3.1-3.1 3.1-8.2 0-11.3L574 665.4zm258.6-474c-84.6-84.6-221.5-84.6-306 0L410.3 307.6a8.03 8.03 0 0 0 0 11.3l39.7 39.7c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c53.8-53.8 144.6-59.5 204 0c59.5 59.5 53.8 150.2 0 204L665.3 562.6a8.03 8.03 0 0 0 0 11.3l39.8 39.8c3.1 3.1 8.2 3.1 11.3 0l116.2-116.2c84.5-84.6 84.5-221.5 0-306.1zM610.1 372.3a8.03 8.03 0 0 0-11.3 0L372.3 598.7a8.03 8.03 0 0 0 0 11.3l39.6 39.6c3.1 3.1 8.2 3.1 11.3 0l226.4-226.4c3.1-3.1 3.1-8.2 0-11.3l-39.5-39.6z"
            /></g
          ></svg
        >
      </a>
    </div>
    <div use:reveal={revealConfig} class="line"></div>
    <p use:reveal={revealConfig}>
      Um diese Portfolio-Seite für Sie verfügbar zu machen, miete ich einen VPS
      auf der Cloud-Plattform DigitalOcean. Darauf läuft ein Ubuntu-Server, den
      ich als Webserver eingerichtet habe. In der Vergangenheit habe ich diesen
      von Hand mit Nginx eingerichtet, nun nutze ich jedoch ein Tool namens
      Coolify, welches das Hosten von Webseiten und Webapplikationen deutlich
      vereinfacht.
    </p>
  </div>
</section>

<style>
  .hero {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  h1 {
    color: #eee;
    font-size: 100px;
  }

  h2 {
    color: #eee;
    font-size: 30px;
  }

  p {
    margin: 20px;
    color: #eee;
    font-size: 20px;
    line-height: 1.5;
    text-align: center;
  }

  img {
    cursor: pointer;
    width: 95%;
    display: block;
    margin: 5px auto;
  }

  .projects {
    padding: 50px 200px;
    background-color: #000;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .last {
    margin-bottom: 0 !important;
  }

  .project {
    width: 700px;
    margin-bottom: 150px;
  }

  .title {
    padding: 10px 20px;
    display: flex;
    justify-content: space-between;
  }

  .line {
    height: 3px;
    width: 100%;
    background-color: #eee;
  }

  .images {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
  }

  @media only screen and (max-width: 790px) {
    .projects {
      padding: 50px 0;
    }
    .project {
      width: clamp(80vw, 50vw, 700px);
    }

    .images {
      flex-direction: column;
    }
  }
</style>
