# AI Dev Notes 

---

## 1) Prompt Log - Some of the prompts give to Cursor

### P1 — Project scaffold and base styles
**Prompt:**  
Create a structure for an HTML/CSS based personal website. I need six pages (home, about, resume, projects, contact, thankyou), one shared `styles.css`, and an `/images` folder with placeholders. Each page should use semantic HTML (`header / nav / main / footer`). Add a modern base stylesheet with color/font tokens, spacing, and simple grid/flex helpers. No real content yet—just structure.

**What the AI gave me:**  
It created the folders and files, added boilerplate to each page, and built a neat base stylesheet with formatting and simple grids. All pages link to the same CSS and feel consistent.

**What I changed & why:**  
Kept almost everything, it was a good starting point for structure. Tested and fixed a couple of broken links.

---

### P2 — Home page (index)
**Prompt:**  
Turn `index.html` into a proper homepage: with name + short subheading, quick teasers and links for all the other pages, and a footer that includes a GitHub repo link. Keep it responsive and add gentle hover/focus effects.

**What the AI gave me:**  
A clean, short intros for all the remaining pages with generic content and a friendly CTA to Contact. 

**What I changed & why:**  
Tweaked the content to sound more like me and align with what I want to convey and made the button labels a touch clearer.

---

### P3 — About page (personal + professional)
**Prompt:**  
Make `about.html` match the look of the Home page. Add introducion sections plus goals, a skills section and a current coursework, and past leadership sections. Use a headshot from images folder with a plain, descriptive alt.

**What the AI gave me:**  
A friendly, professional About page that matches Home. The image is set up with descriptive alt text. It also gave catchy titles for the sections

**What I changed & why:**  
Replaced the content that was generic, added a few more skills manually in the skills section. Fixed the path for headshot as it included main folder title as well.

---

### P4 — Resume page (with PDF view/download)
**Prompt:**  
Build `resume.html` to match the site. Add a **Download** button for the pdf file under assets, and use the attached resume to extract information, and format it through html on the page.

**What the AI gave me:**  
A well-structured page with both download buttons and scannable sections. Consistent with other pages.

**What I changed & why:**  
Mostly kept it as-is. Fixed couple of formatting and spacing to align better with my actual resume and made it visually better.

---

## 2) Reflection 

Using AI for this personal website turned out to be very useful. The biggest time saver was the repetitive setup—folders, HTML boilerplate, shared CSS, and consistent page shells. It kept the look and structure aligned across pages so I could spend more time on content and polish. It helped make quick changes in headers or footers without manually having to go and change in every page. I also liked how quickly I could try different tones for the About page until it felt personal, and still professional.

Where AI made mistakes
- It put my headshot under /assets and used backslashes in paths. I moved the photo to /images/Headshot.jpg and fixed all paths to forward slashes.
- First drafts sounded like a résumé recap. I rewrote it to be warmer, personal, and still professional.
- Early ideas had form values sending in the URL. I kept the flow client-side and used sessionStorage only for first name, then cleared it.
- A few button labels and headings were inconsistent across pages. I standardized wording and capitalization.

How I balanced AI assistance with my own coding
- AI was used for speed and structure. I relied on my judgment and knowledge from my experiences to validate and enhance the code. I let AI handle scaffolding, shared CSS, and repeating page shells, then I reviewed every page with a quick checklist (headings, links, content).
- I iterated the About page copy until it felt authentically me—friendly, confident, and not overly formal.
- I verified relative links, fixed broken links and paths, ensured that images and assets were in correct folder, and kept button/section names consistent.
- I fixed minimal logic for javascript code used for password match and the thank-you greeting, avoided query strings, and cleared temporary data.

---