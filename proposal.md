# LOL Pro Play Drafting Tool Proposal  
*An MVP for Data-Driven Champion Drafting in Professional League of Legends*

**Prepared by:** Hsiang-I, Lung  
**Date:** 2025/2/21

---

## Table of Contents
1. [Executive Summary](#executive-summary)
2. [Problem Statement](#problem-statement)
3. [Project Objectives](#project-objectives)
4. [Methodology: The PACE Workflow](#methodology-the-pace-workflow)
   - [4.1 Plan](#41-plan)
   - [4.2 Analyze](#42-analyze)
   - [4.3 Construct](#43-construct)
   - [4.4 Execute](#44-execute)
5. [Timeline & Milestones](#timeline--milestones)
6. [Risks & Mitigations](#risks--mitigations)
7. [Team & Responsibilities](#team--responsibilities)
8. [Conclusion & Next Steps](#conclusion--next-steps)

---

## Executive Summary
The **LOL Pro Play Drafting Tool** is designed to assist professional League of Legends teams in making optimal champion drafting decisions. Leveraging historical match data, solo queue statistics, and patch notes—complemented by lightweight NLP techniques—the tool generates actionable draft recommendations in real time. This proposal outlines an MVP approach using the PACE workflow, ensuring a focused project that is both achievable and impactful.

---

## Problem Statement
In professional League of Legends, the drafting phase is high-stakes and fast-paced. Teams must quickly adapt to evolving metas driven by frequent patch updates, often relying on subjective insights or incomplete data. There is a clear need for a data-driven solution that:
- **Integrates quantitative match statistics with qualitative patch note information.**
- **Provides real-time recommendations reflecting both team synergy and changing champion strengths.**
- **Delivers interpretable insights to support swift and confident decision-making.**

---

## Project Objectives
- **Develop an MVP:** Deliver a working prototype demonstrating core functionalities such as synergy analysis and basic patch impact parsing.
- **Integrate Diverse Data Sources:** Combine pro match data, solo queue performance, and historical patch notes into a unified analytical framework.
- **Implement Predictive Modeling:** Train a model to forecast champion viability post-patch using efficient NLP methods.
- **Create an Interactive UI:** Build a simple web dashboard that displays recommendations and key metrics.
- **Demonstrate Data-Driven Decision-Making:** Highlight how this tool can enhance strategic drafting and offer a competitive edge.
- **Future Expansion:** Within nine months, reach out to DPM.lol to transition the MVP into a production-ready tool. The expanded version will target both professional teams and casual players, broadening the tool’s applicability.

---

## Methodology: The PACE Workflow

### 4.1 Plan
- **Define Scope:**
  - Limit initial data collection to one pro league (e.g., a Major Region) and focus on the most recent 5–10 patches.
  - Prioritize core features: synergy scoring, basic matchup analysis, and keyword-based patch note impact evaluation.
- **Set Objectives:**
  - Deliver a functional MVP that demonstrates the concept.
  - Ensure the project remains manageable as a solo effort with clear deliverables.
- **Resources & Tools:**
  - **Data Sources:** Leaguepedia, Riot API (or OP.GG and other approved databases), and public patch note archives.
  - **Tools:** Python (scikit-learn, TensorFlow/PyTorch), NLP libraries (NLTK, spaCy), and a lightweight web framework (Streamlit or Flask).

### 4.2 Analyze
- **Data Requirements:**
  - Gather historical pro match data, solo queue statistics, and patch note text.
  - Identify key variables such as win rates, champion pairings, and buff/nerf keywords.
- **Feasibility:**
  - Evaluate open-source libraries to accelerate development.
  - Prioritize robust data cleaning and preprocessing to ensure model accuracy.
- **Risk Assessment:**
  - Address potential issues like data quality and rapid meta shifts.
  - Plan automated cleaning procedures and periodic model updates.

### 4.3 Construct
- **Implementation Phases:**
  1. **Data Pipeline:** Set up processes for data ingestion and cleaning.
  2. **Model Development:**
     - Build a basic synergy model (e.g., logistic regression or a small neural network).
     - Integrate keyword extraction from patch notes to adjust champion ratings.
  3. **UI Development:**
     - Develop a basic dashboard for inputting draft scenarios and displaying recommendations.
  4. **Iteration:**
     - Gather feedback and refine the model and interface accordingly.
- **Documentation:**
  - Maintain thorough documentation of code, data sources, and design decisions.
  - Keep a progress log to track development and support future enhancements.

### 4.4 Execute
- **Deployment:**
  - Roll out the MVP as a local web application for demonstration.
  - Test with real draft scenarios and iterate based on performance.
- **Evaluation:**
  - Monitor key metrics such as model accuracy and recommendation quality.
  - Refine the tool continuously through user feedback and performance analysis.
- **Presentation:**
  - Prepare a final slide deck and demo video that highlight both technical innovation and strategic value.
  - Articulate the tool’s competitive advantages and efficiency improvements.

---

## Timeline & Milestones

**Month 1:**
- Project setup, data source identification, and initial data collection.

**Month 2:**
- Exploratory Data Analysis (EDA) and prototype synergy model development.

**Month 3:**
- Develop keyword extraction for patch notes and assign severity scores.

**Month 4:**
- Integrate patch impact data with the synergy model and perform validation.

**Month 5:**
- Develop the initial web dashboard interface and integrate model outputs.

**Month 6:**
- Refine model performance, incorporate user inputs, and improve UI functionality.

**Month 7:**
- Conduct testing with real draft scenarios, document findings.

**Month 8:**
- Finalize documentation, polish presentation materials, and prepare for a comprehensive project review.

**Month 9:**
- **Expansion Phase:** Begin outreach to DPM.lol and initiate efforts to transform the MVP into a production-ready tool that serves both pro play and casual players.

**Month 10 and Beyond:**
- Transition to production:
  - Enhance the data pipeline for real-time data ingestion and continuous updates.
  - Scale the model to handle broader datasets and more complex draft scenarios.
  - Improve the UI for usability and responsiveness in live settings.
  - Pilot the tool with both professional teams and casual player groups.
  - Implement robust error handling, monitoring, and user support systems.

---

## Risks & Mitigations
- **Data Inconsistency:**
  - *Risk:* Incomplete or noisy match/patch data.
  - *Mitigation:* Implement robust data cleaning and normalization procedures.
- **Rapid Meta Changes:**
  - *Risk:* Frequent game updates may quickly outdate the model.
  - *Mitigation:* Design the system for periodic retraining and integrate a feedback loop.
- **Technical Complexity:**
  - *Risk:* Balancing model sophistication with development time constraints.
  - *Mitigation:* Start with simple models and iteratively add complexity only if feasible.

---

## Team & Responsibilities

**Project Lead (Hsiang-I, Lung):**  
- Oversee technical development, including data pipeline, predictive modeling, and NLP integration.  
- Ensure system architecture supports scalability and model accuracy.

**Business & User Experience Lead (Chen-Wei, Guo):**  
- Coordinate stakeholder engagement, gather feedback from teams and users (both pro and casual).  
- Oversee quality assurance, user testing, and the development of an intuitive UI/dashboard.  
- Manage project documentation, communication with non-technical stakeholders, and ensure milestones are met.

---

## Conclusion & Next Steps
The **LOL Pro Play Drafting Tool** aims to revolutionize champion drafting in professional League of Legends by delivering real-time, data-driven recommendations. With our MVP, we will validate the concept using historical data and initial testing. Importantly, after the first eight months we plan to pivot—around Month 9—to extend our solution by reaching out to DPM.lol. The goal is to evolve the MVP into a production-ready tool that not only supports pro play but is also adapted for casual players, significantly broadening its impact.

**Next Steps:**
- Finalize data sources and refine the project scope.
- Set up the development environment and version control.
- Begin data collection and early model prototyping.
- Transition from MVP to a scalable solution through outreach (e.g., with DPM.lol) and iterative enhancements.
- Prepare a comprehensive project review and demo to showcase the tool's potential.

---

