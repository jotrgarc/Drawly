# Backlog – Drawly

This backlog outlines high-level epics, user stories, and development tasks for the Drawly MVP and beyond.

---

## Epic 1: Image Processing
**Goal:** Allow users to upload images and generate Loomis-style breakdowns.

### User Stories
- [ ] As a user, I can upload a photo so the system can process it.
- [ ] As a system, I can detect forms (circle, box, line) from the image.
- [ ] As a user, I get feedback if the image cannot be processed.

### Tasks
- [ ] Backend: Set up FastAPI with upload endpoint.
- [ ] Storage: Save images locally (later S3/Firebase).
- [ ] AI: Implement OpenCV edge detection + contour simplification.
- [ ] Return dummy JSON in Tutorial format.

---

## Epic 2: Tutorial Generation
**Goal:** Convert processed image into step-by-step Loomis tutorials.

### User Stories
- [ ] As a user, I receive a sequence of steps to build my drawing.
- [ ] As a user, I can see shapes added step-by-step.
- [ ] As a user, I can view a simple caption alongside each step.

### Tasks
- [ ] Define tutorial step logic (forms → construction → refine).
- [ ] Implement JSON output for steps/shapes.
- [ ] Generate overlay images for each step.
- [ ] Add captions for teaching guidance.

---

## Epic 3: Frontend Experience
**Goal:** Provide a clean and simple UI for artists.

### User Stories
- [ ] As a user, I can drag & drop a photo to upload.
- [ ] As a user, I can view generated tutorial steps.
- [ ] As a user, I can switch between light/dark mode.

### Tasks
- [ ] Set up Next.js frontend.
- [ ] Build upload form with drag & drop.
- [ ] Display tutorial JSON in UI (debug mode).
- [ ] Create step viewer with prev/next navigation.
- [ ] Add minimal styling (artist-friendly).

---

## Epic 4: Export & Sharing
**Goal:** Let users save and share tutorials.

### User Stories
- [ ] As a user, I can export my tutorial as PNG/PDF.
- [ ] As a user, I can share my tutorial with others.

### Tasks
- [ ] Backend: Implement export service (PDF/PNG).
- [ ] UI: Add "Export" button.
- [ ] Save exported files in storage with links.

---

## Epic 5: Future Enhancements
**Goal:** Expand Drawly beyond MVP.

### Ideas
- [ ] Skill levels (beginner → advanced).
- [ ] User accounts + history of past tutorials.
- [ ] Interactive sketch-along canvas.
- [ ] Community gallery to share tutorials.
- [ ] Mobile app version (iOS/Android).
