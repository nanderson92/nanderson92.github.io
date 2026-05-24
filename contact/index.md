---
layout: page
title: Contact
category: Opportunities
body_class: contact-page
subtitle: Recruiter-friendly contact page for technical internships, co-ops, research, and engineering conversations.
---

<section class="contact-hero-panel recruiter-contact">
  <p class="system-label small">LET'S CONNECT</p>
  <h2>Let’s connect around process engineering and the future of manufacturing.</h2>
  <p class="contact-hero-lede">
    I’m interested in roles and technical conversations where experimental data, process physics, and manufacturing constraints meet — especially in wet processing, advanced materials, semiconductor process development, reliability, scale-up, and clean-technology deployment.
  </p>
  <p class="contact-open-line">
    <strong>Currently open to:</strong> Summer/Fall 2026 internships and co-ops in process engineering, R&amp;D, manufacturing, advanced materials, semiconductors, and clean technology.
  </p>
  <div class="resume-actions contact-actions" aria-label="Primary contact links">
    <a class="button primary" href="mailto:{{ site.email }}">Email Me</a>
    <a class="button secondary" href="{{ site.linkedin }}">LinkedIn</a>
    <a class="button secondary" href="{{ site.github }}">GitHub</a>
    <a class="button tertiary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume</a>
  </div>
  <a class="scroll-cue contact-scroll-cue" href="#contact-workbench" aria-label="Scroll to direct message form">
    <span>Send a note</span>
    <strong aria-hidden="true">↓</strong>
  </a>
</section>

<section id="contact-workbench" class="contact-workbench" aria-label="Contact form and contact guidance">
  <form class="contact-form contact-form-card reveal" style="--reveal-delay: 40ms" action="https://formspree.io/f/xkoeblkb" method="POST">
    <input type="hidden" name="_subject" value="Portfolio contact form message for Nathan Anderson">
    <div class="contact-form-heading">
      <p class="system-label small">DIRECT MESSAGE</p>
      <h3>Send a note</h3>
      <p>Best for role-specific conversations, research questions, technical collaborations, or quick introductions.</p>
    </div>
    <div class="form-grid">
      <label>
        <span>Name</span>
        <input type="text" name="name" autocomplete="name" placeholder="Your name" required>
      </label>
      <label>
        <span>Email</span>
        <input type="email" name="email" autocomplete="email" placeholder="you@example.com" required>
      </label>
    </div>
    <label>
      <span>Message</span>
      <textarea name="message" rows="6" placeholder="What would you like to connect about?" required></textarea>
    </label>
    <button class="button primary contact-submit" type="submit">Send message</button>
    <p class="form-footnote">This form routes through Formspree. Email is still the fastest way to reach me directly.</p>
  </form>

  <aside class="contact-context-card reveal" style="--reveal-delay: 140ms" aria-label="Best ways to reach Nathan Anderson">
    <p class="system-label small">BEST WAY TO REACH ME</p>
    <h3>Start with email for role-specific conversations.</h3>
    <p>
      LinkedIn is best for quick introductions. GitHub is best for seeing code and technical buildout. Resume is best for a fast recruiter screen.
    </p>
    <div class="contact-route-list">
      <div class="contact-route">
        <span>Email</span>
        <strong>Internships, co-ops, research, and detailed technical conversations</strong>
      </div>
      <div class="contact-route">
        <span>LinkedIn</span>
        <strong>Recruiter outreach, quick introductions, and follow-ups</strong>
      </div>
      <div class="contact-route">
        <span>Portfolio</span>
        <strong>Start with the micromodular deposition case study for the strongest technical proof</strong>
      </div>
    </div>
  </aside>
</section>

<section class="best-fit-section reveal" style="--reveal-delay: 40ms">
  <div class="section-heading contact-section-heading">
    <p class="system-label small">WHERE I FIT BEST</p>
    <h2>Best-fit conversations</h2>
    <p>I’m most excited about technical discussions that connect experiments, process variables, measurable outputs, and manufacturing decisions.</p>
  </div>

  <div class="matrix contact-fit-grid">
    <div class="matrix-card contact-fit-card reveal" style="--reveal-delay: 60ms">
      <span class="fit-index">01</span>
      <h3>Process engineering / R&amp;D roles</h3>
      <p>Wet processing, process development, PFDs, mass and energy balances, experimental design, and manufacturing translation.</p>
    </div>
    <div class="matrix-card contact-fit-card reveal" style="--reveal-delay: 140ms">
      <span class="fit-index">02</span>
      <h3>Advanced manufacturing + semiconductors</h3>
      <p>Printed electronics, semiconductor process development, reliability testing, process control, and data-driven decision rules.</p>
    </div>
    <div class="matrix-card contact-fit-card reveal" style="--reveal-delay: 220ms">
      <span class="fit-index">03</span>
      <h3>Clean technology deployment</h3>
      <p>Industrial decarbonization, sustainable materials, clean infrastructure, scale-up, and research-to-deployment pathways.</p>
    </div>
  </div>
</section>

<section class="contact-closing-card reveal" style="--reveal-delay: 80ms">
  <div>
    <p class="system-label small">TECHNICAL PROOF FIRST</p>
    <h2>Want the engineering context before reaching out?</h2>
    <p>Start with the micromodular deposition case study: it shows how I translate messy physical behavior into process variables, measurements, and engineering decisions.</p>
  </div>
  <a class="button secondary" href="{{ '/projects/micromodular-deposition/' | relative_url }}">View flagship case study</a>
</section>

<script>
  (() => {
    document.documentElement.classList.add('js');

    const revealItems = Array.from(document.querySelectorAll('.reveal'));
    if (!revealItems.length) return;

    const reducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
    if (reducedMotion || !('IntersectionObserver' in window)) {
      revealItems.forEach((item) => item.classList.add('in-view'));
      return;
    }

    const observer = new IntersectionObserver((entries, activeObserver) => {
      entries.forEach((entry) => {
        if (!entry.isIntersecting) return;
        entry.target.classList.add('in-view');
        activeObserver.unobserve(entry.target);
      });
    }, {
      threshold: 0.16,
      rootMargin: '0px 0px -8% 0px'
    });

    revealItems.forEach((item) => observer.observe(item));
  })();
</script>
