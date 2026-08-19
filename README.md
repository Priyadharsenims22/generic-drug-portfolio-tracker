# generic-drug-portfolio-tracker
Excel-based strategic portfolio tool for prioritizing generic drug candidates — molecule scoring, R&D pipeline timelines, regulatory/patent tracking, and ROI modeling, built around India's generics market.
**Generic Drug Portfolio & R&D Pipeline Tracker**
An Excel-based strategic planning tool for prioritizing generic drug product candidates, built around the India generics market. Combines market/competitive scoring, R&D development timelines, regulatory & patent tracking, and financial (ROI) modeling into a single workbook.
What it does
Given a shortlist of candidate molecules, this tool helps answer:
Which products are worth pursuing first? (market size, competitive intensity, technical complexity, margin potential → auto-calculated priority score & tier)
What does the development timeline look like? (formulation → bioequivalence → regulatory filing → launch)
Where do we stand on IP/regulatory risk? (patent expiry, Paragraph IV opportunity, filing status per market)
Is it financially worth it? (R&D investment vs. estimated revenue, simple ROI)
Structure
Tab	Purpose

README	Legend and color-coding guide
1. Molecule Portfolio	Candidate molecules scored 1–5 across 4 criteria; priority score & tier calculated automatically
2. R&D Roadmap	Development-stage timeline (in months) per molecule
3. Regulatory Tracker	Filing type, patent expiry, Para IV status, filing stage per target market
4. Financial Summary	R&D investment, peak sales estimate, and auto-calculated ROI per product
Color key
Blue text — input cell (edit this)
Black text — formula (auto-calculates, don't overwrite)
Yellow fill — key assumption (e.g. discount rate)
Data sources used / recommended
Market size & growth: Mordor Intelligence, IMARC Group, TechSci Research, IBEF
Patent expiry & competition: FDA Orange Book, Drug Patent Watch, EMA patent register
R&D timelines: internal historical data where available, industry-standard ranges otherwise
Status
Currently populated with illustrative sample data (8 molecules) as a working template. Real-world data is being substituted in progressively — see Issues/TODO for candidates still being researched.
Tech 
Built with openpyxl; all scoring, tier, and ROI logic is formula-driven so the workbook recalculates live as inputs change.
