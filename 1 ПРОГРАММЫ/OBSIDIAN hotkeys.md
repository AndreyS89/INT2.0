---
DATE: 2024-10-14 08:16
CLASS: -10 ПРОГРАММЫ
TYPE: OBSIDIAN
SubTYPE: hotkets
cover: 
note: Горячие клавиши
excalidraw-plugin: parsed
tags:
  - excalidraw
excalidraw-open-md: true
---
## *table*
```dataview
TABLE
	note as "Примечание",
	cover as "Cover"
WHERE CLASS = "20 ПРОГРАММЫ" where TYPE = "-" where SubTYPE != "-"
SORT published
```
---
# [[OBSIDIAN hotkeys]]
## Navigation
- `Ctrl + O` - search - open / create a note
- `Ctrl + tab` -  switch tab
- **!** `Ctrl + Shift + J` - Move file to order
- `Ctrl + E` - switching between - viewing / editing 
- **!** `Ctrl + Shift + G` - to open local graph
- `Ctrl + W` - Close current table
- **!** `Alt + Shift + O` - Collapse the list
- **!** `Alt + Shift + P` - Expand the list

- **!** `Alt + Shift + I` - Collapse everything

- **!** `Ctrl + Alt + J` - *MetaData Menu*

## Excalidraw
- **!** `Ctrl + Q` - Toggle beetween Excalidraw and Markdown mode
- **!** `Alr + Q` - Excalidraw: Add back-of-note card

## Split
- **!** `Ctrl + Shift + L` - Split down
- **!** `Ctrl + Shift + K` - Split right
## Edit
- `F2` - Editing the title
## Insert
- **!** `Ctrl + Shift + A` - Insert template
- `Ctrl + K` - Вставить быструю ссылку
## Create
- `Ctrl + N` - Create new note
- **!** `Ctrl + Shift + D` - delete current file
- `Ctrl + T` - Create new table
## Images
- `[links](https://...]` - links
- `![.... .jpeg | 200]` - Image size `200`
## Inserts
- `> ` - quote
- \`computer code\` - `computer code`

## Links
- `[[ ]]`**#** - Решётка - ссылка на блок

## Callout
> [!question] Can callouts be nested? 
> > [!todo] Yes!, they can. 
> > > [!example] You can even use multiple layers of nesting.

- >[!info] Name
	- qoute
	- example
	- tip
	- faq
	- question
	- todo
	- example
# PLUGINS
## GIT
- `Ctrl + Shift + [` - Git Pull  *Принять изменения*
- `Ctrl + Shift + ]` - Git Push  *Отправить изменения* 
- `Ctrl + Shift + C` - Git commit  *Добавить коммит* 
## Natural Language Dates
- `Ctrl + Alt + T` - Settings date  

## Kanban
- `Ctrl + Shift + P` - Edit beetwen markdown and kanban   
## Natural Language Dates

| Input      | Example          | Description                                                          |
| ---------- | ---------------- | -------------------------------------------------------------------- |
| `YYYY`     | `2014`           | 4 or 2 digit year. Note: Only 4 digit can be parsed on `strict` mode |
| `YY`       | `14`             | 2 digit year                                                         |
| `Y`        | `-25`            | Year with any number of digits and sign                              |
| `Q`        | `1..4`           | Quarter of year. Sets month to first month in quarter.               |
| `M MM`     | `1..12`          | Month number                                                         |
| `MMM MMMM` | `Jan..December`  | Month name in locale set by `moment.locale()`                        |
| `D DD`     | `1..31`          | Day of month                                                         |
| `Do`       | `1st..31st`      | Day of month with ordinal                                            |
| `DDD DDDD` | `1..365`         | Day of year                                                          |
| `X`        | `1410715640.579` | Unix timestamp                                                       |
| `x`        | `1410715640579`  | Unix ms timestamp                                                    |
| `gggg`     | `2014`           | Locale 4 digit week year                                             |
| `gg`       | `14`             | Locale 2 digit week year                                             |
| `w ww`     | `1..53`          | Locale week of year                                                  |
| `e`        | `0..6`           | Locale day of week                                                   |
| `ddd dddd` | `Mon...Sunday`   | Day name in locale set by `moment.locale()`                          |
| `GGGG`     | `2014`           | ISO 4 digit week year                                                |
| `GG`       | `14`             | ISO 2 digit week year                                                |
| `W WW`     | `1..53`          | ISO week of year                                                     |
| `E`        | `1..7`           | ISO day of week                                                      |

## Tasks

```
```tasks

- фильтр по не сделанным задачам / сортировка - перевёрнуто -
not done 
sort by scheduled reverse
limit 3

- фильтр по тегу / группировка списка по имени файла - 
tags include 2_KG01
group by filename
limit 2

- фильтр по имени файла / не сделано - 
not done
filename includes PC 2024-03-27
limit 2

- сортировку по приоритетам / группировка списка по имени файла - 
not done
sort by due
sort by priority
sort by scheduled
limit 2

- Фильр по имени / Группировка по стадиям / Фильтр по заголовка - 
filename includes _КОТТЕДЖ KG checklists
group by function (task.heading + '.md' === task.file.filename) ? '' : task.heading
group by function task.status.name.toUpperCase()
heading includes 1-

``````

![[Pasted image 20240327195853.png]]

https://publish.obsidian.md/tasks/Queries/Filters#Custom+Filters

### Примеры запросов к тегам
- `tags include #todo`
- `tags do not include #todo`
- `tag regex matches /#t$/`
    - Выполняет поиск по односимвольному тегу `#t` без вложенных тегов, поскольку `$` совпадает с концом текста тега.
- `tag regex matches /#book$/i`
    - В конце `i` указано, что регистр не чувствителен.
    - Выполняет поиск по таким тегам, как `#book`, `#Book`, `#BOOK` и `$` предотвращает совпадение `#books`, `#book/literature` и т.д.
---
## TRACKER
### Setting
- Должен быть включён **Dataview**

---
# Desk - 0 Obsidian hotkeys

![[0 Obsidian hotkeys.svg]]
%%
# Excalidraw Data
## Text Elements
## Drawing
```compressed-json
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

CUIRBXq/qwa/5JCcABGIXREcIa6Y8EAY8IAA
```
%%