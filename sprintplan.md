# Sprint Plan – Drawly

This document outlines the sprint goals, tasks, and deliverables for building the Drawly MVP.

---

## Sprint 1 (Weeks 1–2): Foundations & Image Processing

### Goals
- Set up repository structure and development environment.
- Enable basic photo upload and storage.
- Implement initial AI image processing (edge detection + simple shape recognition).
- Define tutorial data pipeline (ImageInput → Tutorial → Steps → Shapes).

### Tasks
- [ ] Initialize repo with README, PRD, DataModel.
- [ ] Add `.gitignore` (Python + Node).
- [ ] Set up backend (Python FastAPI).
- [ ] Set up frontend (Next.js with drag & drop upload).
- [ ] Implement image upload endpoint.
- [ ] Store images in local/temporary storage (later S3/Firebase).
- [ ] Build simple AI pipeline (OpenCV: grayscale, edge detection, contour → circle/box approximation).
- [ ] Generate dummy tutorial JSON (using DataModel).

### Deliverables
- User can upload an image and receive a JSON tutorial structure with placeholder steps/shapes.
- Basic UI with file upload box + output preview (JSON/text).
- Repo organized with clear documentation.

---

## Sprint 2 (Weeks 3–4): Tutorial Generation & Export

### Goals
- Turn AI shape breakdown into sequential steps.
- Display steps visually with overlays.
- Support export as PNG/PDF.
- Add basic styling for frontend.

### Tasks
- [ ] Implement `Step` sequence generation (at least 3 steps: forms → construction → refine).
- [ ] Render overlay images for each step.
- [ ] Connect backend to frontend (fetch tutorial + steps).
- [ ] Add step viewer in frontend (prev/next buttons).
- [ ] Implement export endpoint (generate PNG/PDF).
- [ ] Style UI for minimal but clean experience (light/dark theme).

### Deliverables
- User uploads a photo → sees step-by-step Loomis tutorial in the UI.
- User can export tutorial as PNG or PDF.
- Core MVP loop complete.

---

## Future Sprint Ideas (Post-MVP)

- **Sprint 3:** Skill levels (beginner vs advanced breakdowns).  
- **Sprint 4:** User accounts + saving past tutorials.  
- **Sprint 5:** Interactive sketch-along canvas.  
- **Sprint 6:** Mobile app version.  

---
