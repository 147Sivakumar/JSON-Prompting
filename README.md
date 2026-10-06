# JSON Prompting for Tamil Visuals

## Assignment

**Learn • Build • Operate**

This project demonstrates how structured JSON prompting can be used to create culturally authentic Tamil-themed images and a short video.

## Objective

The goal is to build a reusable JSON prompt template where each visual decision is stored in a separate field.

This makes it possible to change one element while keeping the rest of the scene consistent.

## Cultural Theme

The visual concept is based on **Chettinad heritage in Tamil Nadu**.

The scene includes:

* Chettinad mansion architecture
* Nattukottai Chettiar heritage
* Kanchipuram silk sarees
* Traditional Tamil royal clothing
* Margazhi morning atmosphere
* Kolam
* Brass kuthuvilakku lamps
* Nadaswaram and thavil
* Traditional palace activities
* Tamil cultural details

The prompts avoid generic descriptions such as only "Indian" or "traditional" and instead use specific regional, architectural and cultural references.

## JSON Prompt Structure

The reusable template contains fields such as:

```json
{
  "subject": "...",
  "setting": {
    "place": "...",
    "era": "...",
    "time_of_day": "..."
  },
  "lighting": "...",
  "camera": {
    "shot": "...",
    "lens": "...",
    "angle": "..."
  },
  "palette": [
    "...",
    "...",
    "..."
  ],
  "style": "...",
  "aspect_ratio": "...",
  "avoid": [
    "...",
    "..."
  ]
}
```

## Controlled Prompt Experiments

### Image 1 — Base Template

The original JSON template is used without changing any fields.

**Purpose:** Establish the base visual scene.

### Image 2 — Time of Day

Only the `time_of_day` field is changed.

**Original:**
`early morning during Margazhi`

**Changed to:**
`golden hour before sunset`

**Purpose:** Observe how changing the time of day affects lighting and atmosphere while keeping the rest of the scene consistent.

### Image 3 — Camera Shot

Only the camera.shot field is changed.

### Original:
wide establishing shot

### Changed to:
close-up

Purpose: Observe how camera framing changes the visual composition while preserving the same characters, setting and style.

### Video

The video uses the same base JSON scene with an additional motion section.

The motion describes:

Subject movement
Environmental movement
Camera movement
Video duration

The goal is to preserve the same characters, architecture, costumes, lighting and visual identity while introducing natural movement.

### Why JSON Prompting?

JSON prompting provides:

Consistency — important scene details can remain fixed.
Control — individual fields can be changed independently.
Reusability — the same template can generate multiple variations.
Clarity — every visual decision has a defined location.
Experimentation — one field can be modified and its effect compared.
Maintainability — prompts are easier to update than large paragraphs.

### Learning Outcome

This project demonstrates that effective AI prompting is not only about writing detailed descriptions. It is also about structuring decisions, controlling variables, maintaining consistency, and using culturally specific visual information.

Authenticity lives in specifics: Chettinad architecture is not Thanjavur architecture, Kanchipuram silk is not a generic sari, and a Margazhi morning is not just any morning.
