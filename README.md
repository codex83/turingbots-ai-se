
# Will TuringBots Replace Human Software Developers?  
*A Big Data Analysis of Trends in Open Source Coding, Automation, and AI*

**By Hritik Jhaveri | Big Data and Cloud Computing**

---

## Overview

This project investigates whether AI-powered development tools—so-called “TuringBots”—are poised to replace human software developers. By mining trends from the GitHub Archive (over 1.36 TiB of commits and repository data), we analyze shifts in programming language usage, license adoption, automation, and the real impact of AI tools on the software development landscape.

---

## Key Findings

- **AI-assisted coding is on the rise:** Automated commits are more frequent due to the rise of TuringBots and similar tools.
- **Programming language trends:** Python dominates AI/ML, while JavaScript is the most broadly active language overall.
- **Humans remain essential:** While AI can automate repetitive tasks, human developers are still needed for high-level architecture, debugging, and innovation.
- **Big Tech’s role:** Companies like Google and Linux exert significant influence through open-source contributions.
- **Automation & repetition:** Many commits, especially in front-end projects, are repetitive or templated, underscoring dependence on frameworks, templates, and bots.

---

## Data Sources & Methodology

### Data Sources
- **Primary:** GitHub Archive (Google Cloud Storage), over 1.36 TiB.
- **Data Includes:**  
  - Commit metadata (authors, timestamps, messages)
  - Programming language usage per repo
  - Repo license info
  - File metadata and actual file contents

### Data Preparation
- Removed duplicate and incomplete records
- Standardized text (e.g., commit messages)
- Extensive cleaning: only well-populated, relevant fields retained

### Technologies Used
- **Processing:** Apache Spark (large-scale data manipulation)
- **EDA/Visualizations:** Python (Matplotlib, Pandas)

### Analytical Methods
- **Exploratory Data Analysis (EDA):** Examined key variables and distributions
- **Temporal Analysis:** Trends in code commits, languages, and AI associations over time
- **Text Analysis:** Checked for commit message uniqueness and frequency of automation (bots vs humans)

---

## Main Results

- **Popular Programming Languages:**  
  - By bytes: C; by repo count: JavaScript.
  - Post-2010s: JavaScript and HTML uproar due to mobile/web/cloud boom.
  - Python is the clear leader in AI/ML work.

- **Open Source Licenses:**  
  - MIT is the most widely-used license.
  - GPL-3.0 gathers the widest spread of programming languages.

- **AI/Data Science in Practice:**  
  - Most associated keywords: `numpy`, `tensorflow`, `pandas`.
  - Python-centric tools dominate, reflecting broader trends in DS/AI.

- **Bot Automation & Commit Patterns:**  
  - Automated accounts (e.g., GitHub bots, CI/CD agents) are now among the top committers.
  - Commit messages in front-end (JS/HTML) projects especially repetitive; Python sees more unique message content.

---

## Conclusions & Recommendations

- **TuringBots and AI tools will *not* fully replace human developers.** They automate repetitive tasks, but humans remain indispensable for creative problem-solving and architectural thinking.
- **Actionable Steps:**
  - Adopt AI coding tools to maximize efficiency—especially for routine coding tasks.
  - Invest in upskilling teams to work seamlessly with AI.
  - Closely monitor which development tasks can be reliably automated, without sacrificing software quality.
  - Contribute to open-source AI initiatives and use Python for ML projects.
- **Future Outlook:**  
  Collaboration will define future software engineering: AI handles the rote work; humans lead on innovation and complex decisions.

---

## Project Structure

```
.
├── data_preprocessing/     # Data cleaning scripts (Spark, Python)
├── analysis/               # EDA, Text/Temporal analysis
├── visualizations/         # Charts/plots showing trends (Matplotlib, Pandas)
├── results/                # Summaries, tables, and extracted insights
├── README.md
└── Final-Presentation-Hritik-Jhaveri.pptx
```

---

## Acknowledgments

Many thanks to open-source communities and researchers whose tools and data made this project possible.
