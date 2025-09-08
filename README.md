# week-4-<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>CarePay — Finance Intern Demo (Responsive)</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <a class="brand" href="#">CarePay<span class="dot">.</span></a>
      <nav class="nav">
        <ul class="nav-list">
          <li><a href="#features">Features</a></li>
          <li><a href="#how">How it works</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
      <button class="btn btn-ghost nav-toggle" aria-expanded="false" aria-label="Toggle navigation">☰</button>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-inner">
        <div class="hero-copy">
          <h1>Finance + Healthcare, simplified.</h1>
          <p class="lead">A small, responsive landing layout demonstrating modern CSS: Flexbox for UI components and Grid for content layout.</p>
          <div class="hero-cta">
            <a class="btn" href="#features">Explore features</a>
            <a class="btn btn-outline" href="#contact">Apply now</a>
          </div>
        </div>
        <div class="hero-visual">
          <img src="https://images.unsplash.com/photo-1522075469751-3a6694fb2f61?w=1200&q=60&auto=format&fit=crop" alt="Team collaborating"/>
        </div>
      </div>
    </section>

    <!-- Features: Grid layout -->
    <section id="features" class="section">
      <div class="container">
        <h2 class="section-title">Core features</h2>
        <p class="section-sub">Built with Grid for the feature cards, Flexbox for card internals and controls.</p>

        <div class="features-grid">
          <article class="card">
            <div class="card-icon">💳</div>
            <div class="card-body">
              <h3>Payments & reconciliation</h3>
              <p>Streamlined invoicing and reconciliation workflows for clinics and payers.</p>
            </div>
          </article>

          <article class="card">
            <div class="card-icon">📊</div>
            <div class="card-body">
              <h3>Real-time reports</h3>
              <p>Dashboards and exportable reports to support financial decision-making.</p>
            </div>
          </article>

          <article class="card">
            <div class="card-icon">🔒</div>
            <div class="card-body">
              <h3>Secure by design</h3>
              <p>Role-based access, audit logs and best-practice encryption.</p>
            </div>
          </article>

          <article class="card">
            <div class="card-icon">🤝</div>
            <div class="card-body">
              <h3>Partner integrations</h3>
              <p>Open APIs to connect to insurers, clinics and payment rails.</p>
            </div>
          </article>
        </div>
      </div>
    </section>

    <!-- Two-column section using Grid + Flexbox for stats -->
    <section id="how" class="section alt">
      <div class="container two-col">
        <div class="col text">
          <h2>How it works</h2>
          <p>Content-driven breakpoints keep the layout resilient across screen sizes. We use Grid to create the overall two-column layout and Flexbox for the stats row and CTA alignment.</p>
          <div class="stats-row" role="list">
            <div class="stat" role="listitem">
              <strong>4.7m</strong>
              <span>Users</span>
            </div>
            <div class="stat" role="listitem">
              <strong>5,100</strong>
              <span>Facilities</span>
            </div>
            <div class="stat" role="listitem">
              <strong>99.9%</strong>
              <span>Uptime</span>
            </div>
          </div>
          <div class="cta-row">
            <a class="btn" href="#contact">Start application</a>
            <a class="btn btn-ghost" href="#features">Learn more</a>
          </div>
        </div>
        <div class="col visual">
          <div class="card surface">
            <h3>Sample reconciliation view</h3>
            <div class="recon-grid">
              <div class="recon-item">Date</div>
              <div class="recon-item">Invoice</div>
              <div class="recon-item">Amount</div>
              <div class="recon-item">Status</div>
              <div class="recon-item">2025-07-01</div>
              <div class="recon-item">INV-1029</div>
              <div class="recon-item">KES 150,000</div>
              <div class="recon-item">Paid</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" class="section">
      <div class="container contact-card">
        <h2>Apply for the finance internship</h2>
        <form class="form-grid" action="#" onsubmit="alert('Demo form — no submission')">
          <label class="sr-only" for="name">Name</label>
          <input id="name" placeholder="Your full name" required>

          <label class="sr-only" for="email">Email</label>
          <input id="email" type="email" placeholder="Email address" required>

          <label class="sr-only" for="message">Why you?</label>
          <textarea id="message" placeholder="Why do you want this internship?" rows="4"></textarea>

          <button class="btn" type="submit">Submit application</button>
        </form>
      </div>
    </section>

  </main>

  <footer class="site-footer">
    <div class="container footer-inner">
      <p>&copy; <span id="year">2025</span> CarePay — Demo layout • Built with Flexbox & Grid</p>
      <nav class="footer-nav">
        <a href="#">Privacy</a>
        <a href="#">Terms</a>
      </nav>
    </div>
  </footer>

  <script>
    // Simple nav toggle for small screens
    const toggle = document.querySelector('.nav-toggle');
    const nav = document.querySelector('.nav');
    toggle && toggle.addEventListener('click', () => {
      const expanded = toggle.getAttribute('aria-expanded') === 'true';
      toggle.setAttribute('aria-expanded', !expanded);
      nav.classList.toggle('open');
    });

    // Set year
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
assignment
