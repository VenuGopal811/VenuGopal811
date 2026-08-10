# How to Deploy This Rebuild

## 1. Replace the repo contents

Push this folder's contents to `VenuGopal811/VenuGopal811` on the `main` branch, overwriting
the current README.md.

## 2. Enable the GitHub Activity feed

1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate a token with `repo` scope
3. In this repo: Settings → Secrets and variables → Actions → add secret `GH_TOKEN`
4. Trigger `update-gh-activity` manually once (Actions tab → Run workflow) to confirm it fills
   the `<!--START_SECTION:activity-->` block

## 3. WakaTime stats (optional, delete if unused)

Only keep this if you track coding time with WakaTime.

1. Sign up at wakatime.com, install the editor plugin
2. Copy your API key from wakatime.com/settings/api-key
3. Add secret `WAKATIME_API_KEY`
4. If not using it, delete `.github/workflows/update-timestats.yml` and the
   `<!--START_SECTION:waka-->` block from README.md

## 4. What changed from the old version

- Fixed both project links, which previously pointed at your profile root instead of the
  actual repos
- Swapped TensorFlow/PyTorch out of the stack table for LangGraph, LangChain, and FastAPI —
  what you actually build with
- Added GLA University, Droid Club (Treasurer & Lead Organizer), and your Azure certs, none
  of which were in the old version
- Replaced ContentOS (an early/foundational project) with SpendOS and the WhatsApp
  Notification Router, your more current work; LabelSense is intentionally left out
- Added the GitHub Activity workflow so the "Recent Activity" section is no longer static
- Added github-readme-stats and streak-stats cards alongside the existing activity graph

## 5. Repo settings

Add a one-line description and a few topics (`agentic-ai`, `langgraph`, `github-profile`) in
the repo's About panel — it currently shows "No description, website, or topics provided."
