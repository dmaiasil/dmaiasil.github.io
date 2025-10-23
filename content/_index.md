---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: /uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium   # small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle  # circle (default), square, rounded

  - block: markdown
    content:
      title: '🏛️ My Mission'
      subtitle: ''
      text: |-
        My mission is to **lead and build AI systems that are ethical, explainable, and impactful**, transforming how organizations use data to make better, more responsible decisions.  

        As an **educator and international speaker**, I’m passionate about **democratizing technology** through inclusion and knowledge-sharing. I founded **Vem ser Dev** to empower Portuguese-speaking learners in Python and data science.

        Through my talks and collaborations, I aim to **bridge the gap between complex AI systems and human understanding**, inspiring teams and audiences to use data for good.  

        📩 *Open to collaboration, speaking engagements, and initiatives that drive ethical innovation.*  

        **So, what can data do for you?**
    design:
      columns: '1'

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card

  - block: markdown
    content:
      title: "💬 What People Say"
      subtitle: ""
      text: |-
        <div class="t-rotator" role="region" aria-label="Testimonials">
          <div class="t-track">
            <figure class="t-item">
              <blockquote>“Debs’ wisdom and authenticity at the SHPE Convention were truly inspiring. Her insights on career growth and navigating challenges resonated deeply. This is a talk that stays with you.”</blockquote>
              <figcaption>— <strong>Darwing Vargas</strong>, SHPE 2024 Attendee; Career Assistant, RPI</figcaption>
            </figure>

            <figure class="t-item">
              <blockquote>“Insightful, practical, and empowering. Debs connects AI to real people and real impact.”</blockquote>
              <figcaption>— <strong>Program Chair</strong>, Data & Ethics Summit</figcaption>
            </figure>

            <figure class="t-item">
              <blockquote>“One of the most thoughtful talks on navigating bias and building agency I’ve heard.”</blockquote>
              <figcaption>— <strong>Tech Leader</strong>, Fortune 100</figcaption>
            </figure>
          </div>

          <div class="t-dots" aria-hidden="true"></div>
        </div>

        <style>
          .t-rotator { --t-speed: 6500ms; max-width: 52rem; margin: 0 auto; padding: 1rem 1.25rem; }
          .t-track { position: relative; overflow: hidden; }
          .t-item { display: none; margin: 0; text-align: center; }
          .t-item blockquote { font-size: 1.125rem; line-height: 1.7; margin: 0 0 .75rem; }
          .t-item figcaption { font-size: .95rem; color: var(--muted, #555); }
          .t-item.is-active { display: block; animation: fadeIn .5s ease; }
          @keyframes fadeIn { from { opacity: 0; transform: translateY(4px); } to { opacity: 1; transform: translateY(0); } }
          /* Dots */
          .t-dots { display: flex; justify-content: center; gap: .4rem; margin-top: .75rem; }
          .t-dot { width: .5rem; height: .5rem; border-radius: 999px; background: #c8cbd1; opacity: .65; }
          .t-dot.is-active { background: currentColor; opacity: 1; }
        </style>

        <script>
          (function(){
            const root = document.currentScript.previousElementSibling.previousElementSibling; // .t-rotator
            const track = root.querySelector('.t-track');
            const items = Array.from(track.querySelectorAll('.t-item'));
            const dotsWrap = root.querySelector('.t-dots');

            if (!items.length) return;

            // Build dots
            items.forEach((_, i) => {
              const dot = document.createElement('button');
              dot.className = 't-dot';
              dot.type = 'button';
              dot.setAttribute('aria-label', 'Show testimonial ' + (i+1));
              dot.addEventListener('click', () => show(i, true));
              dotsWrap.appendChild(dot);
            });

            let i = 0, timer;
            function show(idx, userTriggered=false){
              items.forEach(el => el.classList.remove('is-active'));
              dotsWrap.querySelectorAll('.t-dot').forEach(el => el.classList.remove('is-active'));
              items[idx].classList.add('is-active');
              dotsWrap.children[idx].classList.add('is-active');
              i = idx;
              if (userTriggered) reset();
            }
            function next(){ show((i+1) % items.length); }
            function reset(){
              clearInterval(timer);
              timer = setInterval(next, getSpeed());
            }
            function getSpeed(){
              // Read CSS custom property (fallback to 6500ms)
              try {
                const v = getComputedStyle(root).getPropertyValue('--t-speed').trim();
                return v.endsWith('ms') ? parseInt(v) : 6500;
              } catch { return 6500; }
            }

            // Pause on focus/hover for accessibility
            root.addEventListener('mouseenter', () => clearInterval(timer));
            root.addEventListener('mouseleave', reset);
            root.addEventListener('focusin', () => clearInterval(timer));
            root.addEventListener('focusout', reset);

            show(0);
            reset();
          })();
        </script>
    design:
      columns: '1'

  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
        # featured_only: true   # uncomment if you only want featured items
    design:
      view: article-grid
      columns: 2
---
