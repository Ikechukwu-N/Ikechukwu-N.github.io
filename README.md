# Ikechukwu Nwaigwe — Portfolio Site

Single-page portfolio built in the style of BootstrapMade's **"Personal"** template
(the one Somto Lily's site uses): a full-screen dark landing page with your name
centered and horizontal nav links beneath it. Clicking a link shrinks the header
into a compact top bar and fades in the chosen section — sections toggle rather
than scroll. Built from scratch, so no BootstrapMade license/attribution needed
and no jQuery.

## Structure

```
portfolio/
├── index.html              ← everything (HTML + CSS + JS in one file)
└── assets/
    ├── img/
    │   ├── profile.jpg     ← ADD: your profile photo (square, ~500x500px works well)
    │   └── portfolio/      ← ADD: project screenshots (project-1.png ... project-6.png)
    └── files/
        └── resume.pdf      ← ADD: your resume PDF
```

## Already filled in with your real content

- Landing: name, typed roles, nav (Home / About / Resume / Portfolio / Contact / LinkedIn ↗)
- About: headline, summary (Jean Edwards product delivery, PwC, Manchester MSc + PTDF),
  info grid (no status row), skill chips with logos (no percentages), awards, and the
  "What if?" quote band
- Resume, two columns:
  - Left: Education — MSc Business Analytics & AI with relevant modules
    (Python Programming for Business Analytics, Machine Learning for Business,
    Digital Strategy, AI Trends & AI Ethics), B.Eng with transcript modules,
    Napo — then Certifications
  - Right: Professional Experience (Jean Edwards, PwC, NASRDA, research project)
    then Volunteer Experience
  - Download Resume button below
- Portfolio: no filters; hover overlays show title + tools + link; "Find these and
  more on my GitHub →" line on top
- Contact: email / LinkedIn / GitHub cards + Formspree form
- Deep links work: yoursite.com/#portfolio opens straight to the Portfolio section

## Things YOU still need to do (checklist)

1. [ ] Add assets/img/profile.jpg
2. [ ] Add assets/files/resume.pdf
3. [ ] Replace `yourusername` with your real GitHub username (appears 3 times)
4. [ ] Confirm your LinkedIn URL — currently linkedin.com/in/ikechukwu-nwaigwe
5. [ ] Set up the contact form (below)
6. [ ] Fill in the 6 portfolio cards as projects become ready
7. [ ] Optional: trim awards/certifications lists

## Contact form — Formspree (free)

Free tier: 50 submissions/month, no backend needed.

1. Sign up at https://formspree.io (free)
2. Create a form; you get an endpoint like https://formspree.io/f/abcd1234
3. In index.html, replace YOUR_FORM_ID in the form's action attribute
4. Submit once yourself to verify your email — done

To remove the form later, delete the <form class="cform">...</form> block.

## Deployment — GitHub Pages vs Vercel

Both free. Recommendation: **GitHub Pages** — recruiters clicking from your
portfolio to your GitHub see your repos right there.

### GitHub Pages steps
1. Create a repo (`portfolio`, or `yourusername.github.io` for a root URL)
2. Upload index.html + assets/ (web UI: Add file → Upload files)
3. Settings → Pages → Deploy from a branch → main / root → Save
4. Live in ~1 minute

### Vercel alternative
Connect the same GitHub repo at vercel.com → auto-deploys on every push.

### Custom domain (optional)
~$10–15/yr (Namecheap etc.); add a CNAME file to the repo + set DNS per
GitHub's docs. Free HTTPS included.

## Notes

- Skill logos load from the devicon CDN; Power BI, Tableau, and Excel use built-in
  colored monogram badges (not available on devicon).
- Portfolio hover overlays stay permanently visible on touch devices.
- Reduced-motion preferences respected (typing animation becomes static).
