# Tijil Chhabra

I build ML systems, agent pipelines and data products, and I design them so they
can't make things up: grounded outputs, fail-closed checks, and numbers I can defend.
Data Science @ UC San Diego, class of 2028.

[tijilchhabra.tech](https://tijilchhabra.tech) · [LinkedIn](https://linkedin.com/in/tijil-chhabra) · tchhabra@ucsd.edu

---

## Where I've worked

**PwC** · SWE Intern (AI/ML) · Jun 2026 to Aug 2026<br>
Built a multi-agent nudge platform for a top-3 Indian private bank on a LangGraph
state machine and Postgres, with an admin surface and a customer surface. Scaled the
nudge catalogue from 10 to 33 through 7 reusable capability packs. Replaced
LLM-generated product suggestions, which invented offers that didn't exist, with a
grounded recommendation engine: fail-closed eligibility, RAG scoped to explanation
only, and product ids validated in code with a deterministic fallback. Zero
hallucinated products in offline evaluation on a demo customer dataset, not
production traffic. Added 20 tests, suite green at 35/35, no new runtime dependencies.

**Lawgical** · Software Engineer Intern (AI/ML) · Jul 2025 to Sep 2025<br>
Shipped a full-stack document OCR service (Next.js + Express) into the production
website, cutting manual data entry 40–50%. Built GCP Document AI pipelines for 6
document types at 90%+ accuracy, then added an LLM post-processing stage for a
further 6–10 points. Built a Claude Opus classifier that labels 10+ US visa
document types.

**DGLiger** · Data Science Intern · Jul 2024 to Sep 2024<br>
Three services in one internship for a partner bank's Data-as-a-Service initiative:
Databricks ETL pipelines and schemas over raw transactional data, a FAISS
vector-similarity service that surfaces high-value prospects for merchant partners,
and a Prophet cashflow forecaster for SME liquidity.

**DataHacks, DS3 @ UC San Diego** · Director · Oct 2024 to now<br>
Directed San Diego's largest hackathon: 36 hours, MLH-certified, 450 hackers from
70+ universities, $90K in sponsorship.

---

## Projects

**[Portfolio Manager](https://github.com/tijilchhabra1729/portfolio-manager)** · Live portfolio tracker for NSE and US markets<br>
Upload holdings from Excel or a broker CSV and get live prices, a FIFO cost-basis
ledger, realised and unrealised P&L, and alerts for concentration, small-cap
exposure and allocation drift. A LangGraph team (orchestrator → market → sector
specialists) reads Google News and Yahoo Finance and writes a weekly briefing. Money
is `Decimal` end to end, never a float. 244 tests. Free-tier hosting, so the first
load can take 30–60 s.<br>
`FastAPI` `PostgreSQL` `Supabase` `LangGraph` `Claude` `yfinance` · [live](https://portfolio-manager-sikd.onrender.com/)

**[T Cell Swarming Simulation](https://github.com/tijilchhabra1729/active-matter)** · Why T cell swarms stop themselves<br>
Wrote the simulation engine for our 4-person team at UCSD's Active Matter hackathon
in under 24 hours: self-propulsion, Vicsek alignment, chemotaxis, receptor
desensitization and excluded-volume forces. Limit tests switch off each mechanism in
turn and check the model collapses to the known simpler regime. The swarm on
[my site](https://tijilchhabra.tech) runs on the same rules, and you can play
against it.<br>
`Python` `NumPy` `Matplotlib`

**[TweetGuard](https://github.com/tijilchhabra1729/TweetGuard)** · Hate speech detection under class imbalance<br>
31,962 labeled tweets, 7% positive, so a 0.5 threshold is the wrong default. NLTK
preprocessing, GloVe 50d embeddings, 3 stacked BiLSTMs, and a decision threshold
tuned off the precision-recall curve.<br>
`TensorFlow` `Keras` `NLTK` · [site](https://tijilchhabra1729.github.io/TweetGuard/)

**[Do High-Calorie Recipes Taste Better?](https://github.com/tijilchhabra1729/do-high-calorie-recipes-taste-better)** · 83K recipes, 732K reviews<br>
No: p = 0.072 on a permutation test. Also MNAR missingness analysis, and a
class-balanced Random Forest tuned with 5-fold GridSearchCV that lifts minority-class
recall from 0% to 12%.<br>
`pandas` `scikit-learn` · [site](https://tijilchhabra1729.github.io/do-high-calorie-recipes-taste-better/)

**[SoleSavings](https://github.com/tijilchhabra1729/SoleSavings)** · Sneaker price aggregator<br>
Plugin-style scrapers pull live listings from several marketplaces into one SQLite
store, so adding a marketplace never touches core code.<br>
`Flask` `SQLite` `BeautifulSoup` `Selenium`

---

## Also

- AWS Certified Cloud Practitioner · [verify](https://www.credly.com/badges/4ca0b880-e13a-4864-9f5e-23564ebb50dd)

---

<details>
<summary><b>Full stack</b></summary>
<br>

**Languages**<br>
Python · SQL · JavaScript · Java · R · HTML/CSS

**AI and ML**<br>
LangGraph · Claude API · RAG · FAISS · TensorFlow / Keras · scikit-learn · Prophet · NLTK · GloVe · GCP Document AI

**Data**<br>
pandas · NumPy · PySpark · Databricks · PostgreSQL · SQLite · SQLAlchemy · D3.js

**Backend and infra**<br>
FastAPI · Flask · Next.js · Express · Docker · Supabase · Render · GCP · AWS · Git

</details>
