<div align="center">

# Felipe Gardenghi
### Desenvolvedor Full-Stack | Engenharia de Software & Ciência de Dados

[![Portfólio](https://img.shields.io/badge/🌐_Portfólio_Online-felipegardenghidev.github.io-6366f1?style=for-the-badge)](https://felipegardenghidev.github.io/portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/felipegardenghi/)
[![Currículo PDF](https://img.shields.io/badge/📄_Download_CV-PDF-059669?style=for-the-badge)](https://felipegardenghidev.github.io/portfolio/resume/felipe-gardenghi-cv.pdf)
[![E-mail](https://img.shields.io/badge/E--mail-felipegg.dev%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:felipegg.dev@gmail.com)

<br/>

> *"Desenvolvo aplicações web escaláveis, microsserviços orientados a eventos e soluções de Ciência de Dados & Machine Learning — integrando sistemas legados e ERPs corporativos a arquiteturas modernas, combinando rigor técnico com visão pragmática de negócio."*

</div>

---

### 👨‍💻 Sobre Mim & Trajetória Profissional

- 💼 **Atuação Corporativa Atual:** Desenvolvedor / Estagiário de T.I. na **Nova Smar S/A**, onde desenvolvi e mantenho em produção um **Dashboard Financeiro e de Automação ERP** (PHP, Oracle Database 12c, OCI8 com parametrização anti-SQL Injection, TOTVS Protheus, MySQL), além de triggers/procedures PL/SQL para conciliação contábil e relatórios de estoque que viabilizaram a conclusão do inventário corporativo em tempo recorde em 2025.
- 🎓 **Formação Acadêmica:** Bacharelado em **Ciência de Dados** pela **UNIVESP** (*Universidade Virtual do Estado de São Paulo*).
  - **Backend & Microsserviços:** C# / .NET 8 (ASP.NET Core Web API, Entity Framework Core, Dapper, LINQ, Clean Architecture), Java 21 LTS (Spring Boot 3, Arquitetura Hexagonal, Virtual Threads / Loom, Spring Security), resiliência distribuída com **Transactional Outbox Pattern**, **Resilience4j Circuit Breaker**, **Flyway Database Migrations**, Domain-Driven Design (DDD & Value Objects), **Terraform (IaC na AWS)**, mensageria orientada a eventos com RabbitMQ, Redis Sliding Window Cache com scripts Lua atômicos, observabilidade com Prometheus/Micrometer e Docker/Testcontainers.
  - **Frontend & Engenharia Quantitativa:** Angular, React 19, Next.js 16 (App Router), TypeScript, Tailwind CSS v4, cálculos financeiros de precisão arbitrária (**Decimal.js**), gráficos em **Canvas GPU TradingView** a 60 FPS, simulação estocástica assíncrona (**Monte Carlo via Web Workers**), streaming **Server-Sent Events (SSE)** em Edge Runtime, Zustand com persistência seletiva, Zod e pirâmide de testes completa com **Vitest (130 testes)** e **Playwright (8 suítes E2E)**.
  - **Ciência de Dados & MLOps:** Python (Scikit-learn, LightGBM, SHAP Explainable AI, Pandas), Web Scraping automatizado, APIs de inferência em tempo real com FastAPI + Pydantic v2, conteinerização Docker, IaC com Terraform na AWS e dashboards em Streamlit.
  - **Mobile Nativo & IA:** Kotlin 2.0 (Jetpack Compose, Clean Architecture + MVVM, Google Hilt DI, DataStore Preferences, Offline-First, P2P Nearby), Google MediaPipe Hands (Visão Computacional na GPU), Tone.js e integração de LLMs (Google Gemini API / FastAPI).
- 📈 **Bagagem Empreendedora & Visão de Negócio:** 5 anos de experiência liderando operação própria no e-commerce (**Mercadolíder** em menos de 1 ano), gerenciando precificação, análise de dados de vendas e relacionamento com clientes. Vivência prática que orienta cada linha de código para solucionar dores reais de negócio.
- 🌍 **Idiomas:** Português (Nativo) · Inglês (Intermediário Técnico B2) · Alemão (Básico A1).

---

### 🚀 Projetos Públicos & Cases em Destaque

| Projeto | Descrição & Destaques Técnicos | Tecnologias | Links |
| :--- | :--- | :--- | :---: |
| 🏢 **Dashboard Financeiro & ERP** | **Case Corporativo em Produção:** Sistema web intranet multiusuário e auditável integrado ao ERP TOTVS Protheus e Oracle DB. Substituiu controles manuais por fluxo de caixa automatizado e relatórios em tempo real para tomada de decisão da diretoria e acionistas. | `PHP` `Oracle PL/SQL` `TOTVS Protheus` `MySQL` `JavaScript` | 🔒 *Código Proprietário (Nova Smar S/A)* |
| 🛡️ **Fraud Detection & Risk Engine API** | Plataforma corporativa de prevenção a fraudes em tempo real (<10ms) sob **Arquitetura Hexagonal (Ports & Adapters)**, **Java 21 Virtual Threads (Loom)** e **9 ADRs formais**. Esteira determinística com **7 regras de produção** (incluindo *Impossible Travel* via Haversine, Perfil Comportamental via Z-Score e *Smurfing/Structuring*). **Resilience4j Circuit Breaker** protegendo o cluster de cache, **Redis ZSET com script Lua atômico** para janela deslizante sem race conditions, **Flyway SQL Migrations** com `validate`, **Transactional Outbox Pattern (ACID)** para entrega *At-Least-Once*, **Testcontainers (Docker)** para paridade de produção no PostgreSQL, **telemetria Micrometer/Prometheus**, **IaC completo via Terraform na AWS** e **46+ testes automatizados (100% passing)**. | `Java 21` `Spring Boot 3` `Hexagonal` `Virtual Threads` `Resilience4j` `Flyway` `Testcontainers` `Outbox` `Redis Lua` `Prometheus` `JaCoCo (46+)` | [Código](https://github.com/FelipeGardenghiDev/fraud-detection-api) |
| 📦 **Order Processing API (.NET 8 & CQRS)** | API corporativa em **.NET 8 (C# 12)** com **Clean Architecture** e padrão híbrido **CQRS**: **Entity Framework Core** para escrita consistente com encapsulamento de regras de domínio via backing fields, e **Dapper (Micro-ORM)** para leitura analítica de alta performance com multi-mapping e agregações. Enfileiramento assíncrono desacoplado via **`System.Threading.Channels`** consumido por **`BackgroundService` (Worker)** e **26 testes unitários e de integração com xUnit, FluentAssertions e NSubstitute**. | `C# 12` `.NET 8` `EF Core` `Dapper` `Clean Arch` `Channels` `Worker` `xUnit` | [Código](https://github.com/FelipeGardenghiDev/order-processing-api) |
| 🌾 **AgroFinance RWA Banking Dashboard** | Plataforma bancária corporativa, tesouraria de Real World Assets (RWA) e crédito rural (CPR Digital) para o agronegócio. Arquitetura com **ADRs**, aritmética financeira de precisão arbitrária (**Decimal.js** eliminando falhas IEEE-754), gráficos em **Canvas GPU TradingView** a 60 FPS, motor quantitativo **Monte Carlo (1.000 iterações)** assíncrono via **Web Worker**, simulador **What-If** de estresse macroeconômico, relação de troca (*Barter*), **Dossiê Bancário com selo SHA-256 e @media print**, streaming **Server-Sent Events (SSE)** em Edge Runtime, exportação contábil para ERPs agrícolas (**TOTVS Agro / Siagri**), i18n bilíngue nativo e **130 testes no Vitest + 8 suítes E2E no Playwright (100% passing)**. | `Next.js 16` `React 19` `TypeScript` `Decimal.js` `TradingView` `Web Workers` `Vitest (130)` `Playwright (8 E2E)` `Zustand` | [Demo](https://agrofinance-dashboard-dev.vercel.app/dashboard) · [Código](https://github.com/FelipeGardenghiDev/agrofinance-dashboard) |
| 📡 **Sentinela Casa — Network Security & IoT Agent** | Bot autônomo de inteligência de rede local e segurança IoT via Telegram. Monitoramento ARP passivo/ativo contínuo, resolução instantânea de vendors MAC OUI (Apple, Xiaomi, Amazon, Samsung), priorização inteligente de dispositivos online com expurgo automático de aliases obsoletos, tolerância a MACs privados rotativos, gestão de convidados temporários e alertas proativos sem dependência de nuvem. | `Python 3.11` `Scapy` `Telegram Bot API` `Asyncio` `SQLite` `Network Security` | [Código](https://github.com/FelipeGardenghiDev/sentinela-casa) |
| 🏡 **Imóveis Pricing ML — Inteligência Imobiliária** | Pipeline End-to-End de MLOps para precificação e arbitragem imobiliária na Grande Ribeirão Preto/SP. Modelo LightGBM ($R^2 = 0.835$), explicabilidade auditada com SHAP, serving em tempo real via API REST desacoplada (FastAPI + Pydantic v2), conteinerização multi-stage em Docker, IaC modular via Terraform na AWS, CI/CD com Pytest e Radar de Oportunidades em Streamlit. | `Python 3.11+` `FastAPI` `LightGBM` `SHAP` `Docker` `Terraform AWS` `Streamlit` `Pytest` | [Código](https://github.com/FelipeGardenghiDev/imoveis-pricing-ml) |
| 🎵 **VisuChord — Síntese por Visão Computacional** | Aplicação web que transforma a webcam em um instrumento musical polifônico em tempo real a 60 FPS. Rastreamento de 21 pontos anatômicos das mãos via Google MediaPipe na GPU (WebGL/Wasm), síntese harmônica cromática com Tone.js e visualizador interativo. | `React 19` `Vite 8` `Google MediaPipe` `Tone.js` `WebGL` `TypeScript` | [Código](https://github.com/FelipeGardenghiDev/visuchord) |
| 🎸 **Website Banda Revanche** | Website institucional oficial e promocional em produção para cliente real. Arquitetura moderna em Next.js 16 App Router, dados estruturados Schema.org (`MusicGroup`) para SEO no Google, player Spotify e agenda dinâmica. | `Next.js 16` `React 19` `TypeScript` `Tailwind CSS v4` `SEO Schema.org` | [Website](https://bandarevanche.com.br) · [Código](https://github.com/FelipeGardenghiDev/revanche-website) |
| 🎲 **Grimório RPG — Companion Android** | Assistente nativo para RPG de mesa com arquitetura Clean + MVVM, injeção de dependências com **Google Hilt** e design 100% Offline-First ($0 custo de nuvem). Parser léxico em Kotlin puro para fórmulas complexas de dados, motor de combate e recursos, compartilhamento via QR Code (GZIP+Base64), mesa local P2P sem internet via Google Nearby Connections (Bluetooth LE / Wi-Fi Direct) com **Star Topology Relay**, persistência reativa com Room SQLite e **Jetpack DataStore Preferences**, feedback sensorial (SoundPool / VibrationEffect), regras ProGuard/R8 e preparação completa para a Google Play Store. | `Kotlin 2.0` `Jetpack Compose` `Hilt (DI)` `Room SQLite` `DataStore` `Google Nearby P2P` `CameraX` | [Código](https://github.com/FelipeGardenghiDev/rpg-companion-android) |
| 🧠 **Segundo Cérebro (Life OS)** | Assistente inteligente integrado com WhatsApp e Painel Web para gestão pessoal, financeira e de estúdio musical. Desenvolvido com FastAPI, inteligência artificial multimodal com Google Gemini 2.0 Flash, FullCalendar e persistência relacional no Supabase. | `Python` `FastAPI` `Google Gemini 2.0` `Supabase PostgreSQL` `FullCalendar` | 🔒 *Repositório Privado (Uso Pessoal)* |


---

### 🛠️ Stack Tecnológica & Habilidades

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>⚙️ Backend & Microsserviços</h4>
      <div>
        <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white" alt="C#" />
        <img src="https://img.shields.io/badge/.NET_8_LTS-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt=".NET 8" />
        <img src="https://img.shields.io/badge/Entity_Framework_Core-512BD4?style=flat-square" alt="EF Core" />
        <img src="https://img.shields.io/badge/Dapper_(Micro--ORM)-005571?style=flat-square" alt="Dapper" />
        <img src="https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java 21" />
        <img src="https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot 3" />
        <img src="https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP" />
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
        <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
        <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
        <img src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white" alt="RabbitMQ" />
        <img src="https://img.shields.io/badge/REST_APIs-005571?style=flat-square" alt="REST APIs" />
      </div>
    </td>
    <td width="50%" valign="top">
      <h4>🎨 Frontend & Web Moderna</h4>
      <div>
        <img src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white" alt="Angular" />
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
        <img src="https://img.shields.io/badge/JavaScript_ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript" />
        <img src="https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React 19" />
        <img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js 16" />
        <img src="https://img.shields.io/badge/Tailwind_CSS_v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS v4" />
        <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5" />
        <img src="https://img.shields.io/badge/CSS3_Design_System-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3" />
        <img src="https://img.shields.io/badge/Decimal.js-Precis%C3%A3o_Arbitr%C3%A1ria-green?style=flat-square" alt="Decimal.js" />
        <img src="https://img.shields.io/badge/TradingView_Canvas-GPU_60FPS-blue?style=flat-square" alt="TradingView" />
        <img src="https://img.shields.io/badge/Web_Workers-Monte_Carlo_Async-orange?style=flat-square" alt="Web Workers" />
        <img src="https://img.shields.io/badge/SSE-Server--Sent_Events-teal?style=flat-square" alt="SSE" />
        <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
      </div>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🤖 Ciência de Dados & IA</h4>
      <div>
        <img src="https://img.shields.io/badge/Machine_Learning-FF6F00?style=flat-square" alt="Machine Learning" />
        <img src="https://img.shields.io/badge/LightGBM-FFA500?style=flat-square" alt="LightGBM" />
        <img src="https://img.shields.io/badge/SHAP_(XAI)-00A389?style=flat-square" alt="SHAP" />
        <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="Scikit-Learn" />
        <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas" />
        <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit" />
        <img src="https://img.shields.io/badge/Google_MediaPipe-0097A7?style=flat-square&logo=google&logoColor=white" alt="MediaPipe" />
        <img src="https://img.shields.io/badge/Google_Gemini_API-4285F4?style=flat-square&logo=google&logoColor=white" alt="Gemini API" />
      </div>
    </td>
    <td width="50%" valign="top">
      <h4>🗄️ Bancos de Dados & Caching</h4>
      <div>
        <img src="https://img.shields.io/badge/Oracle_PL%2FSQL-F80000?style=flat-square&logo=oracle&logoColor=white" alt="Oracle PL/SQL" />
        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
        <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" alt="Supabase" />
        <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL" />
        <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
        <img src="https://img.shields.io/badge/Triggers_%26_Procedures-333333?style=flat-square" alt="Triggers & Procedures" />
      </div>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h4>🧪 Testes, DevOps & Ferramentas</h4>
      <div>
        <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" />
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
        <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
        <img src="https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white" alt="Vitest" />
        <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white" alt="Playwright" />
        <img src="https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white" alt="JUnit 5" />
        <img src="https://img.shields.io/badge/JaCoCo-005571?style=flat-square" alt="JaCoCo" />
        <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
        <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux" />
        <img src="https://img.shields.io/badge/Swagger_%2F_OpenAPI-85EA2D?style=flat-square&logo=swagger&logoColor=black" alt="Swagger" />
      </div>
    </td>
    <td width="50%" valign="top">
      <h4>📱 Mobile & Sistemas Corporativos</h4>
      <div>
        <img src="https://img.shields.io/badge/Kotlin_2.0-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
        <img src="https://img.shields.io/badge/Android_Jetpack_Compose-4285F4?style=flat-square&logo=android&logoColor=white" alt="Jetpack Compose" />
        <img src="https://img.shields.io/badge/Hilt_(DI)-25A162?style=flat-square&logo=dagger&logoColor=white" alt="Hilt" />
        <img src="https://img.shields.io/badge/DataStore-00599C?style=flat-square" alt="DataStore" />
        <img src="https://img.shields.io/badge/Clean_Architecture-00599C?style=flat-square" alt="Clean Architecture" />
        <img src="https://img.shields.io/badge/TOTVS_Protheus-003366?style=flat-square" alt="TOTVS Protheus" />
        <img src="https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black" alt="Power BI" />
      </div>
    </td>
  </tr>
</table>

---

<div align="center">
  
**📬 Vamos conversar sobre oportunidades, desafios técnicos e novos projetos?**

[LinkedIn](https://www.linkedin.com/in/felipegardenghi/) • [Portfólio Oficial](https://felipegardenghidev.github.io/portfolio/) • [felipegg.dev@gmail.com](mailto:felipegg.dev@gmail.com)

</div>
