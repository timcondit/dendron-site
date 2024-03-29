---
id: k63qmya7y4jrnmyy812p3di
title: dendron note lookup
desc: 'Query for notes in your workspace'
updated: 1655577638402
created: 1655577282221
---

## Summary

{{fm.desc}}

## Options

### query
- type: string

Note to query for. Same syntax as [[dendron.topic.lookup]]

### output
- default: `json`
- values: `json|md_gfm|md_dendron`
    - json: JSON output
    - md_dendron: dendron markdown
    - md_gfm: github flavored markdown 

Controls how note is formatted

## Examples

```bash
# creates hello if it does not exist
dendron note lookup --query "tutorial" 
```

- output
    - NOTE: this is truncated for easy viewing

```json
[
    {
        "id": "tbilk9to67d0dwgnjanj5ph",
        "title": "Getting Started",
        "desc": "",
        "updated": 1652280532205,
        "created": 1608051264282,
        "nav_order": 1.1,
        "fname": "tutorial",
        "type": "note",
        "vault": {
            "fsPath": ".",
            "selfContained": true,
            "name": "Dendron"
        },
        "contentHash": "981f271a9d5f1bfbfd66781d3a16b9a8",
        "links": [
            {
                "type": "wiki",
                "from": {
                    "fname": "tutorial",
                    "id": "tbilk9to67d0dwgnjanj5ph",
                    "vaultName": "Dendron-2"
                },
                "value": "tutorial.user-interface",
                "alias": "overview of the Dendron UI",
                "position": {
                    "start": {
                        "line": 5,
                        "column": 27,
                        "offset": 156
                    },
                    "end": {
                        "line": 5,
                        "column": 81,
                        "offset": 210
                    },
                    "indent": []
                },
                "xvault": false,
                "sameFile": false,
                "to": {
                    "fname": "tutorial.user-interface"
                }
            }
        ],
        "anchors": {},
        "children": [
            "wmbd5xz40ohjb8rd5b737cq",
            "rjnqumna1ye82u9u76ni42k",
            "ie5x2bq5yj7uvenylblnhyr",
            "iq3ggn67k1u3v6up8ny3kf5",
            "kl6ndok3a1f14be6zv771c9"
        ],
        "parent": "root",
        "data": {},
        "body": "\nDendron is an IDE for general knowledge.\nCombine the simplicity of markdown with the power of a modern development environment.\n\nTo begin, lets do a quick [[overview of the Dendron UI|tutorial.user-interface]]!\n"
    },
    ...
]
```