---
layout: default
title: What's new — PixFinder
description: The latest improvements and releases for PixFinder.
permalink: /whats-new/
---

<main>
  <section style="background:radial-gradient(900px 360px at 65% -5%, #E1F4FF 0%, rgba(225,244,255,0) 65%), #FBFBFD; border-bottom:1px solid #EAECF2;">
    <div class="pf-container" style="max-width:900px; margin:0 auto; padding:88px 32px 72px; text-align:center;">
      <p style="margin:0 0 14px; color:#00A3FF; font-size:14px; font-weight:700; letter-spacing:.08em;">PIXFINDER RELEASE NOTES</p>
      <h1 class="pf-hero-h1" style="font-family:'Space Grotesk',sans-serif; font-size:56px; line-height:1.04; letter-spacing:-.03em; margin:0 0 18px;">What's new</h1>
      <p style="max-width:600px; margin:0 auto; color:#5A6472; font-size:18px; line-height:1.6;">Every improvement, feature and fix in PixFinder</p>
    </div>
  </section>

  <section class="pf-container" style="max-width:900px; margin:0 auto; padding:64px 32px 88px;">
    <div style="display:grid; gap:16px;">
      {% assign releases = site.releases | sort_natural: 'version' | reverse %}
      {% for release in releases %}
      <a href="{{ release.url | relative_url }}" style="display:flex; align-items:center; justify-content:space-between; gap:24px; padding:26px 28px; color:inherit; text-decoration:none; background:#fff; border:1px solid #EAECF2; border-radius:16px; box-shadow:0 12px 30px -26px rgba(20,26,45,.28);">
        <div>
          <span style="display:block; color:#00A3FF; font-size:13px; font-weight:700; letter-spacing:.06em; margin-bottom:7px;">RELEASE</span>
          <h2 style="font-family:'Space Grotesk',sans-serif; font-size:23px; letter-spacing:-.02em; margin:0;">Version {{ release.version }}</h2>
        </div>
        <span aria-hidden="true" style="font-size:25px; color:#00A3FF;">→</span>
      </a>
      {% endfor %}
    </div>
  </section>
</main>
