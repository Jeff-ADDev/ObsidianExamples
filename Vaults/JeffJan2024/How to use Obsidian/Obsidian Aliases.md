---
date: 2023-11-15
tags:
  - Obsidian/Aliases
  - Obsidian/Instructional
---

You can add Aliases in line.  For example:
try_aliases:: [one,two,three]

![[Pasted image 20231115163920.png]]
```dataview
TABLE aliases
FROM ""
WHERE try_aliases != null
```
![[Pasted image 20231115164128.png]]
```dataview
TABLE aliases
FROM #Obsidian/Dataview 
WHERE try_aliases = null
```