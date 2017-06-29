name: inverse
layout: true
class: middle

---

background-image: url(img/background.png)

---

template: inverse

# .blue[How CodeRefinery can support ARC software and vice versa]

## 1. Introduce the CodeRefinery project
## 2. Recommendations for ARC release cycle

---

layout: false
class: split-50-50

## Software is transforming research

.column[
<img src="img/complex-machine.jpg" style="height: 500px;"/>
]
.column[
- Quality of scientific software is **critical to modern research**

- Scientists often **lack the necessary training** in practices to
  enable them to collaboratively write high-quality scientific software
]

---

## Many researchers struggle with code complexity

<img src="img/joe-paradiso-modular-synth-front.jpg" style="height: 450px;"/>

(c) Joe Paradiso

---

class: split-60-40

## Goals: Better science with better software

.column[
<img src="img/bromance.jpg" style="height: 360px;"/>

(c) The New Yorker, Oct 17, 2016
]
.column[
- Provide researchers with **infrastructure**, **training**, and **guides** in the necessary tools
  and techniques to create sustainable, modular, reusable, and reproducible
  software
- Build **strong partnerships** with related initiatives
]

---

## FAQ: How do we differ?

### [Software Carpentry](https://software-carpentry.org)

- Teaching basic lab skills for research computing.

### [The Software Sustainability Institute](https://www.software.ac.uk)

- Cultivate better, more sustainable, research software to enable world-class
  research (better software, better research).

### [CodeRefinery](https://www.software.ac.uk)

- Training in skills and tools for students/researchers who write code.
- Managing complexity and collaborative modular development.
- Provide infrastructure services.

---

.left-column[
<img src="img/neic.png" style="height: 50px;"/>

<img src="img/csc.png" style="height: 90px;"/>

<img src="img/deic.png" style="height: 50px;"/>

<img src="img/sigma2.jpg" style="height: 60px;"/>

<img src="img/snic.png" style="height: 20px;"/>
]
.right-column[
## CodeRefinery launched September 2016

- Nordic e-Infrastructure Collaboration project
- Funded for two years
- We are a team of enthusiasts located in DK, FI, NO, SE

### Team

- Bjørn Lindi
- Erik Edelmann
- Jyry Suvilehto
- Lukasz Bartosz Berger
- Nikolai Denissov
- Radovan Bast
- Risto Laurikainen
- Sabry Razick
- Sri Harsha Vathsavayi
- Thor Wikfeldt

### Alumni

- Pinja Koskinen
]

---

## [Ten simple rules for making research software more robust](https://doi.org/10.1371/journal.pcbi.1005412)

**M. Taschuk, G. Wilson** (2017). PLoS Comput Biol 13(4): e1005412.

- Use **version control**
- **Document** your code and usage
- Make common operations easy to control
- **Version** your releases
- **Reuse** software (within reason)
- Rely on **build tools** and package managers for installation
- Do not require root or other special privileges to install or run
- Eliminate hard-coded paths
- Include a small **test set** that can be run to ensure the software is actually working
- Produce identical results when given identical inputs

---

class: split-60-40

## Coming to a city near you

.column[
<img src="img/map.jpg" style="height: 380px;"/>

### Challenge: disciplines are at different levels
]
.column[
- Dec 2016 - Helsinki
- Feb 2017 - Stockholm
- May 2017 - Copenhagen
- May 2017 - Umeå
- Jun 2017 - Tromsø
- Oct 2017 - Aarhus
- Nov 2017 - Linköping
- Dec 2017 - Helsinki
- Feb 2018 - Trondheim
- Mar 2018 - Turku
- Apr 2018 - Odense
- May 2018 - Uppsala
- Jun 2018 - Oslo
- Aug 2018 - Reykjavík
]

---

## Git repository hosting for Nordic research software

- Repository hosting
- Collaboration
- Code review
- Issue tracking
- Documentation

<img src="img/gitlab-logo.png" style="width: 300px;"/>

- http://coderefinery.org/repository/
- https://source.coderefinery.org

## Plan: continuous integration service for Nordic research software

---

template: inverse

## Recommendations for ARC development and release cycle

### .blue[Disclaimer: given by outside person and friend who understands that there is history and a large developer and user base]

---

## Track versions with Git

### Subversion

- Centralized
- One server keeps track of versions
- Working copies are "thin clients"
- Commits are often too small (incomplete) or too large (too many unrelated changes)
- Simple user interface

---

## Track versions with Git

### Subversion

- .blue[Centralized]
- One server keeps track of versions
- Working copies are "thin clients"
- Commits are often too small (incomplete) or too large (too many unrelated changes)
- Simple user interface

### Git

- .blue[Distributed]
- Clones ("working copies") are full copies and equivalent
- Allows to **edit commits** (you can commit often *and* have nice commits)
- Allows to commit without network
- Enables **forking workflow**
- Lightweight branches
- Simple branching and merging
- User interface first overwhelming, later turns simple

---

class: split-50-50

.column[
## Centralized workflow

<img src="img/centralized.svg" style="height: 400px;"/>
]
.column[
## Forking workflow

<img src="img/forking-overview.svg" style="height: 400px;"/>
]

---

## Use forking workflow

- Allows to write-protect central repository
- Enables code review (can be done at branch level as well)
- Enables to decentralize development
- Simplifies external contributions
- Simplifies development of derivative code
- Derivative code is good for the base code
- Keeps list of branches is central repository clean
- Risk: community fragmentation

*"But code review slows things down?"*

---

## Use code review

- Like peer review in publishing
- Maintain standards of quality
- Allows to enforce good commit messages (and therefore minimize work to generate changelog and list of features)
- Improve quality
- Learning
- Knowledge transfer
- [GitHub](https://github.com)/[GitLab](https://gitlab.com)/[Bitbucket](https://bitbucket.org) offer a web solution for code review
- Couple code review with automated testing

---

## Issue tracking

- Currently ARC tracks issues on [Bugzilla](http://bugzilla.nordugrid.org)
- Recommendation: track issues close to source code
- Cross-reference commits, issues, and pull/merge requests
- GitLab offers a lean but powerful issue tracker

---

## Use a continuous integration/deployment service

- Test automatically
- Assist maintenance and release preparation
- Automatically build tarballs and packages
- At each update: spin up a Docker container, build and test, report back

---

## Use https://source.coderefinery.org

- Private and public repositories
- Data stays in the Nordics
- Mutual support of Nordic projects
- Code review and issue tracking in one place
- Soon continuous integration (recipes and service for pilot projects)
- Soon hopefully also websites via GitLab pages

### .blue[ARC is a visible and prominent code and could help CodeRefinery to secure services for smaller clients]

---

## Documentation

- Move documentation closer to sources: same repository
- Simplifies versioning of documentation
- Difficult to coordinate across two repositories
- Documentation is part of code patches
- Use [Markdown](https://daringfireball.net/projects/markdown/syntax) or [reStructuredText](http://docutils.sourceforge.net/rst.html), [Sphinx](http://www.sphinx-doc.org), and [Read the Docs](https://readthedocs.org)
- Use lightweight markup
- Do not maintain own servers
- Wiki-based documentation is often difficult to version

---

## [Semantic versioning](http://semver.org)

- http://semver.org
- This is essentially already used without naming it

### Given a version number MAJOR.MINOR.PATCH, increment the:

- MAJOR when you make .blue[API-breaking changes]
- MINOR when you add .blue[backwards-compatible functionality]
- PATCH when you make .blue[backwards-compatible bug fixes]

Communicate to users/clients about what to expect from new versions

---

## Consider adapting the branching model

- Trunk/master collects commits towards next major version
- Write-protect trunk/master
- Sort commits before they go to trunk/master
- Developers/team decide about the scope of a commit by choosing the appropriate target branch
- No communication/coordination needed after a commit has been accepted
- Continuous release preparation

---

## Semantic branching model

- https://dev-cafe.github.io/branching-model/

<img src="img/branching-model.svg" style="height: 360px;"/>

---

## Configure and build code using CMake instead of Autotools

- Portability
- Excellent support for modular code development
- Good tooling

---

## Conclusions 1/2

### Impressions

- ARC project has very well documented policies
- Excellent manuals and documentation
- Openness
- Very professional release cycle

### Recommendations

- Git
- GitLab (or GitHub)
- Code review
- Documentation goes with sources
- Use CI to build, test, and deploy code

---

## Conclusions 2/2

- Maintenance work load will not disappear but may shift
- Good code review takes time
- Already modest code review can have significant effect
- .blue[Do not change tools before preparing a support structure]

---

class: split-50-50

## Slides: [bit.ly/nordugrid-2017](http://bit.ly/nordugrid-2017)

.column[
## Get in touch!

## [coderefinery.org](http://coderefinery.org)

## [@coderefine](https://twitter.com/coderefine)

## [github.com/coderefinery](https://github.com/coderefinery)

## [coderefinery@googlegroups.com](https://groups.google.com/group/coderefinery)
]
.column[
<img src="img/logo.jpg" style="height: 250px;"/>
]
