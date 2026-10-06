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

### Image 3 — Cam
