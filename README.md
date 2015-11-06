# Sync Sketch Plugin
Save your text styles in a Google Sheet and keep your design team in sync. Every time you run this plugin your Sketch text styles will be replaced with those you specify in a spreadsheet. This should make it easier to share typography styles across teams!

# Installation
Install from [Sketch Toolbox](http://sketchtoolbox.com/) (recommended) or [download the zip](https://github.com/nolastan/sync.sketchplugin/releases/download/1.0/sync.sketchplugin.zip), unzip, and open `sync.sketchplugin`.

# Getting started

1. Create a Google Sheet from [this template](https://drive.google.com/previewtemplate?id=17q6GOMM1X6kkvgeL3LeGkRr4C2vOhpM_JiQUWxbBtew&mode=public) (click the "Use this template" button).

2. Visit [Sheetsu](http://sheetsu.com/) and generate an API for your new sheet.

3. Run the Sync command from the plugin menu and paste your Sheetsu URL into the prompt.

All your text styles should now be synced with your spreadsheet. Run the plugin again any time to update. Share your Sheetsu URL with your team to stay in sync.

# Custom API
As an alternative to Google Sheets, you can create a custom JSON api with the following structure:
```
{
  …
  result: [
    {
      Style: "Headline 1",
      Size: "32",
      Color: "DD2E1F",
      Opacity: "85",
      Typeface: "SourceSansPro-Semibold",
      Alignment: "center",
      Line: "40",
      Character: "0"
    },
    …
  ]
}
```
Run the Sync command from the plugin menu and paste your API endpoint URL into the prompt.
