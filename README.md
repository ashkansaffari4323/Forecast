# Forecast Retention Vercel Ready

This version implements the requested retention/payment application workflow.

## Updates included

- Reads payment applications and payment items per project/contract.
- Extracts retention held, retention released, retention net and net actual by month when fields are available in ACC responses.
- Keeps actuals separate from forecast.
- Adds Contract Detail search bar.
- Improves supplier name matching using company maps and multiple contract/vendor/supplier fields.
- Adds View Allocation retention table by month.
- Adds Reduce retention / Add retention back toggle per contract/month.
- Reduces forecast cashflow for that month only when the toggle is active.
- Keeps Programs workflow with XML/XER upload, 5 saved programs and up to 10 contracts per milestone.
- Vercel-ready: vercel.json, api/index.ts and exported Express app included.

## Deploy

```powershell
git add -A
git commit -m "Add retention payment applications workflow"
git push
```

Then in Vercel: Redeploy > Clear Build Cache and Redeploy.

## Vercel settings

- Framework Preset: Other
- Install Command: npm install
- Build Command: npm run build
- Output Directory: client/dist
