---
layout: page
title: Publications
permalink: /publications/
---

<p>
My publications span academic scholarship, policy analysis, and public-facing commentary across emerging technology, security, infrastructure, and philosophy of (the social) science(s). The mix reflects a career spent moving between research, government, and regulation, and an enduring interest in making technical and political worlds legible to one another.
</p>

<div class="research-nav">
  <p class="research-nav-title">Browse by type</p>
  <ul>
    <li><a href="#working-papers"><span class="research-marker">1</span> Work in Progress</a></li>
    <li><a href="#journal-articles"><span class="research-marker">2</span> Journal Articles</a></li>
    <li><a href="#book-chapters"><span class="research-marker">3</span> Book Chapters</a></li>
    <li><a href="#policy-reports"><span class="research-marker">4</span> Policy Reports</a></li>
    <li><a href="#commentary-and-essays"><span class="research-marker">5</span> Commentary and Essays</a></li>
    <li><a href="#other-publications"><span class="research-marker">6</span> Other Publications</a></li>
  </ul>
</div>

<section id="working-papers" class="research-block">
  <h2><span class="research-marker">1</span> Working Papers</h2>
  {% if site.data.publications.working_papers and site.data.publications.working_papers.size > 0 %}
  <ol class="publication-list">
    {% for pub in site.data.publications.working_papers %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
  {% else %}
  <p><em>[Drafts and works in progress will be added here once they are ready for public circulation.]</em></p>
  {% endif %}
</section>

<section id="journal-articles" class="research-block">
  <h2><span class="research-marker">2</span> Journal Articles</h2>
  <ol class="publication-list">
    {% for pub in site.data.publications.journal_articles %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>

<section id="book-chapters" class="research-block">
  <h2><span class="research-marker">3</span> Book Chapters</h2>
  <ol class="publication-list">
    {% for pub in site.data.publications.book_chapters %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>

<section id="policy-reports" class="research-block">
  <h2><span class="research-marker">4</span> Policy Reports</h2>
  <ol class="publication-list">
    {% for pub in site.data.publications.policy_reports %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>

<section id="commentary-and-essays" class="research-block">
  <h2><span class="research-marker">5</span> Commentary and Essays</h2>
  <ol class="publication-list">
    {% for pub in site.data.publications.commentary_and_essays %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>

<section id="other-publications" class="research-block">
  <h2><span class="research-marker">6</span> Other Publications</h2>
  <ol class="publication-list">
    {% for pub in site.data.publications.other_publications %}
    <li class="publication-item">
      {{ pub.citation }}
      {% if pub.doi or pub.url %}
      <span class="publication-links">
        {% if pub.doi %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.url %}{% if pub.doi %} · {% endif %}<a href="{{ pub.url }}">{{ pub.link_label | default: "Link" }}</a>{% endif %}
      </span>
      {% endif %}
    </li>
    {% endfor %}
  </ol>
</section>
