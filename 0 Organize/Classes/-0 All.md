---
fields:
  - name: tags
    type: Input
    options: {}
    path: ""
    id: MVEiru
  - name: CLASS
    type: Select
    options:
      sourceType: ValuesFromDVQuery
      valuesList: {}
      valuesFromDVQuery: dv.pages("0 Organize/Classes").map(page => [page.file.name])
    path: ""
    id: DDLUmA
  - name: SubTYPE
    type: Select
    options:
      sourceType: ValuesListNotePath
      valuesList: {}
      valuesListNotePath: 0 Organize/Lookups/SubTYPE.md
    path: ""
    id: 6x51HG
  - name: TYPE
    type: Select
    options:
      sourceType: ValuesListNotePath
      valuesList: {}
      valuesListNotePath: 0 Organize/Lookups/TYPE.md
    path: ""
    id: Jap3R6
  - name: DATE
    type: DateTime
    options:
      dateShiftInterval: 1 day
      dateFormat: YYYY-MM-DD HH:mm
      defaultInsertAsLink: false
      linkPath: ""
    path: ""
    id: CnHdvU
  - name: note
    type: Input
    options: {}
    style:
      italic: true
    path: ""
    id: FfAh25
version: "2.54"
limit: 20
mapWithTag: true
icon: sticky-note
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: 
savedViews: []
favoriteView: 
fieldsOrder:
  - CnHdvU
  - 6x51HG
  - DDLUmA
  - Jap3R6
  - MVEiru
  - FfAh25
---
