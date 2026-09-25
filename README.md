# Nishit S K

**Backend · Cloud · Data**, and frontend that has to rank — final-year CSE at Sahyadri College of Engineering, Mangaluru.
I build systems that run unattended, then measure them honestly enough to find out where they're wrong.

[nishit.app](https://nishit.app) · [LinkedIn](https://www.linkedin.com/in/nishit-s-k) · nishitsk42@gmail.com

---

## The thing I'd want you to read

**[CADSS — a carbon-aware cloud scheduler](https://github.com/NishitSK/CARBONMAJOR)**, running live on 13 AWS regions.

It places workloads on the cleanest electricity grid that still satisfies their latency SLA and data-residency law. Three scheduling policies run side by side, hourly, dispatching real jobs through AWS Systems Manager.

The scheduler cuts carbon intensity **94.7%** against a carbon-blind baseline. That number is also the least interesting thing about it:

- A held-out statistical decomposition (AR(1)-corrected, *p* < 10⁻¹⁰) shows **97% of the saving comes from picking the right region once** — not from reacting hour to hour. Most work in this area reports the big number and skips the split.
- I verified **25,000+ forecasts** against measured grid data. The model with the *lower* error made the *worse* decisions: it promised +12.7% savings and delivered −3.8%.
- So the system gates every forecast on its own verified record, and it disabled one of my two models. Later it withdrew a horizon from the other. A guard worth having has to be able to say no to you.

Paper accepted for presentation at an IEEE conference, October 2026.

---

## Shipped during my internship

**[squish.urudha.com](https://squish.urudha.com)** — free browser-based image tools (WebP conversion, compression, background removal, PDFs, watermarks, EXIF). Everything runs client-side; nothing is uploaded.

Built at **Urudha** (May–Jul 2026) in Next.js and React, where I also owned the search side of it:

- **Programmatic landing pages** for the queries people actually type — `jpg-to-webp`, `heic-to-webp`, `compress-image`, `batch-image-converter` — each with its own title, description and single H1 rather than one page pretending to be many.
- **Structured data**: FAQPage schema on the tool pages, plus WebSite, Organization and ItemList JSON-LD.
- **Crawl hygiene**: server-rendered routes, canonicals, Open Graph and Twitter cards, robots.txt and a 15-URL sitemap.
- **Core Web Vitals**: image optimisation, lazy loading and bundle-size reduction.

---

## Other work

| | | |
|---|---|---|
| **[Medallion Data Lake](https://github.com/NishitSK/airflow-spark-medallion-pipeline)** | Raw → Bronze → Silver → Gold ETL platform with validation and retries at each layer | Spark · Airflow · S3 · EC2 · Docker |
| **[EventSphere](https://github.com/NishitSK/EventSphere)** | Campus event platform, containerised and auto-deployed on every push to main | MERN · Docker · Nginx · GitHub Actions · EC2 |
| **[LearnPath-AI](https://github.com/NishitSK/LearnPath-AI)** | Personalised skill-gap analyser | JavaScript · LLM APIs |
| **[Pantry Guardian](https://github.com/NishitSK/PANTRY-GUARDIAN)** | Kitchen inventory with OCR receipt scanning and expiry prediction | Next.js · FastAPI · MongoDB · Gemini · Tesseract |

---

## Tools I reach for

**Python** · FastAPI · PyTorch · statsmodels · pandas · Spark · Airflow
**TypeScript / JavaScript** · React · Next.js · Node · Vite
**Search** technical SEO · structured data · Core Web Vitals
**AWS** EC2 · S3 · Systems Manager · CloudWatch · IAM · boto3
**Also** Docker · Nginx · GitHub Actions · MongoDB · MySQL · Git · Linux
