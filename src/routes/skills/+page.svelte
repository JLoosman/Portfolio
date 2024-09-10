<section class="hero">
  <h1>Skills</h1>
</section>
<section class="skills">
  <table>
    <tr>
      <td>Programmiersprachen</td>
      <td>Skill-Level</td>
    </tr>
    <tr>
      <td>HTML & CSS</td>
      <td>5 ⚪ ⚪ ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>JavaScript</td>
      <td>4 ⚪ ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>Java</td>
      <td>4 ⚪ ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>PHP</td>
      <td>3 ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>Phython</td>
      <td>3 ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>C++</td>
      <td>1 ⚪</td>
    </tr>
  </table>
  <table>
    <tr>
      <td>Betriebssysteme</td>
      <td>Skill-Level</td>
    </tr>
    <tr>
      <td>Windows</td>
      <td>4 ⚪ ⚪ ⚪ ⚪ </td>
    </tr>
    <tr>
      <td>Linux</td>
      <td>4 ⚪ ⚪ ⚪ ⚪</td>
    </tr>
  </table>
  <table>
    <tr>
      <td>Docker</td>
      <td>3 ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>Git & GitHub</td>
      <td>3 ⚪ ⚪ ⚪</td>
    </tr>
  </table>
  <table>
    <tr>
      <td>Datenbanken</td>
      <td>Skill-Level</td>
    </tr>
    <tr>
      <td>MySQL</td>
      <td>4 ⚪ ⚪ ⚪ ⚪</td>
    </tr>
    <tr>
      <td>MongoDB</td>
      <td>3 ⚪ ⚪ ⚪</td>
    </tr>
  </table>
  <table>
    <tr><td>Legende</td></tr>
    <tr>
      <td>1 Grundkenntnisse, wenig praktische Erfahrung</td>
    </tr>
    <tr>
      <td>2 Zusammenhänge, wenig praktische Erfahrung</td>
    </tr>
    <tr>
      <td>3 Mittlere Kenntnisse, praktische Erfahrungen</td>
    </tr>
    <tr>
      <td>4 Gute Kenntnisse, einige praktische Erfahrungen</td>
    </tr>
    <tr>
      <td>5 Sehr gute Kenntnisse, viel Erfahrung</td>
    </tr>
  </table>
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

  .skills {
    padding: 50px 200px;
    background-color: #000;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  table {
    width: 40vw;
    margin: 30px 0;
    border-collapse: collapse;
    table-layout: fixed;
  }

  tr {
    height: 35px;
  }

  td {
    padding: 5px;
    border: 1px solid #fff;
    color: #fff;
  }

  @media only screen and (max-width: 990px) {
    table {
      width: 70vw;
      table-layout: auto;
    }
  }
</style>
