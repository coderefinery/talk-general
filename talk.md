name: inverse
layout: true
class: middle

---

background-image: url(img/background.png)

---

layout: false
class: split-50-50

<img src="img/neic.png" style="height: 180px;"/>

- Facilitates the development and operation of high-quality .blue[e-infrastructure solutions]
  in areas of .blue[joint Nordic interest]
- .blue[Distributed organisation] consisting of technical experts from academic high-performance computing centres
- Across the Nordic countries (Denmark, Finland, Iceland, Norway, Sweden)
- Ca. 100 persons contracted by NeIC

---

## Software is transforming research

.column[
<img src="img/complex-machine.jpg" style="height: 500px;"/>
]
.column[
- Quality of scientific software is **critical to modern research**
- **Reproducibility** of most computations is questionable
- Scientists often **lack the necessary training** in practices to
  enable them to collaboratively write high-quality scientific software
]

---

## Many researchers struggle with code complexity

<img src="img/joe-paradiso-modular-synth-front.jpg" style="height: 450px;"/>

(c) Joe Paradiso

---

## Problem: Red Queen's Race

<img src="img/red_queen.jpg" style="height: 360px;"/>

```
"A slow sort of country!" said the Queen. "Now, here, you see,
it takes all the running you can do, to keep in the same place.
If you want to get somewhere else, you must run at least twice
as fast as that!"
- Lewis Carroll, Through the Looking Glass
```

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
<img src="img/neic.png" style="height: 40px;"/>

<img src="img/csc.png" style="height: 90px;"/>

<img src="img/deic.png" style="height: 50px;"/>

<img src="img/sigma2.jpg" style="height: 60px;"/>

<img src="img/snic.png" style="height: 20px;"/>
]
.right-column[
## CodeRefinery launched September 2016

- Nordic e-Infrastructure Collaboration project
- Funded for two years (**preparing a follow-up!**)
- We are a team of enthusiasts located in DK, FI, NO, SE

### Team

- Bjørn Lindi, NO
- Erik Edelmann, FI
- Jyry Suvilehto, FI
- Lukasz Bartosz Berger, DK
- Nikolai Denissov, FI
- Radovan Bast, NO
- Risto Laurikainen, FI
- Sabry Razick, NO
- Sri Harsha Vathsavayi, FI
- Thor Wikfeldt, SE

### Alumni

- Pinja Koskinen, FI
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

template: inverse

## Reproducible research

---

template: inverse

## Why should **only** the publications benefit humanity as a whole?

## If your results are not reproducible, do they really benefit humanity?

---

class: split-60-40

## To reproduce results you need

.column[
<img src="img/Laboratory_tripod.jpg" style="height: 380px">
- By <a href="//commons.wikimedia.org/w/index.php?title=User:NagayaS&amp;action=edit&amp;redlink=1" class="new" title="User:NagayaS (page does not exist)">NagayaS</a> - <span class="int-own-work" lang="en">Own work</span>, <br /><a href="http://creativecommons.org/licenses/by-sa/4.0" title="Creative Commons Attribution-Share Alike 4.0">CC BY-SA 4.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=56343942">Link</a>


]
.column[
- the right version of the code
- the right version of the environment
- the right version of data
]

---

class: split-40-60

## Workshops and events

.column[
- Dec 2016 - **Helsinki**
- Feb 2017 - **Stockholm**
- May 2017 - **Copenhagen**
- May 2017 - Stockholm
- May 2017 - Umeå
- Jun 2017 - **Tromsø**
- Sep 2017 - Manchester
- Oct 2017 - Umeå
- Oct 2017 - **Aarhus**
- Nov 2017 - **Linköping**
- Dec 2017 - **Helsinki**
- Feb 2018 - **Trondheim**
- Mar 2018 - **Turku**
- Apr 2018 - **Odense**
- May 2018 - **Uppsala**
- Jun 2018 - **Oslo**
- Aug 2018 - **Reykjavík**
]
.column[
<img src="img/map.jpg" style="height: 380px;"/>
]

---

template: inverse

## What we preach

---

## Code complexity/viscosity: simple vs. easy

<img src="img/development-speed.svg" style="width: 600px;"/>

---

## Version control: record snapshots as you develop

<img src="img/commits.jpg" style="width: 800px;"/>

---

template: inverse

## "I don't need version control because ..."

- ... it is just me.
- ... we are only two people.
- ... I carefully test my code.
- ... we do not distribute the code.
- ... we are a research group and not a software company.
- ... I do not have time to learn it. It's publish or perish.
- ... I am interested in science and not in software engineering.

---

## Motivation for version control

### Relevant also in a single-person universe

- Undo functionality
- Working on several features in parallel
- Reproducibility
- Bug exposure can be traced back: **code history is extremely valuable**
- Attribution can be determined after the fact: **important for legal reasons**

### Working with others

- People working in parallel on the same project
- Simplify integration of external contributions

---

## Version control: make it possible to collaborate

<img src="img/network.jpg" style="width: 800px;"/>

---

## Branching model

<img src="img/branching-model.svg" style="height: 360px;"/>

---

## Automated testing

```python
def get_bmi(mass_kg, height_m):
    """
    Calculates the body mass index.
    """
    return mass_kg/(height_m**2)


def test_get_bmi():
    bmi = get_bmi(mass_kg=90.0, height_m=1.91)
    expected_result = 24.670376
    assert abs(bmi - expected_result) < 1.0e-6
```

### Motivation

- More robust code
- Simplify collaboration
- Documentation which is up to date by definition
- Make it easier to contribute code
- Guides towards modular code structure

---

class: split-60-40

.column[
<img src="img/suit.jpg" style="width: 400px;"/>
]
.column[
### Suiting up to modify untested code
]

---

### Good code (pure: no side effects)

```python
# function which computes the body mass index
def get_bmi(mass_kg, height_m):
    return mass_kg/(height_m**2)

# compute the body mass index
bmi = get_bmi(mass_kg=90.0, height_m=1.91))
```

### Less good code (impure: side effects)

```python
mass_kg = 90.0
height_m = 1.91
bmi = 0.0

# function which computes the body mass index
def get_bmi():
    global bmi
    bmi = mass_kg/(height_m**2)

# compute the body mass index
get_bmi()
```

---

## Enemy of the state

.left-column[
<img src="img/mad.jpg" style="width: 150px;"/>
]
.right-column[
### Strive for pure functions, fear the state

- Pure functions do not have side effects
- Side effects lead to bugs and increase complexity
- Pure functions are easier to
    - Test
    - Understand
    - Reuse
    - Parallelize
    - Simplify
    - Refactor
    - Optimize
]

---

## Equational reasoning

- We start with a function:
  $$ f(x) $$
- We wish to evaluate this:
  $$ y = f(a) + f(b) \times [f(c) - f(c)] $$
- We can simplify:
  $$ y = f(a) + f(b) \times 0 $$
  $$ y = f(a) $$
- Another example:
  $$ z = f(a) + f(b) + f(c) + f(d) $$
- We know we can rearrange (important for concurrency):
  $$ z = f(b) + f(d) + f(c) + f(a) $$

---

## Concurrency

- Concurrency in imperative code is very hard
- You are totally lost in the dark without a good thread checker
- In a pure, immutable world concurrency is nearly trivial!
- Prefer immutable data to mutable data

<img src="img/floor-loom-diagram.jpg" style="width: 55%;"/>

(Slide taken from [Complexity in software development by Jonas Juselius](https://github.com/scisoft/complexity))

---

## Modular code development

### Modular design is good - examples:

- Lego
- Car manufacturing
- Design of your phone or laptop
- Modular composition when you order a laptop
- Success of USB
- Erasmus study program

### Advantages

- Separation of concerns
- Composability
- Leveraging functionality

---

## Composition

- Build complex behavior from simple components
- We can reason about the components and the composite
- Composition is key to managing complexity
- Modularity does not imply simplicity, but is enabled by it

<img src="img/knit_vs_lego.jpg" style="width: 100%;"/>

(Slide taken from [Complexity in software development by Jonas Juselius](https://github.com/scisoft/complexity))

---

## Documentation

- Close to the code (minimize barrier to contribute)
- **Versions**
- **Branches**
- Lightweight markup
- Readable on any device
- Division into tutorials and API reference
- Tutorials contain good defaults
- Ready examples that one can copy-paste to get quickly started

### Current gold standard

- Hosting: [GitHub](https://github.com) or [GitLab](https://gitlab.com) or [Bitbucket](https://bitbucket.org)
- Markup: [RST](http://docutils.sourceforge.net/rst.html) or [Markdown](http://daringfireball.net/projects/markdown/)
- Rendering: [Sphinx](http://www.sphinx-doc.org) or [GitBook](https://www.gitbook.com)
- Deployed to: [Read the Docs](https://readthedocs.org), [GitHub Pages](https://pages.github.com/)

---

## Building portable and modular code with CMake

- Separation of source and build path
- Portability
- Language support
- Supports modular code development
- Provides tools
- Popular
- General

---

template: inverse

## How can you publish a Nature paper?

---

## How to publish a Nature paper

- Ask the Nature IT admins to give you access to their server
- Promise to submit a high quality paper
  in the right place and using the right format and style
- Once you get access simply upload your article sources
- Make sure the issue looks good
- If somebody complains later, make corrections

---

<img src="img/bizzaro-world.jpg" style="height: 420px;"/>

---

class: split-50-50

.column[
## E-mail workflow

<img src="img/email.svg" style="height: 400px;"/>
]
.column[
## Version control

<img src="img/centralized.svg" style="height: 400px;"/>
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

## Use code review

### Peer review process in publishing

- Papers are reviewed before they are published
- Maintain standards of quality
- Improve performance
- Provide credibility

### Code review

- Code is reviewed before it is integrated
- Improve quality
- Learning
- Knowledge transfer
- [GitHub](https://github.com)/[GitLab](https://gitlab.com)/[Bitbucket](https://bitbucket.org) offer a web solution for code review

*"We don't need code review because we are just two."*

---

## Suggestion: Code reading sessions

- Read and discuss code written in your group
- Read code written by others
- Read code in the standard library


### "Whenever you write, strive for originality, but if you have to steal, steal from the best."
(Woody Allen in Anything Else, 2003)

---

## Suggestions and requests for future topics

- Contribution guides
- How to open-source a project
- Software licenses
- Reproducible science

---

template: inverse

## Infrastructure plans

---

## Git repository hosting for Nordic research software

- Repository hosting
- Collaboration
- Code review
- Issue tracking
- Documentation

<img src="img/gitlab-logo.png" style="width: 300px;"/>

- [http://coderefinery.org/repository/](http://coderefinery.org/repository)
- [https://source.coderefinery.org](https://source.coderefinery.or)

---

## Why GitLab?

- Repositories typically need to be private at least until research has been published
- Research institute bureaucracy can be difficult for small, pay-per-seat per-user services

---

## Plan: Continuous integration service

- [Travis CI](https://travis-ci.org), [GitLab CI](https://about.gitlab.com/gitlab-ci/), [Jenkins](https://jenkins.io), [Drone](https://github.com/drone/drone), [AppVeyor](https://www.appveyor.com), ...
- Test every changeset
- We plan to deploy a service which will make it easier for researchers to test their code

<img src="img/travis.jpg" style="width: 800px;"/>

---

# Ideas

- Binary sharing platform with versions and DOIs: reproducibility, visibility, and credit
- Docker registry: reproducible environments
- Web server: make it easy for groups to serve web pages
- Continuous integration service: make it easy to test code

### Observations/criticism (consume with grain of salt)

- Often technically easy but politically difficult
- Sometimes fear of committing to useful long-term services
- 1-2 year commitments too short to motivate people to adopt
- Huge long-term cost in being slow implementing services

---

# Upcoming events

### [Umeå, Oct 16](http://coderefinery.org/events/2017-10-16-umea/): Git-themed one day workshop
### [Aarhus, Oct 24-26](http://coderefinery.org/events/2017-10-24-aarhus/): 3-day workshop
### Linköping, Nov 7-9: 3-day workshop
### Espoo, Dec 12-14: 3-day workshop

## Find all events here: [coderefinery.org/workshops/](http://coderefinery.org/workshops/)

You can sign up to get notified when registration opens
(see [coderefinery.org/workshops/](http://coderefinery.org/workshops/)).

---

<img src="img/logo.jpg" style="height: 250px;"/>

## CodeRefinery in the press

- https://neic.no/news/2017/03/15/better-software-leads-to-better-science/
- https://www.deic.dk/news/2017-05-10/CodeRefinery
- https://www.pdc.kth.se/news/news-repository/coderefinery-workshop-in-espoo
- https://www.pdc.kth.se/newsletter/2017-1/pdc-newsletter-2017-no.-1
- https://csc.fi/de/web/blog/post/-/blogs/coderefinery-and-the-red-queen-s-race

---

class: split-70-30

.column[
# Get in touch!

## Web: [coderefinery.org](http://coderefinery.org)

## Twitter: [@coderefine](https://twitter.com/coderefine)

## Sources: [github.com/coderefinery](https://github.com/coderefinery)

## Discuss: [coderefinery@googlegroups.com](https://groups.google.com/group/coderefinery)

## Questions: [support@coderefinery.org](mailto:support@coderefinery.org)
]
.column[
<img src="img/logo.jpg" style="height: 150px;"/>
]
