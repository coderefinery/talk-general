name: inverse
layout: true
class: middle

---

background-image: url(img/background.png)

---

template: inverse

## How CodeRefinery can help researchers with modular and reproducible software development

---

layout: false

## Software is transforming research

.column[
<img src="img/complex-machine.jpg" style="height: 500px;"/>
]
.column[
- Quality of scientific software is **critical to modern research**
- **Reproducibility** of many computations is questionable
- Scientists often **lack the necessary training** in practices to
  enable them to collaboratively write high-quality scientific software
]

---

template: inverse

# Reproducible research

---

## To reproduce computational results you need

### - The code: .red[share]
### - The right version of the code: .red[version control]
### - The right version of the environment: .red[containers, share]
### - The data: .red[share]

---

## We have tools for reproducible software: .red[we need to build the culture]

### For research data we have

- Policies
- Openness requirement
- Ownership awareness
- Licensing awareness
- Management plans

### For research software we have

- ...

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

class: split-50-50

<img src="img/neic.png" style="height: 180px;"/>

- Facilitates the development and operation of high-quality .blue[e-infrastructure solutions]
  in areas of .blue[joint Nordic interest]
- .blue[Distributed organisation] consisting of technical experts from academic high-performance computing centres
- Across the Nordic countries (Denmark, Finland, Iceland, Norway, Sweden)
- Ca. 100 persons contracted by NeIC

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

- **Norway**: Bjørn Lindi, Radovan Bast, Sabry Razick
- **Denmark**: Damon Michael Kasacjak, Erland Hochheim
- **Sweden**: Thor Wikfeldt
- **Finland**: Erik Edelmann, Jyry Suvilehto, Nikolai Denissov, Risto Laurikainen, Sri Harsha Vathsavayi

### Alumni

- Pinja Koskinen, FI
- Lukasz Bartosz Berger, DK
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

## Version control: record snapshots as you develop

<img src="img/commits.jpg" style="width: 800px;"/>

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

## Use code review

### Peer review process in publishing

- Papers are reviewed before they are published
- Maintain standards of quality and credibility

### Code review

- Code is reviewed before it is integrated
- Improve quality
- Learning and knowledge transfer
- [GitHub](https://github.com)/[GitLab](https://gitlab.com)/[Bitbucket](https://bitbucket.org) offer a web solution for code review

*"We don't need code review because we are just two."*

---

## Suggestion: Code reading sessions

### "If you don't have time to read, you don't have the time (or the tools) to write."
([Stephen King’s Top 20 Rules for Writers](http://www.openculture.com/2014/03/stephen-kings-top-20-rules-for-writers.html))

### "Whenever you write, strive for originality, but if you have to steal, steal from the best."
(Woody Allen in Anything Else, 2003)

- Read and discuss code written in your group
- Read code written by others
- Read the classics (source code behind classic tools and libraries written by the masters)

---

## Documentation

- Versioned
- Close to code (same repository)
- Use existing services like https://readthedocs.org

---

template: inverse

# Testing

<img src="img/unit-testing.jpg" style="width: 500px;"/>

([@dave1010](https://twitter.com/dave1010/status/613601365529657344))

---

## Simulations and analysis with .blue[untested software] do not constitute science

"Before relying on a new experimental device, an experimental scientist always
establishes its accuracy. A new detector is calibrated when the scientist
observes its responses to known input signals. The results of this calibration
are compared against the expected response. **An experimental scientist would
never conduct an experiment with uncalibrated detectors - that would be
unscientific**. So too, simulations and analysis with untested software do not
constitute science."

(copied from [Testing and Continuous Integration with
Python](http://katyhuff.github.io/python-testing/), created by Kathryn Huff,
see also the Testing chapter in [Effective Computation In
Physics](http://physics.codes) by Anthony Scopatz and Kathryn Huff)

---

## Testing in a nutshell

In software tests, expected results are compared with observed results in order
to establish accuracy:

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

---

## Automated testing

### Motivation

- More robust code
- Simplify collaboration
- Documentation which is up to date by definition
- Make it easier to contribute code
- Guides towards modular code structure
- Guides towards **simpler code**

### .blue[Automatic testing makes it more difficult to write complicated code]

---

## Tests guide towards modular code structure

#### Good code: pure and easy to test

```python
# function which computes the body mass index
def get_bmi(mass_kg, height_m):
    return mass_kg/(height_m**2)

# compute the body mass index
bmi = get_bmi(mass_kg=90.0, height_m=1.91))
```

#### Less good code: has side effects and is difficult to test

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

class: split-60-40

.column[
<img src="img/suit.jpg" style="width: 400px;"/>
]
.column[
### Suiting up to modify untested code
]

---

template: inverse

# Managing complexity and modular code development

---

## Simple vs. easy

<img src="img/development-speed.svg" style="width: 80%;"/>

---

## Modular design is good

### Examples

- Lego
- Car manufacturing
- Design of your phone or laptop
- Modular composition when you order a laptop
- Success of USB
- Study programs

### Advantages

- Separation of concerns
- Composability
- Leveraging functionality

---

## Purity

- Pure functions have no notion of state: They take input values and return
  values
- Given the same input, a pure function *always* returns the same value
- Function calls can be optimized away
- Pure function == data


<img src="img/bugbarrier.jpg" style="width: 40%;"/>

(Slide taken from [Complexity in software development by Jonas Juselius](https://github.com/scisoft/complexity))

---

## Example: pure vs. stateful

### a) pure

```python
# function which computes the body mass index
def get_bmi(mass_kg, height_m):
    return mass_kg/(height_m**2)

# compute the body mass index
bmi = get_bmi(mass_kg=90.0, height_m=1.91))
```

### b) stateful

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

## .red[function: input $\rightarrow$ output]

## f: $x \rightarrow x^2$

## blender: fruits $\rightarrow$ shake

## oven: (ingredients, temperature, time) $\rightarrow$ cake

## .blue[Pure functions are easier to]

- Test
- Understand
- Reuse
- Parallelize
- Simplify
- Optimize

---

## Composition

- Build complex behavior from simple components
- Composition is key to managing complexity

<img src="img/knit_vs_lego.jpg" style="width: 100%;"/>

(Slide taken from [Complexity in software development by Jonas Juselius](https://github.com/scisoft/complexity))

---

## Divide and conquer

- Split the code up
- Construct your program from parts:
  - functions
  - modules
  - packages (Python) or libraries (C or or C++ or Fortran)
- Split functions/units when they get too long or are hard to name

---

## Encapsulation

- Hide internals by language or by convention (header file in C/C++,
  public/private in Fortran, underscores and `__all__` in Python)
- Import as little as possible
- Export as little as possible
- Document and version interfaces

---

## Simplicity and clarity before elegance before efficiency

### Avoid premature optimization

- Do not optimize
- If you have to optimize, optimize later
- If you have to optimize, measure, do not guess

### Simple is better than complex

- If you cannot understand or explain a function on a cold gray Monday morning before coffee, it is too complex. (Quote adapted from [Pieter Hintjens, Social Architecture, 2009](https://www.gitbook.com/book/hintjens/social-architecture/details))

---

template: inverse

# Infrastructure services

---

## Git repository hosting for Nordic research software

- Repository hosting
- Collaboration
- Code review
- Issue tracking
- Documentation

<img src="img/gitlab-logo.png" style="width: 300px;"/>

## [http://coderefinery.org/repository/](http://coderefinery.org/repository)

## [https://source.coderefinery.org](https://source.coderefinery.or)

---

## Why GitLab?

- Many research groups need the possibility to keep code private at least until research has been published
- GitLab.com is an alternative but data leaves the continent
- GitHub and Bitbucket are potentially expensive for large organizations

### Why Nordic GitLab?

- Basically every organization hosts own GitLab instance
- Join forces
- Minimize maintenance effort
- Data stays in the Nordics
- .blue[Partnering with DeiC]

---

## Alpha: Continuous integration service

.blue[Partnering with DeiC] we are about to deploy a service which will make it easier
for researchers to test their code

<img src="img/travis.jpg" style="width: 800px;"/>

---

# Ideas

- .blue[Binary sharing platform with versions and DOIs]: reproducibility, visibility, and credit
- .blue[Container registry]: reproducible environments
- .blue[Web server]: make it easy for groups to serve web pages
- .blue[Continuous integration service]: make it easy to test code
- .blue[Software certification]

### Observations/criticism

- Often technically easy but politically difficult
- Sometimes fear of committing to long-term services
- 1-2 year commitments too short to motivate people to move
- Groups often need 1 year to move to or from a service

---

# Upcoming events

### [Espoo, Dec 12-14](http://coderefinery.org/workshops/2017-12-12-espoo/): 3-day workshop

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

## Take home messages

### For those who code

- Track versions
- Test code
- Share and publish code
- Peer-review code
- Cite code
- Allow code to be cited
- Choose a license
- Document examples
- Keep documentation in your code repository

### If your friends/customers/colleagues code

- Please let them know about us: [coderefinery.org](http://coderefinery.org)

### For those who decide about budgets

- Help us to remove obstacles and launch long-term services that the community needs

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
