<div align="center">

  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=28&pause=1000&color=00F5D4&center=true&vCenter=true&width=800&height=70&lines=Hi%2C+I'm+Alejandro+Duke+%F0%9F%90%A2;Full+Stack+Engineer+%7C+AI+%7C+DevSecOps;Building+systems%2C+not+just+interfaces." alt="Typing Header" />

<br/><br/>

  <a href="https://www.linkedin.com/in/coldex-co/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:alejandrinoduke@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <a href="https://shosocials.netlify.app">
    <img src="https://img.shields.io/badge/Portfolio-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" />
  </a>

<br/><br/>

  <img src="https://komarev.com/ghpvc/?username=AlejandroDukesini&label=Profile%20Views&color=00F5D4&style=for-the-badge" alt="Profile Views" />

</div>

---

# 👋 About Me

I'm a **Full Stack Developer and Systems & Computer Engineering student** focused on building software where architecture, performance, security and maintainability matter.

My strongest interests are:

* **Backend engineering** with Kotlin/Spring Boot and Python/FastAPI.
* **Frontend engineering** with React, Vite and Tailwind CSS.
* **AI / computational systems**, particularly neuroevolution and simulation.
* **DevSecOps and application security**.
* **Performance engineering**, benchmarking and measurable optimization.
* **REST APIs, WebSockets, authentication and RBAC**.
* Designing systems with a clear separation between **domain logic, infrastructure and presentation**.

I prefer to demonstrate engineering decisions through **working systems, reproducible benchmarks, automated tests and technical documentation** rather than purely visual projects.

---

## ⚙️ Engineering Focus

| Area                     | What I work with                                                                     |
| :----------------------- | :----------------------------------------------------------------------------------- |
| **Backend Engineering**  | Kotlin, Spring Boot, Python, FastAPI, REST APIs, JPA/Hibernate                       |
| **Frontend Engineering** | React, Vite, Tailwind CSS, React Router, Axios                                       |
| **Databases**            | PostgreSQL, MySQL, SQLite                                                            |
| **Architecture**         | Layered architecture, modular systems, client/server separation, multi-tenant design |
| **Security**             | JWT, RBAC, dependency vulnerability analysis, OWASP-oriented practices, Kali Linux   |
| **AI / Algorithms**      | Neuroevolution, genetic algorithms, recurrent neural networks, simulation            |
| **Real-Time Systems**    | WebSockets, state synchronization, backpressure handling                             |
| **Testing & QA**         | Unit/integration testing, CI, QA audits, reproducible testing                        |
| **Performance**          | Benchmarking, Lighthouse, Web Vitals, code splitting, asset optimization             |
| **Tooling**              | Git, GitHub Actions, Docker, Gradle, npm, Postman, Linux                             |

---

# 🧠 What I Build

My projects usually fall into three categories:

### Backend & Distributed Application Systems

I build APIs and application backends with explicit concerns around:

* authentication and authorization
* role-based access control
* data isolation
* persistence
* API contracts
* domain/business rules
* performance
* testability

### AI & Computational Systems

I'm particularly interested in systems where algorithms can be evaluated quantitatively.

My **AI-SNAKE** project is an example: instead of hard-coding gameplay rules, the system evolves neural networks using a genetic algorithm and evaluates agents using reproducible metrics.

### Secure Developer Tooling

I'm also interested in applying security directly to the software development lifecycle.

**DepGuard** is a lightweight asynchronous CLI that parses dependency manifests and queries **OSV.dev** for known vulnerabilities.

---

# 🚀 Featured Engineering Projects

## 🧠 AI-SNAKE — Neuroevolution System

**Python · NumPy · FastAPI · React · WebSockets · Vite · Tailwind**

A Snake environment where neural networks learn through **neuroevolution instead of gradient descent or training datasets**.

### Architecture

```text
┌─────────────────────────────┐
│        React Client         │
│                             │
│ UI / Visualization / Input  │
└──────────────┬──────────────┘
               │
          REST / WebSocket
               │
               ▼
┌─────────────────────────────┐
│       FastAPI Server        │
│        Authoritative        │
├─────────────────────────────┤
│ Neuroevolution Engine       │
│ NumPy                       │
│ Genetic Algorithm           │
│ Recurrent Neural Network    │
└──────────────┬──────────────┘
               │
               ▼
        Persistent Models
        & Training History
```

### Engineering Signals

| Metric                 | Result                        |
| :--------------------- | :---------------------------- |
| Simulation throughput  | **≈ 4,000 steps/s**           |
| Generation throughput  | **≈ 2.6 generations/s**       |
| Generation time        | **≈ 380 ms**                  |
| WebSocket streaming    | **20 FPS stable**             |
| Neural perception      | **26 inputs**                 |
| Recurrent architecture | **26 → 20 → 3**               |
| Population size        | **4–100 configurable agents** |

The browser is intentionally a **thin client**. Game rules and simulation state remain server-authoritative, reducing the possibility of client/server state drift.

The streaming layer also implements a form of **latest-state backpressure handling**: transient frames are overwritten while non-lossy events such as generation completion remain queued.

Repository contains dedicated benchmark tooling and technical documentation.

---

## 🍽️ Restaurant Operations Platform

**Kotlin · Spring Boot · PostgreSQL · JPA/Hibernate · React · JWT · RBAC · Docker**

A full-stack restaurant operations system designed around multiple roles and isolated restaurant data.

### Backend

* Kotlin + Spring Boot
* JPA / Hibernate
* PostgreSQL
* JWT authentication
* RBAC
* REST API
* Multi-tenant data isolation
* Business-rule enforcement on the server

### Frontend

* React 19
* Vite
* Tailwind CSS
* React Router

### Roles

```text
ADMIN
 ├── Tables
 ├── Employees
 ├── Menu
 └── Orders

EMPLOYEE
 ├── Floor map
 └── Table orders

COOK
 ├── Kitchen queue
 ├── Recipes
 └── Order state
```

### Quality Engineering

The project currently documents:

* **115 backend tests**
* **44 frontend tests**
* Automated execution through **CI**
* Dedicated `TESTING.md`
* Dedicated `QA_AUDIT.md`

The API also covers reservation logic, capacity control, overlap detection and restaurant registration.

---

## 🛡️ DepGuard

**Python · asyncio · httpx · OSV.dev · CLI · GitHub Actions**

A lightweight DevSecOps dependency vulnerability scanner.

DepGuard analyzes:

* `requirements.txt`
* `package.json`

and queries the **OSV vulnerability database** to identify known dependency vulnerabilities.

### Engineering characteristics

* Asynchronous HTTP requests
* Dependency manifest parsers
* CLI architecture
* Structured terminal output
* Automated tests
* GitHub Actions workflow
* MIT licensed

Architecture:

```text
Manifest
   │
   ▼
Parser
   │
   ▼
Dependency Model
   │
   ▼
Async Scanner ─────► OSV.dev
   │
   ▼
Vulnerability Results
   │
   ▼
CLI Renderer
```

This project reflects my interest in **security automation and shifting security checks closer to the development workflow**.

---

## 🏰 LUDOTECA VALINOR

**React · Vite · Tailwind CSS · React Router · Axios**

A production-oriented frontend for a TCG / tabletop gaming business.

The project goes beyond UI implementation and includes explicit performance and SEO engineering.

### Performance

| Metric         |  Mobile |  Desktop |
| :------------- | :-----: | :------: |
| Performance    |  **87** |  **100** |
| Accessibility  | **100** |  **96**  |
| Best Practices | **100** |  **100** |
| SEO            | **100** |  **100** |
| CLS            |  **0**  |   **0**  |
| LCP            |   3.2s  | **0.7s** |

### Optimization techniques

* Route-level code splitting
* `React.lazy()` + `Suspense`
* Vendor chunk separation
* Lazy-loaded images
* WebP asset optimization
* Explicit image dimensions
* LCP prioritization
* SEO metadata
* Open Graph / Twitter Cards
* JSON-LD structured data
* `robots.txt`
* `sitemap.xml`

One of the measured optimizations reduced a major background asset from approximately **4.88 MB to 170 KB (~96.5% reduction)**.

---

## 🚗 Casa Renault

**React · Vite · Tailwind CSS · React Router · Netlify**

Commercial frontend architecture for an automotive parts platform.

Technical focus includes:

* SPA architecture
* Route-based code splitting
* Responsive UI
* Reduced-motion support
* Static deployment through CDN
* SPA fallback configuration
* Production build optimization

The repository explicitly separates the frontend from the backend/API maintained in another repository.

---

# 📊 Engineering Metrics

Instead of using generic GitHub “streak” statistics, I prefer metrics that describe actual engineering work.

<div align="center">

| Signal                             |         Evidence         |
| :--------------------------------- | :----------------------: |
| Public repositories                |          **15+**         |
| GitHub stars                       |          **16+**         |
| Restaurant platform tests          | **159 documented tests** |
| AI simulation throughput           |    **≈4,000 steps/s**    |
| AI real-time streaming             |        **20 FPS**        |
| AI neural inputs                   |          **26**          |
| Largest measured asset reduction   |        **≈96.5%**        |
| Lighthouse — Valinor Desktop       |    **100 Performance**   |
| Lighthouse — Valinor SEO           |          **100**         |
| Lighthouse — Valinor Accessibility |      **100 Mobile**      |

</div>

> Metrics are reported from the documentation and benchmark methodology of the corresponding repositories rather than generated GitHub vanity statistics.

---

# 🧪 Engineering Practices

Across my projects I focus on:

### Architecture

* Separation of concerns
* Modular components
* Explicit domain boundaries
* Thin clients where appropriate
* Server-authoritative state
* API-driven applications

### Quality

* Unit and integration testing
* CI pipelines
* QA documentation
* Reproducible benchmarks
* Technical audits

### Performance

* Profiling and benchmarking
* Code splitting
* Lazy loading
* Asset compression
* WebSocket backpressure strategies
* Database/query optimization

### Security

* JWT authentication
* RBAC
* Dependency vulnerability scanning
* Secure API boundaries
* Security-oriented development workflows

---

# 🔬 Current Technical Direction

I'm currently deepening my knowledge around:

```text
Software Architecture
        │
        ├── Distributed Systems
        ├── Multi-Tenant SaaS
        ├── Backend Performance
        └── API Design

DevSecOps
        │
        ├── Dependency Security
        ├── CI/CD Security
        ├── Vulnerability Assessment
        └── Secure Development Lifecycle

AI Engineering
        │
        ├── Neuroevolution
        ├── Neural Architectures
        ├── Simulation
        └── Algorithmic Optimization
```

---

# 💼 What I'm Looking For

I'm particularly interested in opportunities where I can contribute to:

* **Backend Engineering**
* **Full Stack Engineering**
* **Software Architecture**
* **DevSecOps**
* **Application Security**
* **AI / Applied Algorithms**
* **Performance Engineering**

I value environments where engineers are expected to understand not only **how to make software work**, but also **why the system is designed that way and how to prove that it works**.

---

# 📫 Contact

If you're interested in discussing software engineering, architecture, security, AI systems or potential collaboration, feel free to reach out.

<div align="center">

**Building systems. Measuring them. Improving them.**

</div>
