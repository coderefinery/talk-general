name: inverse
layout: true
class: center, middle

---

background-image: url(img/front.png)

# The CodeRefinery Project

## Radovan Bast

[coderefinery.org](http://coderefinery.org) | [@coderefine](https://twitter.com/coderefine) | [neic.nordforsk.org](https://neic.nordforsk.org)

---

layout: false
class: split-50-50

<img src="img/neic.png" style="height: 100px;"/>

### Nordic e-Infrastructure Collaboration

- Facilitates the development and operation of high-quality e-Infrastructure solutions in areas of joint Nordic interest
- Distributed organisation consisting of technical experts from academic high-performance computing centres
- Across the Nordic countries (Denmark, Finland, Iceland, Norway, Sweden)
- Ca. 65 persons contracted by NeIC

---

## Software is transforming research

.column[
<img src="img/complex-machine.jpg" style="height: 500px;"/>
]
.column[
- Quality of scientific software is **increasingly becoming critical** for the advancement of knowledge

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
- This project is not about efficient code but rather about **efficient coding**
]

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
- Sabry Razick
- Sri Harsha Vathsavayi
- Thor Wikfeldt

### Alumni

- Pinja Koskinen
]

---

## Version control: record every change

<img src="img/commits.jpg" style="width: 800px;"/>

*"I don't need version control because it is just me."*

---

## Version control: make it possible to collaborate

<img src="img/network.jpg" style="width: 800px;"/>

- We plan to deploy a Nordic-wide code repository hosting platform

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

### Bonus

- Robust code
- Best documentation
- Simplify collaboration
- Guides towards modular code structure

---

class: split-60-40

.column[
<img src="img/suit.jpg" style="width: 400px;"/>
]
.column[
- Suiting up to modify untested code
]

---

### Good code (pure)

```python
# function which computes the body mass index
def get_bmi(mass_kg, height_m):
    return mass_kg/(height_m**2)

# compute the body mass index
bmi = get_bmi(mass_kg=90.0, height_m=1.91))
```

### Less good code (side effects)

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

### But we need to deal with state somewhere
]

---

## Recommendations

- Keep I/O on the outside and connected
- Always read/write on the outside and pass data
- Do not read/write deep down inside the code
- Keep the inside of your code pure/stateless
- Move all the state "up" to the caller
- Keep the stateful outside shell thin
- Unit test the inside
- Regression test the shell

![](img/good-vs-bad.svg)

---

## Continuous integration service

- [Travis CI](https://travis-ci.org)
- [Jenkins](https://jenkins.io)
- Test every changeset
- We plan to deploy a service which will make it easier for researchers to test their code

<img src="img/travis.jpg" style="width: 800px;"/>

---

## Documentation

- Close to the code (minimize barrier)
- **Versions**: If the project has versions, the documentation should too
- Lightweight markup (LaTeX is not lightweight enough)
- Readable on any device
- Division into tutorials and keyword reference
- Tutorials contain good defaults
- Ready examples that one can copy-paste to get quickly started
- Prose, written by humans

### Current gold standard (in my opinion):

### [GitHub](https://github.com)/[GitLab](https://gitlab.com)/[Bitbucket](https://bitbucket.org) -> [RST](http://docutils.sourceforge.net/rst.html)/[Sphinx](http://www.sphinx-doc.org) -> [Read the Docs](https://readthedocs.org)

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
- Consider code reading sessions

*"We don't need code review because we are just two."*

---

## Code review workflow

<img src="img/code-review.svg" style="height: 500px;"/>

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

## Code complexity/viscosity: simple vs. easy

<img src="img/development-speed.svg" style="width: 600px;"/>

---

## Code sharing platform

### Open-source software

- [GitHub](https://github.com)/[GitLab](https://gitlab.com)/[Bitbucket](https://bitbucket.org)
- Often anonymous download

### Closed-source software

- Typically has paid maintainers
- Own distribution websites

### Open-use software

- Typically no budget
- Often "home-cooked" solutions
- Often anonymous download not enough
- Maintenance burden

---

class: split-60-40

## Coming to a city near you

- [Typical workshop schedule](http://coderefinery.org/workshops/2017-05-09-copenhagen/)

.column[
<img src="img/map.jpg" style="height: 380px;"/>
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

## Upcoming events

### 3-day workshops

- [Copenhagen, May 9-11](http://coderefinery.org/workshops/2017-05-09-copenhagen/)
- Tromsø, Jun 19-21

### [NeIC 2017 conference](http://neic2017.nordforsk.org)

- [Umeå, May 29](http://neic2017.nordforsk.org/workshops/coderefinery/): Mixed Martial Arts - Interfacing Fortran, C, C++, and Python for Great Good!

### Seminars and meetups

- [Oslo, Apr 6](http://www.uio.no/english/services/it/research/events/coderefinery-2017-april.html)
- Stockholm, May 19

---

class: split-40-60

## Get in touch!

.column[
### [coderefinery.org](http://coderefinery.org)

### [@coderefine](https://twitter.com/coderefine)

### [github.com/coderefinery](https://github.com/coderefinery)
]
.column[
<img src="img/magic.jpg" style="height: 300px;"/>
]
