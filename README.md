# Overview

Overview repository hosting this readme and content relating to the entire cma-open organisation content

Click links in the chart below to view the repos (subject to permissions for the private repos)

Use of common dependency repos (tools, cmatools) by exemplar projects (both public and private)


```mermaid
flowchart TB
 subgraph Public
    workflows-->cmatools
    cmatools-->cmascience
    cmatools-->simple
    overview
    end
    subgraph Private
    workflows-->tools
    tools-->|dependency|science-alt
    tools-->science
    cma-training
    tools-->cmadata
    B
     click B "https://www.github.com" "This is a tooltip for a link"
    end
```

---

# Key documents

- plan
- other

# Organisation repository list and contents


overview
- used for 
- independant from other repos
- host development plan in the wiki

cmatools
- https://github.com/cma-open/cmatools
- used for
- acts as a template (easily create new repos with this structure and starting content)
- used by 
    - a
    - b 

---

WIP and next steps

science
- new simple template "science" project




