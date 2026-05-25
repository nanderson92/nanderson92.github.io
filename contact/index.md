---
layout: page
title: Contact
body_class: contact-page
category: Contact
subtitle: For co-ops, contract work, research conversations, and hard-tech buildout.
---

<div class="contact-system-grid contact-reveal builder-contact-grid">
 <section class="contact-card recruiter-contact contact-intro-panel" aria-label="Contact priorities">
 <p class="system-label small">LET'S CONNECT</p>
 <h2>Send me the weird manufacturing problem.</h2>
 <p>I’m interested in wet processing, printed electronics, semiconductor-adjacent R&amp;D, biotech process development, embedded controls, clean technology, and small hard-tech teams trying to make a first process work.</p>
 <div class="resume-actions contact-action-row primary-contact-actions">
 <a class="button primary" href="mailto:{{ site.email }}">Email me directly</a>
 <a class="button secondary" href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Resume (PDF, 1 page)</a>
 <a class="button tertiary" href="{{ site.linkedin }}">LinkedIn</a>
 <a class="button tertiary" href="{{ site.github }}">GitHub</a>
 </div>
 </section>

 <section class="contact-form-panel soft-form-panel" aria-label="Contact form">
 <div class="contact-panel-header">
 <p class="system-label small">DIRECT MESSAGE</p>
 <h2>Short notes are best.</h2>
 <p>This form is wired to my email through Formspree. Direct email is still fastest for roles, projects, and founder conversations.</p>
 </div>
 <form class="contact-form" action="https://formspree.io/f/xkoeblkb" method="POST">
 <input type="hidden" name="_subject" value="Portfolio contact form message">
 <div class="form-grid">
 <label class="field"><span>Name</span><input type="text" name="name" autocomplete="name" placeholder="Your name" required></label>
 <label class="field"><span>Email</span><input type="email" name="email" autocomplete="email" placeholder="you@example.com" required></label>
 </div>
 <label class="field"><span>Message</span><textarea name="message" rows="7" placeholder="A short note about the role, project, or technical problem." required></textarea></label>
 <button class="button secondary contact-submit" type="submit">Send message <span aria-hidden="true">→</span></button>
 <p class="form-note">Prefer less friction? Email me directly at <a href="mailto:{{ site.email }}">{{ site.email }}</a>.</p>
 </form>
 </section>
</div>

<section class="contact-methods contact-reveal" aria-label="Contact methods">
 <article><span>Email</span><strong>{{ site.email }}</strong><a href="mailto:{{ site.email }}">Start an email →</a></article>
 <article><span>Resume</span><strong>PDF download</strong><a href="{{ '/assets/files/Nathan_Anderson_Resume.pdf' | relative_url }}" download="Nathan_Anderson_Resume.pdf">Download resume →</a></article>
 <article><span>Projects</span><strong>Build logs</strong><a href="{{ '/projects/' | relative_url }}">View work →</a></article>
</section>

<section class="contact-fit-panel contact-reveal" aria-label="Best-fit conversations">
 <p class="system-label small">BEST-FIT CONVERSATIONS</p>
 <div class="matrix contact-fit-grid">
 <div class="matrix-card"><h3>Process development roles</h3><p>Wet processing, PFDs, balances, scale-up, and plant/manufacturing environments.</p></div>
 <div class="matrix-card"><h3>Advanced manufacturing teams</h3><p>Semiconductors, printed electronics, process control, reliability, and manufacturing decision rules.</p></div>
 <div class="matrix-card"><h3>Biotech process development</h3><p>Microfluidics, stem-cell encapsulation, microscopy QC, and scale-up-aware biological workflows.</p></div>
 <div class="matrix-card"><h3>Early-stage hard-tech (pre-Series A)</h3><p>Comfortable being the only ChemE in the room and figuring out the first version of your wet-processing line.</p></div>
 </div>
</section>
