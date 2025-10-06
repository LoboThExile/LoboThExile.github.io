This is a dashboard for easy access to projects. 
Dude.. This is lowkey me right now![[gamer.jpg|70]]
### Quick Links
- [[#Projects]]
	- [[#Minecraft]]
	- [[#Roblox Studio]]
	- [[#Blender]]
	- [[#Arduino]]
- [[#Random Crap Lul...]]

---
# Projects
These are projects that are completed or not
<p align=center>
	<video src="assets/jason.webm" width="400" controls style="border-radius: 20px;" volume="0.2">
	</video>
	<br>
	<em>when beheaded in my raging pace</em>
</p>
 Ouch. Loud ^^!!!
### Completed (Any)
```dataview
table name as "Project",
      choice(complete, "Done", "Not Done") as "Completed",
      split(file.folder, "/")[1] as "From"
from "project"
where complete = true
```

```dataview
table name as "Project", priority as "Priority"
from "project"
where length(split(file.folder, "/")) = 2 and complete != true
sort priority desc
limit 5

```


<p align="center">
  <img src="gaming.png" width="400" alt="gamer" style="border-radius: 20px;">
  <br>
  <em>"God damn it Morgan, Did you use ChatGPT on this?"</em>
</p>


### Minecraft

#minecraft

```dataview
table name as "Project", 
      priority as "Priority", 
      choice(complete, "Done", "Not Done") as "Completed"
from "project/minecraft"
where length(split(file.folder, "/")) = 2
sort complete asc, priority desc
```

---

### Roblox Studio

#roblox-studio

```dataview
table name as "Project", 
      priority as "Priority", 
      choice(complete, "Done", "Not Done") as "Completed"
from "project/roblox-studio"
where length(split(file.folder, "/")) = 2
sort complete asc, priority desc
```

---

### Blender

#blender

```dataview
table name as "Project", 
      priority as "Priority", 
      choice(complete, "Done", "Not Done") as "Completed"
from "project/blender"
where length(split(file.folder, "/")) = 2
sort complete asc, priority desc
```

---

### Arduino

#arduino

```dataview
table file.link as "Project", 
      priority as "Priority", 
      choice(complete, "Done", "Not Done") as "Completed"
from "project/arduino"
where length(split(file.folder, "/")) = 2
sort complete asc, priority desc
```

# Random Crap Lul...
