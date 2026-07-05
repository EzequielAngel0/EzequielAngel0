<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=2B6FB5&center=true&vCenter=true&width=700&lines=Angel+Ezequiel+Barbosa+Lomeli;Full+Stack+%26+Cross-Platform+Developer;Go+%7C+Flutter+%7C+React+%7C+OCI;From+first+commit+to+production" alt="Typing SVG"/>

<a href="https://www.linkedin.com/in/angelezequiel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://ezequielangel0.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-2B6FB5?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="mailto:angelbarbosa@angelezequiel.dev"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://x.com/Ezequiel27Angel"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"/></a>

<br>

<img src="https://img.shields.io/badge/Open_to_Work-2EA043?style=for-the-badge&logo=briefcase&logoColor=white" alt="Open to Work"/>
<img src="https://komarev.com/ghpvc/?username=EzequielAngel0&style=flat-square&color=2b6fb5" alt="Profile views"/>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## About Me &nbsp;/&nbsp; Sobre mí

<table>
<tr>
<td valign="top" width="50%">

<b>EN</b>

I design, build, and operate complete systems end-to-end, often solo. My flagship work, <b>ACP Suite</b>, runs in production on Oracle Cloud: a Go backend, a React admin panel, a Next.js public site, and four offline-first Flutter apps, provisioned with Terraform/Ansible and shipped through a CI/CD pipeline with security gates. Oracle Next Education (ONE) Tech Advanced graduate (Back-End track), OCI Certified Foundations Associate, Google Cloud Cybersecurity certified, and Software Development student at CETI.

</td>
<td valign="top" width="50%">

<b>ES</b>

Diseño, construyo y opero sistemas completos de punta a punta, frecuentemente en solitario. Mi trabajo insignia, <b>ACP Suite</b>, corre en producción sobre Oracle Cloud: backend en Go, panel admin en React, sitio público en Next.js y cuatro apps Flutter offline-first, aprovisionado con Terraform/Ansible y publicado con un pipeline CI/CD con gates de seguridad. Graduado del programa Oracle Next Education (ONE), ruta Back-End y nivel Tech Advanced, certificado OCI Foundations Associate y Google Cloud Cybersecurity, y estudiante de Desarrollo de Software en el CETI.

</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## Featured Projects &nbsp;/&nbsp; Proyectos Destacados

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>ACP Suite &nbsp;<img src="https://img.shields.io/badge/LIVE_IN_PRODUCTION-2EA043?style=flat-square" alt="Live"/></h3>
      <p>End-to-end ticketing &amp; parcel platform for an intercity bus company, <b>live in production on Oracle Cloud</b>. Built solo, replacing fully manual operations: two Go APIs (RBAC, audited mutations, transactional sales), a React admin panel, a Next.js public site, and four <b>offline-first</b> Flutter apps (ticket office, driver, parcels, customer) sharing in-house design-system, API-client, and ESC/POS thermal-printing packages.</p>
      <p>
        <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white"/>
        <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
        <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
        <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white"/>
        <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white"/>
        <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white"/>
        <img src="https://img.shields.io/badge/Podman-892CA0?style=flat-square&logo=podman&logoColor=white"/>
        <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
        <img src="https://img.shields.io/badge/Oracle_Cloud-F80000?style=flat-square&logo=oracle&logoColor=white"/>
      </p>
      <details>
        <summary><b>Architecture highlights / Detalles técnicos</b></summary>
        <ul>
          <li>In-house auth built from scratch: JWT (RS256), mandatory TOTP 2FA (RFC 6238), rotated refresh tokens with real session revocation.</li>
          <li>Offline-first field ops: AES-256-GCM encrypted queues, on-device folio generation, offline QR ticket validation (ES256), photo + signature delivery evidence.</li>
          <li>Pure-Dart ESC/POS printing library (tickets, waybills, shift reports, native QR) over Windows spooler, TCP/IP, and Bluetooth.</li>
          <li>Payments: Stripe, Mercado Pago &amp; PayPal via direct HTTP, webhook-verified confirmation, automatic order expiration, feature-flagged rollout.</li>
          <li>Infra as code: Terraform + Ansible on OCI (4 VMs + load balancer, PostgreSQL primary/replica, PgBouncer, Cloudflare tunnel, hardened nginx).</li>
          <li>CI/CD: multi-arch image builds with a vulnerability gate (Trivy, 0 HIGH/CRIT), SBOM, rolling deploys via self-hosted runner.</li>
          <li>Quality: 150+ automated tests, 40-step API E2E, Playwright UI E2E with real 2FA enrollment, k6 load baseline (public API p95 &lt; 100 ms), PII anonymization (LFPDPPP).</li>
        </ul>
      </details>
      <p><i>Private repository (client project). Architecture case study available on request.</i></p>
    </td>
    <td width="50%" valign="top">
      <h3>SoloKey</h3>
      <p>Zero-trust, offline-first password manager for Android. Military-grade cryptography (Argon2id, AES-256-GCM) secured via the native Android KeyStore, a built-in TOTP (2FA) generator, and a real-time weak password auditing system, all built on Clean Architecture.</p>
      <p>
        <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
        <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white"/>
        <img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white"/>
        <img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white"/>
      </p>
      <p><a href="https://github.com/EzequielAngel0/SoloKey">github.com/EzequielAngel0/SoloKey</a></p>
    </td>
  </tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## Tech Stack & Tools

<div align="center">

<b>Languages</b><br>
<img src="https://skillicons.dev/icons?i=go,dart,ts,java,python,cs" alt="Languages"/>

<b>Frameworks & Frontend</b><br>
<img src="https://skillicons.dev/icons?i=flutter,react,nextjs,spring,angular,dotnet,nodejs" alt="Frameworks"/>

<b>Databases</b><br>
<img src="https://skillicons.dev/icons?i=postgres,mysql,sqlite,mongodb" alt="Databases"/>

<b>Cloud, DevOps & Tools</b><br>
<img src="https://skillicons.dev/icons?i=terraform,ansible,docker,githubactions,nginx,cloudflare,git,github,linux" alt="Tools"/>
<br>
<img src="https://img.shields.io/badge/Podman-892CA0?style=for-the-badge&logo=podman&logoColor=white" height="40"/>
<img src="https://img.shields.io/badge/Oracle_Cloud-F80000?style=for-the-badge&logo=oracle&logoColor=white" height="40"/>
<img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" height="40"/>
<img src="https://img.shields.io/badge/k6-7D64FF?style=for-the-badge&logo=k6&logoColor=white" height="40"/>

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## Certifications &nbsp;/&nbsp; Certificaciones

<div align="center">

<a href="https://www.credly.com/badges/6b602da5-95ea-4328-a5dd-03ba538dfbf9/linked_in_profile"><img src="https://img.shields.io/badge/Google_Cloud_Cybersecurity_Certificate-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" alt="Google Cloud Cybersecurity Certificate"/></a>
<a href="https://catalog-education.oracle.com/ords/certview/sharebadge?id=9E6AA54792091B7F8EAD1C3D4C0E00B4640759558EA9319193256E348344778E"><img src="https://img.shields.io/badge/OCI_2025_Certified_Foundations_Associate-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="OCI Foundations Associate"/></a>
<a href="https://app.aluracursos.com/program/certificate/8a039e9d-447c-4d64-9a32-40a020f15bf5?lang"><img src="https://img.shields.io/badge/ONE_Tech_Advanced_G9_·_Back--End-2B6FB5?style=for-the-badge&logo=oracle&logoColor=white" alt="ONE Tech Advanced G9 Back-End"/></a>

</div>

## Currently Learning &nbsp;/&nbsp; Aprendiendo

<table>
<tr>
<td valign="top" width="40%">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/><br>
  <b>Python · FastAPI</b>
</td>
<td valign="top" width="60%">
  Expanding my backend toolbox into the Python ecosystem: REST services with <b>FastAPI</b>, async I/O, and Pydantic, applying the same architecture, testing, and security standards I use in Go.
  <br><br>
  <i>Ampliando mi backend al ecosistema Python: servicios REST con FastAPI, async I/O y Pydantic, con los mismos estándares de arquitectura, pruebas y seguridad que uso en Go.</i>
</td>
</tr>
</table>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>

## GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=EzequielAngel0&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats"/>
<img height="165" src="https://github-readme-streak-stats.herokuapp.com/?user=EzequielAngel0&theme=tokyonight&hide_border=true" alt="Streak"/>

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=EzequielAngel0&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages"/>

<img src="https://github-profile-trophy.vercel.app/?username=EzequielAngel0&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&row=1" alt="Trophies"/>

</div>

### Contribution Snake

<div align="center">
  <img src="https://raw.githubusercontent.com/EzequielAngel0/EzequielAngel0/output/github-contribution-grid-snake-dark.svg" alt="Contribution Snake"/>
</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%"/>
