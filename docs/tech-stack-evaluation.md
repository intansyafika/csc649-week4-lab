# Tech Stack Evaluation

## Project
A Multi-Output Predictive System for Occlusal and Skeletal Pattern Classification

## Requirements that drive the decision
List 3 to 5 requirements from your own docs/requirements.md. Include at
least 2 non-functional requirements.
- [FR 1]:The system shall accept a lateral cephalometric radiograph (e.g. PNG/JPEG/DICOM) of  a patient aged 6–17 and preprocess it (resize, normalise) for the model.
- [FR 2]: The system shall automatically detect the key cephalometric landmarks (Sella, Nasion, A-point, B-point, Gonion, Menton) using heatmap regression and display them overlaid on the radiograph.
- [NFR 1]: The system shall process one radiograph and return landmarks, classifications and report within 5 seconds on a standard GPU/workstation.
- [NFR 2]: The system shall detect landmarks with a mean radial error of 2 mm or less, with at least 80% of landmarks falling within 2 mm of the expert annotation.

## Options
- Option A: [for example: static website (HTML and JavaScript) on GitHub Pages]
- Option B: [for example: Python web app (Flask) with a database on a cloud host]
- Option C: [Java web application developed using NetBeans IDE, with JSP, Servlets, and a database]

## Decision matrix
Weight: how important the criterion is for YOUR project (1 = low, 5 = high).
Score: how well each option does (1 = poor, 5 = excellent).
Weighted score = weight x score. Add them up for each option.

| Criterion                          | Weight | A score | B score | C score |
|------------------------------------|--------|---------|---------|---------|
| Fits my requirements               |    5   |     1   |    5    |     2   |
| Skills I already have              |    4   |     3   |    4    |     4   |
| Time to build before my deadline   |    5   |     3   |    4    |     2   |
| Free hosting and tools             |    3   |     5   |    4    |     4   |
| Performance and security needs     |    5   |     2   |    5    |     3   |
| Room to grow later                 |    4   |     2   |         |     3   |
| **Total (weighted)**               |        |     65  |   109   |    75   |

## Decision record
- **Context:** The project requires deep learning, radiograph processing, and multiple prediction outputs within limited time and budget.
- **Decision:** Choose Option B - Python web application using Flask
- **Reasons:** 
    1. Supports the functional requirements : can preprocess radiographs and perform heatmap-based landmark detection
    2. Allows future expansion: The system can later incorporate additional prediction outputs, report generation and a databse if required.
- **Consequences:** Esiear model integration and report generation, but requires effort to optimise performance and secure patient data.
- **Risks and next review:** The model may not meet the accuracy and processing-time targets. Review after developing the first prototype and testing its performance.
