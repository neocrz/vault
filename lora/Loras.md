---
tags:
  - moc
---

```dataview
TABLE WITHOUT ID
("[[" + file.name + "|" + name + "]]") AS "Name", 
desc AS "Description", 
keywords AS "Keywords",
filename AS "Filename",
map(ref-img, (it) => "![Image|100](" + it + ")") AS "Images"
FROM "lora" and #resource/lora 
```
