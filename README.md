# ✈️ TaxPilot — Free US Tax Help Website

> Free tax calculators, guides, and smart answers for individuals, startups, and corporations. No ads. No data collection. No products sold.

---

## 🚀 Deploy to Vercel in 60 Seconds

### Option A — Drag & Drop (Easiest)
1. Go to [vercel.com](https://vercel.com) and sign up / log in (free)
2. Click **"Add New Project"** → **"Deploy"**
3. Drag the entire `taxpilot/` folder onto the Vercel upload area
4. Click **Deploy** — you're live in ~30 seconds

### Option B — Vercel CLI
```bash
npm install -g vercel
cd taxpilot/
vercel --prod
```

### Option C — GitHub (Recommended for updates)
1. Push this folder to a GitHub repo
2. Connect the repo to Vercel at vercel.com/new
3. Vercel auto-deploys every time you push a change

---

## 📁 Project Structure

```
taxpilot/
├── index.html      ← Entire website (HTML + CSS + JS in one file)
├── vercel.json     ← Vercel deployment config & security headers
├── robots.txt      ← SEO: tells search engines to index everything
├── sitemap.xml     ← SEO: sitemap for Google/Bing
└── README.md       ← This file
```

---

## 🌐 What's Built In (Zero External Dependencies)

| Feature | How It Works | Cost |
|---|---|---|
| Income Tax Calculator | IRS 2025 brackets hardcoded | Free |
| Capital Gains Calculator | Long/short term rate logic | Free |
| Refund Estimator | Credits + withholding math | Free |
| SE Tax Calculator | 15.3% SE tax formula | Free |
| Quarterly Tax Calculator | Bracket + SE tax estimate | Free |
| Home Ownership Calculator | SALT cap + mortgage interest | Free |
| Vehicle Mileage Calculator | $0.70/mi 2025 standard rate | Free |
| Depreciation Calculator | SL / Sec 179 / Bonus / DDB | Free |
| Payroll Tax Calculator | FICA + FUTA + SUTA | Free |
| AI Tax Assistant | 20+ pre-built expert answers, keyword matching | Free |
| IRS Tax News Feed | IRS RSS → rss2json.com (no key needed) | Free |
| Entity Comparison | Full LLC/S-Corp/C-Corp table | Free |
| Deduction Checklist | Interactive 12-item startup checklist | Free |
| FAQ (10 questions) | Accordion, built-in | Free |
| SEO Article | 2,500+ words, structured content | Free |

---

## 🔧 Customisation

### Change the Domain Name
After deploying on Vercel:
1. Go to your project settings → Domains
2. Add your custom domain
3. Update the `sitemap.xml` and meta tags in `index.html` with your domain

### Update Tax Data (Annual)
Each January, update these values in `index.html`:
- `BRACKETS_2025` object (new tax brackets)
- `STD_DEDUCT` object (new standard deductions)
- Mileage rate (search `0.70` → new rate)
- 401k/IRA limits (search `23,500` / `7,000`)
- SS wage cap (search `176,100`)

### Add Google Analytics (Optional)
Add before `</head>`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer=window.dataLayer||[];
  function gtag(){dataLayer.push(arguments);}
  gtag('js',new Date());
  gtag('config','G-XXXXXXXXXX');
</script>
```

---

## 📈 SEO Tips to Rank

1. **Submit your sitemap** to Google Search Console → Sitemaps → `https://yourdomain.com/sitemap.xml`
2. **Register on Bing Webmaster Tools** — submit sitemap there too
3. **Build backlinks** by posting the tool in Reddit communities: r/personalfinance, r/tax, r/smallbusiness, r/freelance
4. **Update annually** — Google rewards freshness; update rates every January
5. **Add structured data** — the schema.org markup is already included in `<head>`

---

## ⚖️ Legal Notice

TaxPilot provides general tax education for informational purposes only. It is not legal or financial advice. Always consult a qualified CPA, Enrolled Agent, or Tax Attorney for advice specific to your situation.

---

Built with ❤️ for every American taxpayer.
