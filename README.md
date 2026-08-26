# TomatoGuard AI — Frontend v5

## Important design rule
This version does **not** invent crop-health, soil, disease or weather values.

When backend/model services are unavailable:
- Dashboard shows `Not analyzed`, `Not synced`, or `Integration pending`.
- Disease page accepts a suitable leaf image, but does not invent a disease name/confidence.
- Soil page performs OCR + questionnaire collection, but does not invent fertility classes or fertilizer doses.
- Weather page shows no fake weather values.
- Reports include only results that actually exist.

## API integration
Copy `.env.example` to `.env` when your team gives you endpoints:

```env
VITE_DISEASE_API_URL=http://localhost:8000/api/disease
VITE_SOIL_API_URL=http://localhost:8000/api/soil
VITE_WEATHER_API_URL=http://localhost:8000/api/weather
```

Restart Vite after editing `.env`.

### Expected disease request
`POST multipart/form-data`, field: `image`

The UI can read common response keys such as:
```json
{
  "label": "Early Blight",
  "confidence": 0.94,
  "recommendation": "..."
}
```

### Expected soil request
`POST application/json` with:
- `soil_values`
- `questionnaire`
- `ocr_text`

### Weather request
Frontend calls:
`GET <VITE_WEATHER_API_URL>?location=<location>`

The weather page currently displays the raw backend response until your team's final response schema is agreed.

## Working frontend features
- Landing page
- Register/login/logout (localStorage demo auth)
- Profile photo upload
- Light/dark theme
- Working notification dropdown
- Daily task tracker
- Leaf image pre-check + remove/reset
- Soil-report OCR + report validation + remove/reset
- Soil questionnaire
- Government scheme links
- Reports based only on available data

## Run
```bash
npm install
npm run dev
```
