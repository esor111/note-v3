```dataview
table file.mtime as "Last Modified"
from "Projects"
where contains(tags, "#active")
sort file.mtime desc
