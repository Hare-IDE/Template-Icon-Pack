# Icon-Pack
Template repository for icon packs 

## Structure

An Icon pack for Hare IDE has the next structure

```
{
  "defaults": {
    // HERE OVERWRITE DEFAULT ICONS
    "name": [{
      "light": "url/to/light.svg",
      "dark": "url/to/dark.svg"
    }]
  },
  "contextValues" : {
    // HERE OVERWRITE ICONS FOR CONTEXT VALUES
    "folder": {
      "default": [{
        "light": "url/to/light.svg",
        "dark": "url/to/dark.svg",
        "when": "state == collapsed" // OPTIONAL IF ITEM IN TREE VIEW CAN BE EXPANDED
      },{
        "light": "url/to/light.svg",
        "dark": "url/to/dark.svg",
        "when": "state == expanded"
      }],
      "regex": {
        // MATCH REGEX EXPRESSION IN ORDER
        "css": [{
          "light": "url/to/light.svg",
          "dark": "url/to/dark.svg",
          "when": "state == collapsed"
        },{
          "light": "url/to/light.svg",
          "dark": "url/to/dark.svg",
          "when": "state == expanded"
        }]
      }
    },
    "file": {
      "default": [{
        "light": "url/to/light.svg",
        "dark": "url/to/dark.svg"
      }],
      "regex": {
        "*.tsx": [{
          "light": "url/to/light.svg",
          "dark": "url/to/dark.svg"
        }]
      }
    }
  }
}
```
