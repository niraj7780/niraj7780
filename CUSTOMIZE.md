# 🛠️ CUSTOMIZE.md — every placeholder you still need to fill in

This file lists **all placeholders** left in [`README.md`](./README.md), what each one is for, and an example of what to type instead.

**Quick find:** run `grep -n "YOUR_" README.md` in this folder to jump to every placeholder line.

---

## 1. Contact placeholders (section: Connect With Me)

| Placeholder | Appears in | Replace with | Example |
|---|---|---|---|
| `YOUR_LINKEDIN_URL` | `<a href="YOUR_LINKEDIN_URL">` | Your full LinkedIn profile URL | `https://www.linkedin.com/in/your-name-123456/` |
| `YOUR_PROFESSIONAL_EMAIL` | `<a href="mailto:YOUR_PROFESSIONAL_EMAIL">` | Your professional email address only (no `mailto:` prefix, it is already in the code) | `niraj.charpe@example.com` |
| `YOUR_PORTFOLIO_URL` | `<a href="YOUR_PORTFOLIO_URL">` | Your portfolio / personal website | `https://your-portfolio.example` |
| `YOUR_RESUME_URL` | `<a href="YOUR_RESUME_URL">` | A public link to your résumé (Google Drive, GitHub repo, or website page) | `https://example.com/resume.pdf` |

> ✅ Your GitHub link is already real and correct: `https://github.com/niraj7780`.
> 📵 **Never** add your phone number, employee ID, client names or any internal company details to this file.

---

## 2. Featured project placeholders (section: ⭐ Featured Project — Bank Management System)

| Placeholder | Appears in | Replace with | Example |
|---|---|---|---|
| `YOUR_REPOSITORY_URL` | Project resource table **and** the installation code block | Public GitHub repo URL of your Bank Management System | `https://github.com/niraj7780/bank-management-system` |
| `YOUR_SCREENSHOT_URL` | Project resource table | Direct link to a terminal screenshot | `https://raw.githubusercontent.com/niraj7780/bank-management-system/main/docs/screenshot.png` |
| `YOUR_DEMO_GIF_URL` | Project resource table | Direct link to a short screen recording | `https://raw.githubusercontent.com/niraj7780/bank-management-system/main/docs/demo.gif` |
| `YOUR_ENTRY_FILE.py` | Installation code block | Your actual entry file name | `main.py` or `bank_management.py` |
| Installation instructions | Code block marked _"placeholder, replace with your real steps"_ | The real commands to clone, install dependencies and run your project | see snippet below |
| Database setup instructions | SQL block marked _"placeholder, replace with your real steps"_ | Your real SQL Server database creation / schema / seed script | see snippet below |

### Example — after you fill it in

````markdown
**▶️ Installation instructions**

```bash
# 1. Clone the repository
git clone https://github.com/niraj7780/bank-management-system.git
# 2. Install the Python dependencies
pip install -r requirements.txt
# 3. Run the application
python main.py
```
````

````markdown
**🗄️ Database setup instructions**

```sql
-- 1. Create the database
CREATE DATABASE BankDB;
-- 2. Run schema + seed script
USE BankDB;
-- 3. Run your tables script here
```
````

### Adding the screenshot / demo GIF visually

Replace the "Screenshot & demo: coming soon" note with:

```html
<p align="center">
  <img src="YOUR_SCREENSHOT_URL" alt="Screenshot of the Bank Management System command-line interface showing a login prompt" width="700" />
</p>
```

```html
<p align="center">
  <img src="YOUR_DEMO_GIF_URL" alt="Animated demo of the Bank Management System: logging in, creating an account and making a deposit" width="700" />
</p>
```

---

## 3. Optional tweaks (no placeholder — edit freely)

| What | Where | Note |
|---|---|---|
| Animated header text | Top `<img src="https://capsule-render.vercel.app/...">` | Change `text=Niraj%20Charpe` or the `desc=` subtitle |
| Typing messages | Top `<img src="https://readme-typing-svg.demolab.com/...&lines=...">` | Messages are separated by `;` |
| Stats widget theme | Section 📊 GitHub Statistics | `theme=tokyonight` (stats, streak) and `theme=onedark` (trophies) — try `github-dark`, `radical`, `dracula` |
| Badge wording | Section 🛠️ Technical Skills | Keep honest labels: `learning`, `practising`, `fundamentals` |
| Colour accents | All badge URLs | Last colour value in each shields URL (e.g. `0FAAFF` blue, `00B8D9` cyan, `7C3AED` purple) |

---

## 4. Already verified — do not change

- **GitHub username** `niraj7780` is used in **all** widget URLs (stats, top languages, streak, trophies, contribution graph, visitor counter, followers, stars) and in your profile link.
- Every image/badge URL in `README.md` was requested live and returned **HTTP 200**, except:
  - `github-profile-trophy.vercel.app` → currently returns **402** (the trophy service is rate-limited today). It is placed inside a collapsible details block with descriptive alt text, so the README stays clean if it does not load. Re-check later with:
    `curl -s -o /dev/null -w "%{http_code}\n" "https://github-profile-trophy.vercel.app/?username=niraj7780"`
- Contribution activity graph uses `ghchart.rshah.org` (verified working) instead of the activity-graph service, which is returning 402.
- No JavaScript, iframes, external CSS, percentage skill bars or hand-written statistics anywhere.

---

## 5. Content / privacy rules this README follows (keep them when editing)

1. **HCLTech** = current employer; position = **IT Intern**.
2. **HCL TechBee** = completed training program (approx. 10 months).
3. **Bank Management System** = clearly labelled a *training project* — never "production", "deployed", or "used by banks".
4. **SAP ABAP** = *fundamentals / learning* level.
5. **Class 12** = Higher Secondary Education, completed.
6. No client names, confidential project info, employee IDs, managers, customer IDs, workstation or internal system details.
7. No phone number.
8. No invented certifications, experience, achievements or contact details.

---

## 6. Before you push checklist

- [ ] All `YOUR_*` placeholders replaced (except any you deliberately keep)
- [ ] Screenshot / demo GIF added to the project section
- [ ] Installation and database setup blocks contain your real steps
- [ ] Links open correctly (click each badge)
- [ ] Re-read the summary and project description for accuracy
- [ ] No personal or confidential information added
- [ ] README still renders well on mobile (preview on github.com)
