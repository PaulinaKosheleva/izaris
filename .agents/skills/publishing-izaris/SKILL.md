---
name: publishing-izaris
description: Use when updating or publishing the IZARIS planner on GitHub and Netlify, especially when multiple edits need one publication decision.
---

# Publish IZARIS as one batch

Target: PaulinaKosheleva/izaris, branch main, https://izaris.netlify.app/.

1. Fetch current main before editing; preserve unrelated remote changes. Collect the user's requested changes into one batch.
2. Prepare all changes locally. Preserve read-only planner data, mobile layout, topic assignments and materials. Check JavaScript syntax, affected behavior and existing planner checks. Summarize the concrete result before any required approval.
3. Determine publication authorization from this conversation. An explicit request to publish authorizes this batch: proceed without another question. Otherwise ask once: «Опубликовать весь подготовленный пакет изменений на izaris.netlify.app?» A yes covers all files, commit and push for this batch. A no means leave the work prepared and unpublished. Do not treat silence as approval. Preview-only requests must remain unpublished.
4. Create one commit containing the whole batch and advance main once. Use an expected-head check to avoid overwriting concurrent changes. If main moved, fetch and reconcile before continuing. Do not force-push.
5. Wait for Netlify, fetch the public page and verify the changed content matches the intended revision. Only then report publication and provide the public link.
6. If a write or approval fails, state the exact failure and keep the prepared work. A skill cannot bypass platform approvals, provider permissions or security checks. Explain any unavoidable additional prompt.

Repository owner permissions are not proof of integration write access. Never ask for passwords or tokens in chat. Never claim the old chatgpt.site host updated when only Netlify changed.
