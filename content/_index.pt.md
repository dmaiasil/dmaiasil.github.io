---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ''
      button:
        text: Baixar currículo (em inglês)
        url: /uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: '🏛️ Minha missão'
      subtitle: ''
      text: |-
        Minha missão é **liderar e construir sistemas de IA éticos, explicáveis e de impacto real**, transformando a forma como as organizações usam dados para tomar decisões melhores e mais responsáveis.  

        Como **educadora e palestrante internacional**, sou apaixonada por **democratizar a tecnologia** por meio da inclusão e do compartilhamento de conhecimento. Também me dedico a levar ensino de alta qualidade em ciência de dados e machine learning a quem fala português.  

        Com minhas palestras e colaborações, busco **aproximar sistemas complexos de IA da compreensão humana**, inspirando equipes e públicos a usar os dados para o bem.  

        📩 *Aberta a colaborações, convites para palestras e iniciativas que impulsionem a inovação ética.*  

        **Afinal, o que os dados podem fazer por você?**
    design:
      columns: '1'

  - block: collection
    id: talks
    content:
      title: Destaques e próximas palestras
      filters:
        folders:
          - events
    design:
      view: article-grid
      columns: 2

  - block: markdown
    content:
      title: "💬 Depoimentos"
      subtitle: ""
      text: |-
        <div class="testimonials">
          <figure>
            <blockquote>
              “A sabedoria e a autenticidade da Debs na SHPE Convention foram realmente inspiradoras.  
              Suas reflexões sobre crescimento profissional e sobre como enfrentar desafios me tocaram profundamente.  
              É daquelas palestras que ficam com a gente.”
            </blockquote>
            <figcaption>— <strong>Darwing Vargas</strong>, Career Assistant, RPI <span class="translation-note">(tradução livre)</span></figcaption>
          </figure>

          <figure>
            <blockquote>
              “A palestra da Debs no RTC Summit foi profundamente inspiradora. Sua autenticidade e suas reflexões sobre como encontrar o seu nicho na tecnologia me marcaram e mostraram como alinhar seus pontos fortes a um propósito leva a uma carreira mais significativa na área.”  
            </blockquote>
            <figcaption>— <strong>Vaishnavi Rajendra Dhotargavi</strong>, Machine Learning Engineer, BulkMagic <span class="translation-note">(tradução livre)</span></figcaption>
          </figure>
        </div>

        <style>
          .testimonials { 
            max-width: 52rem; 
            margin: 2rem auto; 
            padding: 1rem 1.25rem; 
            text-align: center; 
          }
          .testimonials figure { 
            margin: 2rem 0; 
          }
          .testimonials blockquote { 
            font-size: 1.1rem; 
            line-height: 1.7; 
            margin: 0 0 0.75rem; 
            font-style: italic; 
          }
          .testimonials figcaption { 
            font-size: 0.95rem; 
            color: var(--muted, #555); 
          }
          .testimonials .translation-note { 
            font-size: 0.85rem; 
            font-style: italic; 
          }
        </style>
    design:
      columns: '1'

  - block: cta-card
    content:
      title: "📩 Convide para uma palestra"
      text: "Leve uma palestra da Debs para a sua empresa ou evento."
      button:
        text: "Fale com a Debs por e-mail"
        url: "mailto:missdmaia@gmail.com"
    design:
      card:
        css_class: 'bg-primary-100 cta-fix'

  - block: collection
    id: publications
    content:
      title: Publicações
      filters:
        folders:
          - publications
    design:
      view: article-grid
      columns: 2
---
