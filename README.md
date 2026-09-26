# DS_6021_Final_Project
Work Related to Intro to Predictive Modeling Machine Learning Final Group Project

# DS 6021 Final Project — Team Roadmap

**Course:** DS 6021 – Introduction to Predictive Modeling
**Final Deliverable Due:** Sunday, 12/6/2026, 11:59 PM (Canvas)
**Presentation Date:** 12/7/2026

## Team
| Name | Role(s) | GitHub Handle |
|------|---------|----------------|
| | | |
| | | |
| | | |
| | | |

---

## Milestone 1 — Team Formation (Due: Week 3, 9/7–9/11)
- [ ] Finalize team of 3–4 members
- [ ] Exchange contact info (email, phone, Slack/Discord) and agree on a primary communication channel
- [ ] Set up shared GitHub repository; add all members as collaborators
- [ ] Create repo structure: `/data/raw`, `/data/cleaned`, `/notebooks`, `/app`, `/docs`, `/slides`
- [ ] Add a `.gitignore` (exclude large data files, `.env`, virtual environments)
- [ ] Schedule a recurring weekly team check-in time

---

## Milestone 2 — Problem & Dataset Selection (Due: Week 5, 9/21–9/25)
- [ ] Brainstorm 3–5 candidate business problems or research questions
- [ ] For each candidate, identify: who cares about the answer, what decision it informs, and why ML (not just reporting) is needed
- [ ] Vote/decide on final problem statement as a team
- [ ] Write a 1-paragraph problem statement documenting the "why"
- [ ] Identify candidate data source(s); confirm each has:
  - [ ] At least 4 numeric variables (across combined sources if needed)
  - [ ] At least 4 categorical variables
  - [ ] Sufficient rows for modeling (no strict minimum, but flag if under ~500)
- [ ] Confirm data is legally/ethically usable (license, terms of use, no PII issues)
- [ ] Download/pull a sample of the data and sanity-check it opens correctly
- [ ] Document data source(s), access method (download/API/scrape), and rationale in `/docs/data_sources.md`
- [ ] If using an API or scraping, write and test a minimal script to pull the raw data

---

## Milestone 3 — Data Cleaning & Exploration (Due: Week 8, 10/12–10/16)
- [ ] Load raw data into a notebook; save an untouched copy to `/data/raw`
- [ ] Inventory each column: type, meaning, % missing, unique values
- [ ] Handle missing data (drop, impute, flag) — document reasoning for each decision
- [ ] Standardize column names (consistent casing, no spaces)
- [ ] Remove duplicate rows/irrelevant columns
- [ ] Check and fix data types (dates as datetime, categories as category, etc.)
- [ ] Detect and address outliers/invalid values (e.g., negative ages)
- [ ] Engineer at least 1–2 new features relevant to your problem statement
- [ ] If combining multiple datasets, perform and validate the join/merge (check row counts before/after)
- [ ] Save cleaned dataset to `/data/cleaned`; save the cleaning script/notebook to `/notebooks`
- [ ] Generate summary statistics (`.describe()`, value counts for categoricals)
- [ ] Build 4–6 exploratory visualizations tied to specific questions (not just "because you can")
- [ ] Write 2–3 sentence takeaways under each visualization
- [ ] Team check-in: does the cleaned data actually support your problem statement? Adjust if not

---

## Milestone 4 — First Model Attempt (Due: Week 10, 10/26–10/30)
- [ ] Define target variable and confirm problem type (regression vs. classification)
- [ ] Split data into train/test (and validation if needed)
- [ ] Build a baseline model (e.g., linear regression or logistic regression)
- [ ] Evaluate baseline with appropriate metrics (RMSE/R² for regression; accuracy/precision/recall/F1/ROC-AUC for classification)
- [ ] Document baseline results in `/notebooks` with clear markdown commentary
- [ ] Identify obvious next steps (feature scaling, encoding categoricals, addressing class imbalance, etc.)
- [ ] Team check-in: review midterm material against your model-building process

---

## Milestone 5 — Second Modeling Technique + App Scaffolding (Due: Week 12, 11/9–11/13)
- [ ] Implement a second, appropriately-chosen modeling technique (e.g., KNN, classification/regression tree, GLM variant)
- [ ] Track and compare experiments (model type, hyperparameters, metrics) in a simple table or experiment log
- [ ] Select/justify a "best model so far" with clear reasoning
- [ ] Choose an app framework (Streamlit, Dash, Flask, or FastAPI)
- [ ] Set up minimal app skeleton: loads model + cleaned data, single input → prediction output
- [ ] Deploy a "hello world" version of the app publicly (e.g., Streamlit Community Cloud, Render, Heroku) to confirm deployment works early
- [ ] Assign app ownership/roles among team members

---

## Milestone 6 — Unsupervised Learning Plan (Due: Week 13, 11/16–11/20)
- [ ] Decide where unsupervised learning fits (e.g., PCA for dimensionality reduction pre-modeling, k-means for customer/observation segmentation)
- [ ] Implement chosen technique(s) and evaluate (e.g., explained variance for PCA, silhouette score/elbow method for k-means)
- [ ] If a technique doesn't improve results, document what was tried and why it was rejected (required either way — no penalty for trying and explaining)
- [ ] Incorporate any useful unsupervised results back into the supervised modeling pipeline or app

---

## Milestone 7 — Model Finalization (Target: Week 14, 11/23–11/27)
- [ ] Finalize best model(s) per problem type; re-validate on test set
- [ ] Clean up and comment all modeling code for reproducibility
- [ ] Write a model summary: what was tried, what worked, what didn't, and why
- [ ] Confirm classification/regression choice matches problem type throughout (no misapplied linear regression on classification, etc.)
- [ ] Integrate final model into the app (replace placeholder from Milestone 5)

---

## Milestone 8 — App Completion (Target: Week 14–15, 11/23–12/4)
- [ ] Build out full interactivity (user inputs → live predictions, filters, visualizations)
- [ ] Add explanatory text/labels so a non-technical user understands what they're seeing
- [ ] Test app end-to-end on a fresh machine/browser (not just localhost)
- [ ] Confirm public deployment is stable and accessible via a shareable link
- [ ] Add app link to repo README

---

## Milestone 9 — Presentation Build (Target: Week 15, 11/30–12/4)
- [ ] Draft slide outline (8–10 slides total):
  1. Title slide — project title, group number, members (alphabetical by last name)
  2. Executive summary — problem, impact, key results only
  3. Problem & motivation
  4. Data source(s) & key EDA visuals
  5. Cleaning/feature engineering highlights
  6. Modeling approach(es) & comparison
  7. Unsupervised learning results
  8. App demo (live or screen-recorded backup)
  9. Conclusions & insights
  10. (Optional) Limitations & future work
- [ ] Build slides (PowerPoint or Google Slides), export as PDF/HTML for submission
- [ ] Assign speaking sections to each team member
- [ ] Record a backup screen capture of the app demo in case of live-demo issues
- [ ] Full team run-through, timed — target ≤ 9 minutes talk + 3 min Q&A buffer (12 min total)
- [ ] Revise for clarity and visual clutter (no walls of text)

---

## Milestone 10 — Final Packaging & Submission (Due: 12/6/2026, 11:59 PM)
- [ ] Finalize GitHub repo: all code committed, well-commented, with a top-level README explaining how to run everything
- [ ] Confirm raw + cleaned datasets are in the repo (or linked via S3 if too large)
- [ ] Confirm app is deployed and link works from a clean browser session
- [ ] Write Generative AI usage document (`/docs/genai_usage.md`) covering:
  - [ ] How AI was used (which tasks, which tools)
  - [ ] Flag any AI-generated code in the repo (comments or README note)
  - [ ] Description of how AI-generated code was tested/validated
  - [ ] Include any `CLAUDE.md` or Claude Skills used, or link to where they're defined
  - [ ] Versioned prompt log, if applicable
- [ ] Export final presentation as PDF/HTML
- [ ] Submit to Canvas: slides, dataset(s), GitHub link, app link, GenAI usage doc
- [ ] Do a final team check: does everything on this list have an owner and a ✅?

---

## Notes
- Data cleaning/exploration is iterative — expect to revisit Milestone 3 steps throughout modeling.
- If a modeling/dimensionality-reduction technique doesn't help, document the attempt and reasoning rather than omitting it — this avoids losing points.
- Start app deployment early (Milestone 5); last-minute deployment issues are avoidable.
