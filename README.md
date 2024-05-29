# Course Proof-Of-Concept

This is the beginnings of an introductory course for scientific programming. It will hopefully evolve into a fully-fledged course.

## Philosophy and Course Layout

The main philosophy behind this course is to teach foundational programming techniques with a focus on scientific and data analysis. However, I want this course to go beyond simple labs, so there is a large emphasis on programming *tooling*, and a *de-emphasis* on the programming language itself. As such, there are multiple versions of the excersizes for different languages well suited to scientific analysis: python, r, and julia. Students are encouraged to complete labs in different languages as they progress.

By the end of this course, you will know how to:
* work with many different types of datasets
* use open-source libraries for scripting
* create packages, including tests and documentation
* problem solve in *multiple* programming languages
* use modern tooling to aid your programming
* generate professional reports, plots, and figures

---

The repository contains a main `excersizes/` directory, which contains a sequence of excersize subdirectories. Each week has 3 options, as subdirectories: `python/`, `julia/`, and `r/`. The `excersizes/` directory looks like this:

```
excersizes/
├── lab_01
│   ├── README.md
│   ├── julia
│   │   ├── solution.jl
│   │   └── tests
│   ├── python
│   │   ├── solution.py
│   │   └── tests
│   └── r
│       ├── solution.r
│       └── tests
├── lab_02
│   └── ...
└── lab_03 ...
```

The `README.md` file, as previously described, contains information related to that week's excersize. There will be a section dedicated to nuances of each language for that particular excersize. The `tests` directory contains unit and/or integration tests. These are not for modification, but will provide students with a way to check their work as they complete the excersize.

The same instructions, but in a nicer format, will also eventually be available on Github. In the meantime, docs can be served locally with `rye run mkdocs serve`.

## Getting Started

### Requirements

[`just`](https://github.com/casey/just) is required for running commands. The documentation site requires [`mkdocs-material`](https://squidfunk.github.io/mkdocs-material/), though this is not a course requirement.

Python, R, and Julia are required as well. There are different requirements for each language, as follows:

#### Python
* [`rye`](https://rye.astral.sh/) is an experimental project management solution for python. It is used to install python, dependencies, format/lint code, run tests, and run scripts.
* [`pytest`](https://docs.pytest.org/en/latest/?badge=latest) is used to run tests. 

Once `rye` is installed, all dependencies can be installed with `rye sync`.
<!--NOTE: This will probably be changed to some simple command with `just`.-->

#### R
* [`renv`](https://rstudio.github.io/renv/index.html) is used to manage R environments, similar to virtualenv's in python.
TODO

#### Julia
TODO

---

# License
This work is licensed under [GNU-GPL](LICENSE.txt).
