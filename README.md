# Notion widgets

Small tools for personal Notion pages and the web: a calendar, sticky notes, a daily panel and a KaTeX designer.

## The collection

| Tool | What it does | Open it | Source |
| --- | --- | --- | --- |
| Mini Calendar | Responsive calendar with month and week views, navigation and filters | [Calendar](https://numinull.github.io/notion_widgets/Mini%20Calendar.html) | [Mini Calendar.html](Mini%20Calendar.html) |
| Sticky Notes | Editable reminder note with appearance settings | [Sticky note](https://numinull.github.io/notion_widgets/Sticky_Notes.html) | [Sticky_Notes.html](Sticky_Notes.html) |
| Daily Panel | Daily words, reading and facts from TheFreeDictionary | [Daily panel](https://numinull.github.io/notion_widgets/daily_panel.html) | [daily_panel.html](daily_panel.html) |
| KaTeX Designer | Preview and customise equation styling for Notion | [Designer](https://numinull.github.io/notion_widgets/katex_designer.html) | [katex_designer.html](katex_designer.html) |

## Use a widget

1. Open a tool using the links above.
2. For an embedded widget, copy its URL, type `/embed` in Notion and paste the link.
3. Resize the Notion block to suit your page.

Use the KaTeX Designer in a browser to prepare equation styling for Notion. The tools are standalone pages; they do not require a package installation or build step.

## Run locally

Download the repository, or clone it:

```sh
git clone https://github.com/numinull/notion_widgets.git
cd notion_widgets
python3 -m http.server 8000
```

With Python 3 installed, this serves the files at [localhost:8000](http://localhost:8000/). Choose an HTML file from the directory listing. Keep the server running while you preview changes; press Ctrl+C to stop it.

## Customisation and saved data

Each HTML file contains its own page structure, styles and scripts. Use the widget's controls where available; edit the file for deeper changes.

Sticky notes, calendar preferences, daily-panel compact mode and designer presets use local browser storage. Treat browser storage as local to the browser and embed context you are using, rather than as a cross-device backup.

The Daily Panel loads external content from TheFreeDictionary and fonts from Google Fonts. The KaTeX Designer loads KaTeX from jsDelivr and fonts from Google Fonts. Those features need an internet connection and depend on the external services being available.

## Maintaining the collection

- Keep existing filenames and URLs stable: they may already be embedded in Notion pages.
- Add new tools to the table with a working preview link and a source link.
- Use lowercase, hyphenated filenames for new tools.
- Check the page in a browser and a resized Notion embed after changes.

This repository is `notion_widgets` (with an underscore). Its existing widget URLs use that exact name.
