<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=2B6FB5&center=true&vCenter=true&width=760&lines=Angel+Ezequiel+Barbosa+Lomeli;Full+Stack+%26+Cross-Platform+Developer;Go+%7C+Flutter+%7C+React+%7C+OCI;Security-minded%3A+I+secure+what+I+ship;From+first+commit+to+production" alt="Typing SVG"/>

<a href="https://www.linkedin.com/in/angelezequiel"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://portfolio.angelezequiel.dev"><img src="https://img.shields.io/badge/Portfolio-2B6FB5?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"/></a>
<a href="mailto:angelbarbosa@angelezequiel.dev"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://x.com/Ezequiel27Angel"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"/></a>

<br>

<img src="https://img.shields.io/badge/Open_to_Work-2EA043?style=for-the-badge&logo=briefcase&logoColor=white" alt="Open to Work"/>
<img src="https://komarev.com/ghpvc/?username=EzequielAngel0&style=flat-square&color=2b6fb5" alt="Profile views"/>

<br><br>

<sub><b>// now</b> &nbsp;·&nbsp; Cisco Junior Cybersecurity Analyst + Ethical Hacker &nbsp;·&nbsp; PortSwigger Web Security Academy &nbsp;·&nbsp; hardening my own production stack</sub>

</div>

---

## About Me &nbsp;/&nbsp; Sobre mí

<table>
<tr>
<td valign="top" width="50%">

<b>EN</b>

I design, build, and operate complete systems end-to-end, often solo, and I build them to be attacked. My flagship work, <b>ACP</b>, runs in production on Oracle Cloud: a Go backend, a React admin panel, a Next.js public site, and four offline-first Flutter apps, provisioned with Terraform/Ansible and shipped through a CI/CD pipeline with security gates. I am now deepening application security to audit and defend what I ship. Oracle Next Education (ONE) Tech Advanced graduate (Back-End track), OCI Certified Foundations Associate, Google Cloud Cybersecurity certified, and Software Development student at CETI.

</td>
<td valign="top" width="50%">

<b>ES</b>

Diseño, construyo y opero sistemas completos de punta a punta, frecuentemente en solitario, y los construyo pensando en que serán atacados. Mi trabajo insignia, <b>ACP</b>, corre en producción sobre Oracle Cloud: backend en Go, panel admin en React, sitio público en Next.js y cuatro apps Flutter offline-first, aprovisionado con Terraform/Ansible y publicado con un pipeline CI/CD con gates de seguridad. Ahora profundizo en seguridad de aplicaciones para auditar y defender lo que construyo. Graduado del programa Oracle Next Education (ONE), ruta Back-End y nivel Tech Advanced, certificado OCI Foundations Associate y Google Cloud Cybersecurity, y estudiante de Desarrollo de Software en el CETI.

</td>
</tr>
</table>

---

## Featured Projects &nbsp;/&nbsp; Proyectos Destacados

<table>
  <tr>
    <td valign="top">
      <h3>ACP &nbsp;<img src="https://img.shields.io/badge/LIVE_IN_PRODUCTION-2EA043?style=flat-square" alt="Live"/></h3>
      <p>End-to-end ticketing &amp; parcel platform for an intercity bus company, <b>live in production on Oracle Cloud</b>. Built solo, replacing fully manual operations: two Go APIs (RBAC, audited mutations, transactional sales), a React admin panel, a Next.js public site, and four <b>offline-first</b> Flutter apps (ticket office, driver, parcels, customer) sharing in-house design-system, API-client, and ESC/POS thermal-printing packages.</p>
      <p>
        <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white"/>
        <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
        <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
        <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white"/>
        <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white"/>
        <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white"/>
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
  </tr>
</table>

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>DocuAgent &nbsp;<img src="https://img.shields.io/badge/LIVE_+_DEMO-2EA043?style=flat-square" alt="Live"/></h3>
      <p>RAG-powered AI agent for querying a company's internal documentation. A LangGraph pipeline (Cohere Embed v3 + Rerank over Qdrant) returns source-cited answers with an anti-hallucination validator; multilingual chat (ES/EN/PT) streamed over WebSocket. <b>Live in production on Oracle Cloud with a public demo</b>. Admin behind Cloudflare Turnstile + TOTP; the VM exposes no ports (Cloudflare Tunnel only).</p>
      <p>
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
        <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
        <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white"/>
        <img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white"/>
        <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
      </p>
      <p>
        <a href="https://github.com/EzequielAngel0/DocuAgent">Repo</a> &nbsp;·&nbsp;
        <a href="https://docuagent.angelezequiel.dev">Live demo</a>
      </p>
    </td>
    <td width="50%" valign="top">
      <h3>SoloKey</h3>
      <p>Local-first, cross-platform password manager: an <b>Android app + a Windows desktop companion</b> sharing one encrypted vault. Optional sync is peer-to-peer and end-to-end encrypted over the LAN (X25519 pairing, AES-256-GCM), no cloud. Argon2id + AES-256-GCM, built-in TOTP, weak/reused/breached auditing (HaveIBeenPwned k-anonymity), and 510 automated tests with a CI coverage floor.</p>
      <p>
        <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
        <img src="https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white"/>
        <img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white"/>
        <img src="https://img.shields.io/badge/Windows-0078D4?style=flat-square&logo=windows&logoColor=white"/>
      </p>
      <p><a href="https://github.com/EzequielAngel0/SoloKey">github.com/EzequielAngel0/SoloKey</a></p>
    </td>
  </tr>
</table>

---

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

---

## Certifications &nbsp;/&nbsp; Certificaciones

<div align="center">

<a href="https://www.credly.com/badges/6b602da5-95ea-4328-a5dd-03ba538dfbf9/linked_in_profile"><img src="https://img.shields.io/badge/Google_Cloud_Cybersecurity_Certificate-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" alt="Google Cloud Cybersecurity Certificate"/></a>
<a href="https://catalog-education.oracle.com/ords/certview/sharebadge?id=9E6AA54792091B7F8EAD1C3D4C0E00B4640759558EA9319193256E348344778E"><img src="https://img.shields.io/badge/OCI_2025_Certified_Foundations_Associate-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="OCI Foundations Associate"/></a>
<a href="https://app.aluracursos.com/program/certificate/8a039e9d-447c-4d64-9a32-40a020f15bf5?lang"><img src="https://img.shields.io/badge/ONE_Tech_Advanced_G9_·_Back--End-2B6FB5?style=for-the-badge&logo=oracle&logoColor=white" alt="ONE Tech Advanced G9 Back-End"/></a>

</div>

---

## Currently Learning &nbsp;/&nbsp; Aprendiendo

<table>
<tr>
<td valign="top" width="40%">
  <img src="https://img.shields.io/badge/Offensive_Security-111827?style=for-the-badge&logo=hackthebox&logoColor=9FEF00"/><br>
  <b>AppSec & Ethical Hacking</b>
</td>
<td valign="top" width="60%">
  Adding an attacker's perspective to defend what I build. Enrolled in Cisco's <b>Junior Cybersecurity Analyst</b> career path and <b>Ethical Hacker</b> course, plus the <b>PortSwigger Web Security Academy</b>, with hands-on labs on TryHackMe and Hack The Box. Focus: web &amp; API security (OWASP, injection, SSRF, auth flaws) applied to my own production systems.
  <br><br>
  <i>Sumando la perspectiva del atacante para defender lo que construyo. Inscrito en la ruta de Analista Junior en Ciberseguridad y el curso Ethical Hacker de Cisco, más la PortSwigger Web Security Academy, con laboratorios en TryHackMe y Hack The Box. Enfoque: seguridad web y de APIs (OWASP, inyección, SSRF, fallos de autenticación) aplicada a mis propios sistemas en producción.</i>
  <br><br>
  <sub><b>exploring:</b></sub>
  <img src="https://img.shields.io/badge/Kali-557C94?style=flat-square&logo=kalilinux&logoColor=white"/>
  <img src="https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logo=metasploit&logoColor=white"/>
  <img src="https://img.shields.io/badge/OWASP-000000?style=flat-square&logo=owasp&logoColor=white"/>
</td>
</tr>
<tr>
<td valign="top" width="40%">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/><br>
  <b>Python · FastAPI</b>
</td>
<td valign="top" width="60%">
  Expanding my backend toolbox into the Python ecosystem: REST services with <b>FastAPI</b>, async I/O, and Pydantic, applying the same architecture, testing, and security standards I use in Go. Already shipped in DocuAgent.
  <br><br>
  <i>Ampliando mi backend al ecosistema Python: servicios REST con FastAPI, async I/O y Pydantic, con los mismos estándares de arquitectura, pruebas y seguridad que uso en Go. Ya en producción en DocuAgent.</i>
</td>
</tr>
</table>

---

## GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=EzequielAngel0&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub Stats"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=EzequielAngel0&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages"/>

<br><br>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=EzequielAngel0&bg_color=1a1b27&color=c9d1d9&line=2b6fb5&point=ffffff&area=true&area_color=2b6fb5&hide_border=true&custom_title=Contribution%20Activity" alt="Contribution Activity Graph" width="100%"/>

</div>
