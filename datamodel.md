# Data Model – Drawly

AI turns photos into step-by-step Loomis tutorials (forms → construction → line).

---

## Diagram
```mermaid
erDiagram
  IMAGE_INPUT ||--|| TUTORIAL : generates
  TUTORIAL ||--o{ STEP : contains
  STEP ||--o{ SHAPE : composes
  TUTORIAL ||--o{ EXPORT : produces
{
  "image_id": "uuid",
  "file_url": "https://cdn.drawly.app/u/abc.jpg",
  "uploaded_at": "2025-08-24T17:00:00Z",
  "status": "processed",
  "width": 2048,
  "height": 1365
}
{
  "tutorial_id": "uuid",
  "image_id": "uuid",
  "title": "Portrait – 3/4 View",
  "style": "loomis",
  "level": "beginner",
  "created_at": "2025-08-24T17:02:00Z",
  "steps": [ /* see Step */ ]
}
{
  "step_id": "uuid",
  "tutorial_id": "uuid",
  "step_number": 1,
  "caption": "Start with a circle for the cranium.",
  "overlay_url": "https://cdn.drawly.app/tuts/123/step1.png",
  "render_mode": "forms",
  "shapes": [ /* see Shape */ ]
}
{
  "shape_id": "uuid",
  "step_id": "uuid",
  "type": "circle | line | box | cylinder | sphere",
  "x": 420,
  "y": 360,
  "params": {
    "radius": 180,
    "guide_role": "cranium"
  },
  "confidence": 0.95
}
{
  "export_id": "uuid",
  "tutorial_id": "uuid",
  "format": "png | pdf",
  "file_url": "https://cdn.drawly.app/tuts/123/tutorial.pdf",
  "created_at": "2025-08-24T17:05:00Z"
}
