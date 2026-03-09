---
layout: default
title: Tutorials
---

<div class="tutorial-header">
    <h1>Programming Tutorials</h1>
    <p>Step-by-step guides on the Art of Software.</p>
</div>

<div class="tutorial-list">
    {% assign tutorials = site.posts | where: "category", "tutorial" %}
    {% for post in tutorials %}
    <div class="tutorial-card">
        <small class="category-tag">Tutorial</small>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt | strip_html | truncatewords: 20 }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Start Learning →</a>
    </div>
    {% empty %}
    <div class="no-posts">
        <p>New tutorials are being drafted. Check back soon!</p>
    </div>
    {% endfor %}
</div>

<style>
    .tutorial-header {
        background: var(--navy);
        color: var(--white);
        padding: 3rem 1.5rem;
        text-align: center;
        border-bottom: 4px solid var(--peru);
        margin: -20px -20px 20px -20px; /* Counteracts main padding */
    }

    .tutorial-card {
        background: var(--white);
        padding: 1.5rem;
        border-radius: 8px;
        margin-bottom: 20px;
        box-shadow: 0 4px 12px rgba(0,0,0,0.08);
        border-top: 3px solid var(--peru);
    }

    .category-tag {
        color: var(--peru);
        text-transform: uppercase;
        font-weight: bold;
        font-size: 0.75rem;
        letter-spacing: 1px;
    }

    .tutorial-card h2 a {
        color: var(--navy);
        text-decoration: none;
    }

    .read-more {
        color: var(--peru);
        font-weight: bold;
        text-decoration: none;
        display: inline-block;
        margin-top: 10px;
    }
</style>
