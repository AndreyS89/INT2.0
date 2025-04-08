---
banner: "![[Pasted image 20241104215956.png]]"
banner_y: 0.75
DATE: 2024-10-14 07:38
CLASS: -0 All
TYPE: GENERAL
SubTYPE: general
cover: 
note: описание
tags:
cssclass: dashboard
---
# 00 ГЛАВНЫЕ СТАРНИЦЫ
##  **00** *pages*
```dataview
TABLE
	note as "Примечание",
	tags as "Тэги",
	cover as "Cover"
WHERE CLASS != "-0 All" where TYPE = "GENERAL" where SubTYPE = "general"
SORT name
```
## **00** *changes*
- **ИЗМЕНЕНИЯ** *ВЕЗДЕ*
`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(10).file.link)`
- **10 ПРОГРАММЫ**
	`$=dv.list(dv.pages('#prog').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **20 ИНТЕРЬЕРЫ**
	`$=dv.list(dv.pages('#in_project').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **30 ДИЗАЙН**
	`$=dv.list(dv.pages('#dz_project').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **41 CG ART**
	`$=dv.list(dv.pages('#art_cg').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **42 ПИАНИНО**
	`$=dv.list(dv.pages('#art_piano').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **50 AI**
	`$=dv.list(dv.pages('#ai').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **60 ДЕЯТЕЛЬНОСТЬ**
	`$=dv.list(dv.pages('#activity').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`

## **00** *statistics*
- **СТАТИСТИКА** *все страницы*
	- `$=dv.pages().length`
- **0 BD** 
	- `$=dv.paragraph(dv.pages('"0 BD"').length);`
- **1 ПРОГРАММЫ** 
	- `$=dv.paragraph(dv.pages('"1 ПРОГРАММЫ"').length);`
- **2 ИНТЕРЬЕР** 
	- `$=dv.paragraph(dv.pages('"2 ИНТЕРЬЕР"').length);`
- **3 ДИЗАЙН** 
	- `$=dv.paragraph(dv.pages('"3 ДИЗАЙН"').length);`
- **4 ТВОРЧЕСТВО** 
	- `$=dv.paragraph(dv.pages('"4 ТВОРЧЕСТВО"').length);`
- **5 AI**
	- `$=dv.paragraph(dv.pages('"5 AI"').length);`
- **6 ДЕЯТЕЛЬНОСТЬ** 
	- `$=dv.paragraph(dv.pages('"6 ДЕЯТЕЛЬНОСТЬ"').length);`
- **9 Organize** 
	- `$=dv.paragraph(dv.pages('"9 Organize"').length);`
# 10 ПРОГРАММЫ
## **10 ПРОГРАММЫ** *GENERAL*
- **GENERAL**
	- [[!10 PR ПРОГРАММЫ]]
	```dataview
	TABLE
	WHERE CLASS = "-10 ПРОГРАММЫ" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **GENERAL** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#prog').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`

## **10 ПРОГРАММЫ** *LINKS* tags
- *GENERAL*
	- #prog 
	- #obsidian 
	- #blender 
	- #feather
	- #figma 
	- #grasshopper
	- #revit
- *EXTRA*
	- #gh_design 
## **10 ПРОГРАММЫ** *LINKS* extra
- *clasess*
	- [[-10 ПРОГРАММЫ]]
- *templates*
	- [[_10 PROG]]
# 20 ИНТЕРЬЕРЫ
## **20 ИНТЕРЬЕРЫ** *ПРОЕКТЫ*
- **ПРОЕКТЫ**
	- [[!20 IN ИНТЕРЬЕР]]
- **ПРОЕКТЫ** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#in_project').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **20 ИНТЕРЬЕРЫ** *КАТЕГОРИИ*
- **1 УПРАВЛЕНИЕ**
	`$=dv.list(dv.pages('#in_stage_1_management').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **2 ТЕОРИЯ**
	`$=dv.list(dv.pages('#in_stage_2_theory').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **3 REVIT**
	`$=dv.list(dv.pages('#in_stage_3_revit').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **4 BLENDER**
	`$=dv.list(dv.pages('#in_stage_4_blender').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **20 ИНТЕРЬЕРЫ** *LINKS*
### **20** *LINKS* tags
- **interior** tags
	- #in_stage_1_management
	- #in_stage_2_theory
	- #in_stage_3_revit
	- #in_stage_4_blender

- **interior** *projects*
	- #in_project
### **20** *LINKS* extra
- *clasess*
	- [[-20 ИНТЕРЬЕР]]
- *templates*
	- [[_20 IN]]
# 30 ДИЗАЙН
## **30 ДИЗАЙН** *ПРОЕКТЫ*
- **ПРОЕКТЫ**
	- [[!30 ДИЗАЙН]]
- **ПРОЕКТЫ** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#dz_project').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **30 ДИЗАЙН** *КАТЕГОРИИ*
- **1 УПРАВЛЕНИЕ**
	`$=dv.list(dv.pages('#dz_stage_1_management').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **2 ТЕОРИЯ**
	`$=dv.list(dv.pages('#dz_stage_2_theory').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **3 FIGMA**
	`$=dv.list(dv.pages('#dz_stage_3_figma').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **4 НИШИ**
	`$=dv.list(dv.pages('#dz_stage_4_niche').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(50).file.link )`
## **30 ДИЗАЙН** *LINKS*
### **30** *LINKS* tags
- *EXTRA*
	- #dz_stage_1_management
	- #dz_stage_2_theory
	- #dz_stage_3_figma
	- #dz_stage_4_niche

- *PROJECT*
	- #dz_project

# 40 ТВОРЧЕСТВО
## **40 ТВОРЧЕСТВО** *GENERAL*
- **40 ТВОРЧЕСТВО**
	- [[!40 ART ТВОРЧЕСТВО]]
	```dataview
	TABLE
	WHERE CLASS = "-40 ТВОРЧЕСТВО" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **41 CG ART** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#art_cg').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
- **42 ПИАНИНО** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#art_piano').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`

## **40 ТВОРЧЕСТВО** *LINKS*
- **40** *tags*
	- #art *40 ТВОРЧЕСТВО*
	- #art_cg *41 CG ART*
	- #art_piano *42 ПИАНИНО*
- **40** *classes*
	- [[-40 ТВОРЧЕСТВО]]
- **40** *templates*
	- [[_41 ART CG]] *41 CG ART*
	- [[_42 ART PIANO]] *42 ПИАНИНО*
# 50 AI
## **50 AI** *GENERAL*
- **50 AI**
	- [[!50 AI]]
	```dataview
	TABLE
	WHERE CLASS = "-50 AI" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **50 AI** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#ai').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **50 AI** *LINKS* tags
- *GENERAL*
	- #ai
- *EXTRA*
	- 
## **50 AI** *LINKS* extra
- *classes*
	- [[-50 AI]]
- *templates*
	- [[_50 AI]]
# 60 ДЕЯТЕЛЬНОСТЬ
## **60** *GENERAL*
- **GENERAL**
	- [[!60 ДЕЯТЕЛЬНОСТЬ]]
	```dataview
	TABLE
	WHERE CLASS = "-60 ДЕЯТЕЛЬНОСТЬ" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **GENERAL** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#activity').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **60** *LINKS* tags
- *tags*
	- #activity
- *extra*
	- 
## **60** *LINKS* extra
- *classes*
	- [[-60 ДЕЯТЕЛЬНОСТЬ]]
- *templates*
	- [[_60 ДЕЯТЕЛЬНОСТЬ]]
# 70 МЫШЛЕНИЕ
## **70** *GENERAL*
- **GENERAL**
	- [[!70 МЫШЛЕНИЕ]]
	```dataview
	TABLE
	WHERE CLASS = "-70 МЫШЛЕНИЕ" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **GENERAL** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#mind').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **70** *LINKS* tags
- *tags*
	- #mind
- *extra*
	- 
## **70** *LINKS* extra
- *classes*
	- [[-70 МЫШЛЕНИЕ]]
- *templates*
	- [[_70 МЫШЛЕНИЕ]]
# 80 АРХИТЕКТУРА
## **80** *GENERAL*
- **GENERAL**
	- [[!80 АРХИТЕКТУРА]]
	```dataview
	TABLE
	WHERE CLASS = "-80 АРХИТЕКТУРА" where TYPE != "GENERAL" where SubTYPE = "general"
	SORT published
	```
- **GENERAL** *ИЗМЕНЕНИЯ*
	`$=dv.list(dv.pages('#arch').where(f => f.file.name != '!0 BD NAMES').sort(f => f.file.name, "desc").limit(10).file.link )`
## **80** *LINKS* tags
- *tags*
	- #arch
- *extra*
	- 
## **80** *LINKS* extra
- *classes*
	- [[-80 АРХИТЕКТУРА]]
- *templates*
	- [[_80 АРХИТЕКТУРА]]
