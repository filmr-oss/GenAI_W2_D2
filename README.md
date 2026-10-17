# Tamil Culture — JSON Prompting

## Week 2 Day 2 Assignment

### Use JSON Prompting for Tamil Visuals

This project demonstrates the use of a reusable JSON prompt template to generate culturally specific Tamil visuals.

The same prompt structure was used to create three images and a short video, while changing selected parameters to observe their effect on the generated visuals.

---

## Objective

The goal of this assignment is to:

- Create a reusable JSON prompt template.
- Generate culturally authentic Tamil visuals.
- Keep the main prompt consistent across generations.
- Change only selected fields between images.
- Extend the same JSON structure for video generation.

---

## Cultural Concept

The visual concept is based on:

**Ancient Tamil agricultural life during the Chola period.**

The scene shows an ancient Tamil farmer working with two bullocks in a paddy field, accompanied by his wife carrying harvested grain.

The setting represents rural Tamil Nadu agricultural life with traditional clothing, farming practices, and a historical village environment.

---

## JSON Prompt Template

The reusable prompt is stored in:

`tamil_prompt.json`

The template contains:

- `subject`
- `setting`
  - `place`
  - `era`
  - `time_of_day`
- `lighting`
- `camera`
  - `shot`
  - `lens`
  - `angle`
- `palette`
- `style`
- `aspect_ratio`
- `avoid`

---

## Image 1 — Base Image

The first image was generated using the original JSON template.

### Field Changed

**None**

This image acts as the base visual for comparison with the other generations.

---

## Image 2 — Time of Day Variation

The second image uses the same JSON prompt while changing only the time of day.

### Field Changed

`setting.time_of_day`

### Change

**Early morning → Sunset / Golden hour**

All other major prompt parameters were kept consistent.

This demonstrates how changing the time of day affects the lighting and atmosphere of the scene.

---

## Image 3 — Camera Shot Variation

The third image uses the same prompt while changing only the camera shot.

### Field Changed

`camera.shot`

### Change

**Wide cinematic establishing shot → Close-up**

The subject, setting, historical period, style, and other parameters remain consistent.

This demonstrates how changing the camera shot changes the visual framing and emphasis.

---

## Video

The same JSON template was extended for video generation by adding motion parameters.

Example:

```json
{
  "motion": {
    "subject_motion": "Natural farming movements and subtle movement of the bullocks",
    "camera_move": "Slow cinematic push-in",
    "duration_seconds": 5
  }
}
