name: inverse
layout: true
class: middle

---

background-image: url(img/background.png)

---

layout: false

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

### Team (emphasis: present at this conference)

- **Bjørn Lindi**
- **Erik Edelmann**
- **Jyry Suvilehto**
- Lukasz Bartosz Berger
- Nikolai Denissov
- **Radovan Bast**
- Risto Laurikainen
- Sabry Razick
- Sri Harsha Vathsavayi
- **Thor Wikfeldt**

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

class: split-50-50

.column[
## Centralized workflow

<img src="img/centralized.svg" style="height: 400px;"/>
]
.column[
## Code review workflow

<img src="img/forking-overview.svg" style="height: 400px;"/>
]

---

## .blue[2017: Are you using peer review in publishing?]

### *Of course! What else?*

---

## .blue[2017: Are you using peer review in publishing?]

### *Of course! What else?*

## .blue[2017: Are you using code review in code development?]

### *I don't know what it is.*
### *I don't know how to do it.*
### *I don't have time to do it.*

---

## .blue[2017: Are you using peer review in publishing?]

### *Of course! What else?*

## .blue[2017: Are you using code review in code development?]

### *I don't know what it is.*
### *I don't know how to do it.*
### *I don't have time to do it.*

## .blue[202X: Are you using code review in code development?]

### *Of course! What else?*

---

template: inverse

## Infrastructure plans

---

## Plan: Nordic-wide code repository hosting platform

- Repository hosting
- Code review
- Issue tracking
- Documentation

<img src="img/gitlab-logo.png" style="width: 400px;"/>

### Challenge: long term funding

---

## Plan: Continuous integration service

- [Travis CI](https://travis-ci.org), [GitLab CI](https://about.gitlab.com/gitlab-ci/), [Jenkins](https://jenkins.io), [Drone](https://github.com/drone/drone), [AppVeyor](https://www.appveyor.com), ...
- Test every changeset
- We plan to deploy a service which will make it easier for researchers to test their code

<img src="img/travis.jpg" style="width: 800px;"/>

---

class: split-50-50

## Slides: [bit.ly/neic-2017-coderefinery](http://bit.ly/neic-2017-coderefinery)

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
