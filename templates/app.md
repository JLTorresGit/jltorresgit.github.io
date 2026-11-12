---
# ─────────────────────────────────────────────────────────────────────────────
# APP PAGE TEMPLATE
# 1. Copy this file to docs/_apps/<Slug>.md   (e.g. docs/_apps/MyApp.md)
# 2. Replace every value below. Empty values ("" or []) are simply hidden.
# 3. The page is published at https://jltorresgit.github.io/<Slug>/
# ─────────────────────────────────────────────────────────────────────────────

name: My App                 # Display name
title: My App                # Browser tab and search title (usually the same as name)
slug: MyApp                  # Folder name, no spaces. Must match the privacy folder and `app:` in the policy
permalink: /MyApp/           # Always /<slug>/  (case-sensitive on GitHub Pages)
order: 10                    # Position on the home page (lower comes first)

platform: Android            # Android, iOS, Windows, Web...
status: ""                   # Optional badge: Available, Beta, Coming soon...
version: ""                  # Optional, e.g. 1.2.0
color: "#3b5bdb"             # Accent color for buttons and the initials icon
icon: ""                     # Optional: /assets/apps/MyApp/icon.png (square, 512×512). Initials are shown if empty

tagline: One sentence that says what the app does.
tagline_es: Una frase que dice qué hace la app.   # Optional Spanish line

links:                       # Each button appears only when its link is filled in
  play_store: ""             # https://play.google.com/store/apps/details?id=com.example.myapp
  app_store: ""
  download: ""
  source: ""

highlights:                  # Short "Privacy at a glance" chips; keep them true to the policy
  - No account or server
  - No ads, analytics or tracking
  - Your data stays on your device

features:                    # Cards in the Features section
  - title: Feature name
    text: One or two sentences about it.
  - title: Another feature
    text: One or two sentences about it.

screenshots: []              # Put images in docs/assets/apps/MyApp/ and list them:
#  - /assets/apps/MyApp/screen-1.png
#  - /assets/apps/MyApp/screen-2.png

details:                     # Free key/value facts, shown as small tiles
  Platform: Android
#  Requires: Android 8.0 or later
#  Languages: English, Español
#  Price: Free
---
A paragraph or two describing the app, in Markdown. This appears under "Privacy at a glance".

You can add more sections with `## Headings`, lists and links. Leave this empty if the tagline and features are
enough.
