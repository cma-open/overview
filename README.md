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

overview repo
- used for project planning and organisation overview
- independant from other repos
- host development plan in the wiki

workflows repo
- used to provide shared action workflows to other repos

cma-training rep
- used to hold code course progress
- host code snippets
- function, class and module code examples

science-alt repo
- used to illustrate interaction between core and dependency repos (private)
- simple python package (core)
- example use only (not for project use)

science repo
- used to illustrate interaction between core and dependency repos (private)
- simple python package (core)
- example use only (not for project use)

tools repo
- used to illustrate interaction between core and dependency repos (private)
- simple python package (dependency)
- not for use as an independant package
- example use only (not for project use)

cmatools repo (TEMPLATE WIP)
- https://github.com/cma-open/cmatools
- used to illustrate interaction between core and dependency repos (public)
- python package hosting commonly used tools (dependency)
- not for use as an independant package 
- acts as a template (easily create new repos with this structure and starting content)
- example use only (not for project use)
- (conversion / extend for use by projects - WIP)
- used by 
    - cmadata
    - cmascience
    - camsimple

cmadata repo
- used to provide synthetic data for testing or development
- python package (core or dependency)
- can be used as an independant package
- example use only (not for project use)
- (conversion / extend for use by projects - WIP)
- used by
    - WIP 

cmascience repo (TEMPLATE WIP)
- used to illustrate interaction between core and dependency repos (public)
- mimics a simple science based project package 
- python package (core)
- WIP extend to template
- example use only (not for project use)
- (conversion / extend for use by projects - WIP)

cmasimple repo (TEMPLATE WIP)
- mimics a very simple python package 
- allow quick testing and examples of package features
- python package (core)


---

Summary


| repo            | core use        | dependency use  | wiki            |
| --------------- | --------------- | --------------- | --------------- |
| overview        | No              | No              | Yes             |
| workflows       | No              | Yes             | No              |
| cma-training    | No              | No              | No              |
| science-alt     | Yes             | No              | No              |


core = used as an independnt python package
dependency = only used as a dependency to a core package

---

WIP and next steps

science
- new simple template "science" project




