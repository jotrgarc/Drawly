Product Requirements Document (PRD) – Drawly
1. Overview

Product Name: Drawly
Description: Drawly is an AI-powered art app that transforms photos into step-by-step drawing tutorials using the Loomis method (breaking down objects into simple shapes and forms). It helps artists of all skill levels practice structure, proportions, and form by learning how to see the world in shapes.

Problem Statement:
Many aspiring artists struggle to bridge the gap between real-life references and simplified drawings. Traditional tutorials are static and one-size-fits-all, while artists need dynamic, personalized guides that adapt to what they want to draw.

Solution:
Drawly uses AI to automatically process a photo, reduce it to Loomis-style construction shapes, and generate a progressive tutorial sequence that teaches artists how to build a drawing from the ground up.

2. Goals & Success Metrics

Goals:

Provide an intuitive AI-powered tool for artists to learn drawing fundamentals.

Enable users to turn any photo into a structured, step-by-step tutorial.

Encourage daily practice and skill improvement through guided breakdowns.

Success Metrics:

Engagement → % of users who generate more than 5 tutorials.

Retention → % of users who return weekly to practice.

Accuracy → % of AI outputs that match Loomis guidelines.

User satisfaction → Avg. rating from feedback surveys.

3. Target Users

Beginner Artists → learning proportions, structure, and how to simplify objects.

Intermediate Artists → refining construction methods and practicing daily.

Educators → art teachers using Drawly as a teaching assistant.

4. Features
Core Features (MVP)

Photo Upload → Users upload or take a picture.

AI Shape Breakdown → AI converts image into simplified Loomis-style shapes (spheres, cylinders, boxes, etc.).

Step-by-Step Tutorial Generation → Output multiple tutorial stages (basic forms → refined sketch → details).

Download & Share → Save tutorials as images or PDFs.

Basic User Interface → Clean web/app interface to manage uploads and results.

Future Features (Post-MVP)

Skill Levels → Beginner (very simplified), Intermediate (medium detail), Advanced (subtle corrections).

Interactive Mode → Users can sketch alongside the tutorial in-app.

Community Gallery → Share tutorials and drawings.

Mobile App Integration → iOS/Android for portability.

5. User Flow

User opens Drawly.

Uploads/takes a photo.

AI processes → generates shape breakdown.

Tutorial is displayed as sequential steps.

User saves, practices, or shares tutorial.

6. Technical Requirements

Frontend: React (Next.js) for web app.

Backend: Python (FastAPI/Flask) for AI processing.

AI/ML: Computer Vision + Drawing Decomposition (OpenCV, PyTorch, or TensorFlow).

Storage: AWS S3 / Firebase for storing photos + tutorials.

Authentication (optional): OAuth or Firebase Auth for user accounts.

7. Open Questions

Should Drawly focus strictly on Loomis heads at first, or support any object?

Will it be free to use, freemium (basic free, advanced paid), or education-licensed?

Should we include gamified practice streaks to encourage retention?
