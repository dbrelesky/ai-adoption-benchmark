# Benchmarking AI Adoption Across Teams

**Product Council | April 2026**

Session materials for the AI adoption benchmarking discussion.

## Live Scorecard

**[Take the AI Adoption Scorecard →](https://dbrelesky.github.io/ai-adoption-benchmark/poll/)**

Score your organization 1-5 on five dimensions: Engineering, Testing & QA, Consumer Insights, Talent & Readiness, and Governance & Scale. Room results aggregate in real-time so you can see the group average.

### Enable Live Room Results (2-minute setup)

The scorecard works for individual scoring out of the box. To enable **live room-wide results** (everyone sees the group average), you need a free Firebase Realtime Database:

1. Go to [console.firebase.google.com](https://console.firebase.google.com) and create a project (any name, e.g. "ai-scorecard")
2. Skip Google Analytics when prompted
3. Go to **Build → Realtime Database → Create Database** → choose any region → start in **Test mode**
4. Go to **Project Settings** (gear icon) → General → scroll to "Your apps" → click the **</>** web icon → register app (any nickname)
5. Copy the `firebaseConfig` object
6. Open `poll/index.html`, find the `FIREBASE_CONFIG` object near the top of the `<script>` block, and paste your config values

That's it. Every phone that opens the scorecard will now push scores to Firebase and the **Room** tab will show live averages.

> **Tip:** Change the `SESSION_ID` constant in the script for each meeting to start fresh results.

## Session Materials

| File | Description |
|------|-------------|
| [Slide Deck](docs/AI_Adoption_Benchmarks.pptx) | 7-slide presentation (Modern Minimalist theme) |
| [Reference Document](docs/AI_Adoption_Benchmarks_Reference.docx) | Full data leave-behind with all benchmarks and sources |
| [Presenter Script](docs/Presenter_Script.md) | Slide-by-slide run of show with timing and facilitation notes |

## Key Benchmarks

- **22%** of merged code is AI-authored (DX Q4 2025, 135K+ devs)
- **88%** of organizations use AI in at least one function
- **40%** of enterprise apps will have AI agents by EOY 2026 (Gartner)
- **20%** of organizations say their talent is AI-ready (Deloitte 2026)

## The Framework

Five dimensions, scored 1-5, assessed quarterly:

| Dimension | Weight |
|-----------|--------|
| Code & Delivery | 25% |
| Quality & Testing | 20% |
| Consumer Intelligence | 20% |
| Talent & Culture | 20% |
| Governance & Scale | 15% |

## Sources

- Deloitte, State of AI in the Enterprise 2026
- DX, Developer Impact Report Q4 2025
- Gartner, Enterprise AI Agent Predictions 2026
- World Quality Report 2025-26
- Worklytics, 2025 AI Adoption Benchmarks
