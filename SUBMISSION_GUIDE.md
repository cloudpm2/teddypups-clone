# Submission Guide (step by step)

## 1. Accept the assignment (starts 48h clock)
Reply to hr@instabizweb.com confirming acceptance. Deadline = 48 hours from that reply.

## 2. Push to GitHub
```bash
cd teddypups-clone
git init
git add .
git commit -m "feat: TeddyPups website clone (HTML/CSS/JS)"
git branch -M main
# create an empty repo named teddypups-clone on github.com first
git remote add origin https://github.com/<your-username>/teddypups-clone.git
git push -u origin main
```

## 3. Deploy (pick one — all free)
**Vercel:** vercel.com → Add New → Project → import the GitHub repo → Framework "Other" → Deploy.
**Netlify:** app.netlify.com → Add new site → Import from Git → no build command, publish dir `.` → Deploy.
**GitHub Pages:** Repo → Settings → Pages → Branch `main` / root → Save.
Open the live URL and click every page + test on your phone.

## 4. Test checklist
- [ ] All 8 pages open, nav active state correct
- [ ] Mobile menu opens/closes (resize to 375px)
- [ ] Filters on /puppies work, URL params work
- [ ] Each puppy detail loads; gallery arrows work; form validates
- [ ] FAQ accordion + search
- [ ] Lightbox on Happy families (Esc closes)
- [ ] WhatsApp links open
- [ ] Lighthouse (Chrome DevTools) mobile score

## 5. Loom video (5–8 min) — script
1. **Intro (30s):** name, task, show reference site vs yours.
2. **Process & structure (1.5m):** open folder; explain css/, js/data.js, js/main.js, page shells.
3. **Tech & tools (1m):** HTML5, CSS custom properties/grid/flex, vanilla JS, Git/GitHub, Vercel/Netlify, Claude (AI).
4. **AI usage (1.5m):** show your real prompts (see below) — read them out exactly as you used them.
5. **Decisions & challenges (1.5m):** vanilla JS vs React (no build, fast); data in one file; `puppy.html?slug=` because static hosting has no dynamic routes; media hotlinked; matching animations/responsive.
6. **Testing & deployment (1m):** show checklist, Lighthouse, deploy dashboard, live URL.

### Prompts used (copy into your video — use your exact wording)
1. "Clone the complete website https://puppy.instabizweb.com/ — match design, layout, responsiveness and functionality. Step by step."
2. Claude fetched every page of the reference site (home, puppies, puppy detail, how-it-works, FAQ, contact, happy-families) to extract content and structure.
3. "Build it as a static multi-page site with shared header/footer, filters, slider, lightbox, accordion and validated enquiry forms."

## 6. Submission email
**To:** hr@instabizweb.com  **CC:** neelnsoni1306@gmail.com
**Subject (exact):** `Technical Assignment Submission – [Pratik mistry] – Insta Biz Web`

```
Hello Team,

Please find my assignment submission:

Live Website: <url>
GitHub Repository: <url>
Loom Video: <url>

Thank you,
Pratik Mistry
```
