# Overview

Overview repository hosting this readme and content relating to the entire cma-open organisation content

Click links in the chart below to view the repos (subject to permissions for the private repos)

Use of common dependency repos (tools, cmatools) by exemplar projects (both public and private)


```mermaid
flowchart TB
 subgraph Public
    workflows
      click workflows "https://github.com/cma-open/workflows" "Link to workflows repo"
    workflows-->cmatools
    cmatools-->cmascience
    click cmatools "https://github.com/cma-open/cmatools" "Link to cmatools"
    overview
      click overview "https://github.com/cma-open/overview" "Link to overview repo"
      click cmascience "https://github.com/cma-open/cmascience" "Link to cmascience repo"
    simple
      click simple "https://github.com/cma-open/simple" "Link to simple repo"
    end
    subgraph Private
    workflows-->tools
    tools-->|dependency|science-alt
      click science-alt "https://github.com/cma-open/science-alt" "Link to scient-alt repo"
    tools-->science
    click science "https://github.com/cma-open/science" "Link to science repo"
    click tools "https://github.com/cma-open/tools" "Link to science repo"
    tools-->cmadata
    click cmadata "https://github.com/cma-open/cmadata" "Link to cmadata repo"
    cma-training
      click cma-training "https://github.com/cma-open/cma-training" "Link to training repo"
    end
```

---

# Key documents

- Development plan https://github.com/cma-open/overview/wiki/Development-plan
- System requirements advice https://github.com/cma-open/overview/wiki/Software-requirements-(generic)

# Organisation repository list and contents

overview repo  (public)
- https://github.com/cma-open/overview
- used for project planning and organisation overview
- independant from other repos
- host development plan in the wiki

workflows repo  (public)
- https://github.com/cma-open/workflows
- used to provide shared action workflows to other repos

cmatools repo (TEMPLATE WIP)  (public)
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

cmascience repo (TEMPLATE WIP)  (public)
- https://github.com/cma-open/cmascience
- used to illustrate interaction between core and dependency repos (public)
- mimics a simple science based project package 
- python package (core)
- WIP extend to template
- example use only (not for project use)
- (conversion / extend for use by projects - WIP)

simple repo (TEMPLATE WIP)  (public)
- https://github.com/cma-open/simple
- mimics a very simple python package 
- allow quick testing and examples of package features
- python package (core)
- no GitHub pages site

cma-training repo  (private)
- https://github.com/cma-open/cma-training
- used to hold code course progress
- hosts code snippets
- function, class and module code examples

science-alt repo  (private)
- https://github.com/cma-open/science-alt
- used to illustrate interaction between core and dependency repos (private)
- simple python package (core)
- example use only (not for project use)

science repo  (private)
- https://github.com/cma-open/science
- used to illustrate interaction between core and dependency repos (private)
- simple python package (core)
- example use only (not for project use)

tools repo  (private)
- https://github.com/cma-open/tools
- used to illustrate interaction between core and dependency repos (private)
- simple python package (dependency)
- not for use as an independant package
- example use only (not for project use)

cmadata repo  (private)
- https://github.com/cma-open/cmadata
- used to provide synthetic data for testing or development
- python package (core or dependency)
- can be used as an independant package
- example use only (not for project use)
- (conversion / extend for use by projects - WIP)
- used by
    - WIP 


---

# Relationships between python package and environment

Two main situations exist.

1. The code repo manages the python package and also manages the environment setup and maintenance
- e.g. repos
    - 1,2,3 (TODO) 

2. Code is managed in seperate repos for the particular python package and a seperate code environment
- e.g.
   - 4,5,6 


---

Summary

| repo            | core use        | dependency use  | wiki         | template | GH page? | env-env | unique env | Status |
| --------------- | --------------- | --------------- | ------------ | -------  | -------- | ------- | ---------- | ------ |
| overview        |                 |                 | Yes          |          |          |         |            | Active |
| workflows       |                 | Yes             |              |          |          |         |            | |
| cma-training    |                 |                 |              |          |          |         |            | |
| science-alt     | Yes             |                 |              |          |          |         |            | |
| science         | Yes             |                 |              |          |          |         |            | |
| tools           |                 | Yes             |              |          |          |         |            | |
| cmadata         |                 | Yes             |              |  WIP     |          |         |            | |
| cmascience      |                 | Yes             | WIP          |  WIP     |          |         |            | |
| cmatools        |                 | Yes             | Yes          |  WIP     |    Yes   |         |            | |
| simple          | Yes             |                 |              |  WIP     |          |         |            | |
| project         |                 |                 |              |          |          |   Yes   |            | |


- core = used as an independent python package
- dependency = only used as a dependency to a core package
- status = Active / WIP / Retired

---




