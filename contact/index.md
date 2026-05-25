---
layout: page
title: Contact
body_class: contact-page
category: Opportunities
subtitle: For internships, co-ops, research conversations, and process-engineering opportunities.
---

<div class="contact-system-grid contact-reveal">
 <section class="contact-card recruiter-contact contact-intro-panel" aria-label="Contact priorities">
 <p class="system-label small">LET'S CONNECT</p>
 <h2>Let’s connect around process engineering, R&amp;D, and manufacturing.</h2>
 <p>
 I’m interested in technical conversations involving wet processing, advanced materials, semiconductor process development, scale-up, reliability, biotech process development, and hard-tech deployment.
 </p>
 <div class="contact-signal-list" aria-label="Best-fit contact reasons">
 <span>Process development internships / co-ops</span>
 <span>Advanced manufacturing and semiconductor roles</span>
 <span>Research-to-engineering conversations</span>
 </div>
 <div class="resume-actions contact-action-row">
 <a class="button primary" href="mailto:{{ site.email }}">Start an Email</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download Resume</a>
 <a class="button tertiary" href="{{ site.linkedin }}">LinkedIn</a>
 <a class="button tertiary" href="{{ site.github }}">GitHub</a>
 </div>
 </section>

 <section class="contact-form-panel soft-form-panel" aria-label="Contact form">
 <div class="contact-panel-header">
 <p class="system-label small">DIRECT MESSAGE</p>
 <h2>Send a concise note.</h2>
 <p>Use this form for recruiting, project conversations, or technical collaboration. It routes to my portfolio inbox.</p>
 </div>
 <form class="contact-form" action="https://formspree.io/f/xkoeblkb" method="POST">
 <input type="hidden" name="_subject" value="Portfolio contact form message">
 <div class="form-grid">
 <label class="field">
 <span>Name</span>
 <input type="text" name="name" autocomplete="name" placeholder="Your name" required>
 </label>
 <label class="field">
 <span>Email</span>
 <input type="email" name="email" autocomplete="email" placeholder="you@example.com" required>
 </label>
 </div>
 <label class="field">
 <span>Message</span>
 <textarea name="message" rows="7" placeholder="A short note about the role, project, or technical conversation." required></textarea>
 </label>
 <button class="button secondary contact-submit" type="submit">Send Message <span aria-hidden="true">→</span></button>
 <p class="form-note">Fastest route: use the direct email button on the left.</p>
 </form>
 </section>
</div>

<section class="contact-methods contact-reveal" aria-label="Contact methods">
 <article>
 <span>Email</span>
 <strong>{{ site.email }}</strong>
 <a href="mailto:{{ site.email }}">Start an email →</a>
 </article>
 <article>
 <span>Resume</span>
 <strong>PDF download</strong>
 <a href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download resume →</a>
 </article>
 <article>
 <span>Projects</span>
 <strong>Engineering case files</strong>
 <a href="{{ '/projects/' | relative_url }}">View work →</a>
 </article>
</section>

<section class="contact-fit-panel contact-reveal" aria-label="Best-fit conversations">
 <p class="system-label small">BEST-FIT CONVERSATIONS</p>
 <div class="matrix contact-fit-grid">
 <div class="matrix-card"><h3>Process engineering internships / co-ops</h3><p>Wet processing, process development, PFDs, balances, simulation, and plant/manufacturing environments.</p></div>
 <div class="matrix-card"><h3>Advanced manufacturing roles</h3><p>Semiconductors, printed electronics, process control, reliability, and manufacturing decision rules.</p></div>
 <div class="matrix-card"><h3>Biotech process development</h3><p>Microfluidics, stem-cell encapsulation, microscopy QC, and scale-up-aware biological workflows.</p></div>
 <div class="matrix-card"><h3>Early-stage hard-tech</h3><p>Comfortable being the only ChemE in the room and helping define the first version of a wet-processing, automation, or scale-up workflow.</p></div>
 </div>
</section>
