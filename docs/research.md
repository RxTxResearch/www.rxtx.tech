---
ᴴₒᴴₒᴴₒ: true
hide:
    - navigation
title: Research
---

# RxTx Research

> RxTx Research is utilizing the latest computational biochemical and biophysical scientific findings to develop the next generation open-source software for academic and industrial applications.

## Talks

We held talks about [RxDock](https://rxdock.gitlab.io/) at [University of Auckland School of Chemical Sciences](https://www.auckland.ac.nz/en/science/about-the-faculty/school-of-chemical-sciences.html) and [University of Rijeka Department of Biotechnology](https://www.biotech.uniri.hr/) seminars. The recordings are embedded below.

### University of Auckland School of Chemical Sciences (22nd May 2020)

<iframe src="https://www.youtube.com/embed/NH6XSRdezyI" title="YouTube video player" style="border: 1px solid black; width: 100%; height: 25rem" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### University of Rijeka Department of Biotechnology (14th February 2020)

<iframe src="https://www.youtube.com/embed/0GuQMdhOQVA" title="YouTube video player" style="border: 1px solid black; width: 100%; height: 25rem" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Publications

### Papers in conference proceedings

1. **Miletić, V.**, **Nikolić, P.** & Kinkela, D. [Structure-based Molecular Docking in the Identification of Novel Inhibitors Targeting SARS-CoV-2 Main Protease.](https://ieeexplore.ieee.org/document/9596660) in 2021 44th [International Convention on Information, Communication and Electronic Technology (MIPRO)](http://www.mipro.hr/), 435–440 (2021). [doi:10.23919/MIPRO52101.2021.9596660](https://doi.org/10.23919/MIPRO52101.2021.9596660)

### Abstracts in conference proceedings

1. Koren, R., Martinović, M., **Nikolić, P.**, Odorčić, I., Ostojić, L., Visentin, D., Vrbnjak, K., **Miletić, V.** & Svedružić, Ž. M. Supercomputers as microscopes for the 21st century: substrate channeling, epigenetic regulation, and molecular basis of Alzheimer's disease. in [27HSKIKI Book of Abstracts](https://27hskiki.hkd.hr/book-of-abstracts/), Zagreb, Croatia ([Croatian Chemical Society](https://www.hkd.hr/), 2021).

## Projects

### Modernization, modularization, and active maintenance of [RxDock](https://rxdock.gitlab.io), a fast, versatile, and open-source program for docking ligands to proteins and nucleic acids (April 2019 – March 2022)

#### Background

At RxTx, we develop our solutions by using and extending free and open-source software. We strongly believe in keeping the software free and open source as we use, modify, and enhance it to fit our needs. [RxDock](https://rxdock.gitlab.io) is a fork of [rDock](https://rdock.gitlab.io/), a fast, versatile and open-source ([LGPLv3](https://www.gnu.org/licenses/lgpl-3.0.en.html)) program for docking ligands to proteins and nucleic acids. For a non-developer perspective, see the documentation linked below. For a developers perspective, read on.

The original rDock started in the late 1990s and RxDock forked from it in 2019. Considering the speed of software evolution, that time points are several lifetimes apart in the world of software development. Some wrinkles here and there in code are to be expected and, while we at RxTx and the community around us are very busy ironing these wrinkles, they admittedly are there. [The primary target systems](https://rxdock.gitlab.io/documentation/devel/html/developer-guide/target-platforms.html) for RxDock are Linux on AMD64 (x86-64) with the GCC compiler as well as FreeBSD on AMD64 with the Clang compiler.

#### Goal

[RxDock](https://rxdock.gitlab.io/) should become the high-throughput virtual screening engine for workstations, high performance computers, and the cloud. The goal of this project was to evolve the molecular docking code for running on modern computers, including supercomputers and clouds.

#### People

##### Core team

* [Dr. Vedran Miletić](https://vedran.miletic.net/) ([GitHub](https://github.com/vedranmiletic), [LinkedIn](https://www.linkedin.com/in/vedranmiletic/), [Twitter](https://twitter.com/vedranmiletic))
* [Dr. Davide Mercadante](https://lab.mercadante.net/) ([LinkedIn](https://www.linkedin.com/in/davide-mercadante-274b86113/), [Twitter](https://twitter.com/DavideMercadan2))
* [Patrik Nikolić](https://nikoli.ch/) ([GitHub](https://github.com/patrik-nikolic), [LinkedIn](https://www.linkedin.com/in/patrik-nikolic-8aa48310a), [Twitter](https://twitter.com/patriknikolic))
* [Luka Vretenar](https://luka.vretenar.pro/) ([GitHub](https://github.com/lvretenar), [LinkedIn](https://www.linkedin.com/in/luka-vretenar-5137473b/))

##### Contributors

* Sebastian Jennen ([GitHub](https://github.com/zebastian))
* Dominik Kinkela
* Jon Turney

#### Results

The source code has been modernized using [C++11](https://isocpp.org/wiki/faq/cpp11) and beyond. Continuing the great work done by the [rDock](https://rdock.gitlab.io/) project, [RxDock](https://rxdock.gitlab.io/) is using [Meson](https://mesonbuild.com/) for building and automatically downloading missing or outdated dependencies as [wrapped libraries](https://wrapdb.mesonbuild.com/). Testing is now done with [Google Test](https://github.com/google/googletest), linear algebra is powered by [Eigen](https://eigen.tuxfamily.org/), and random number generation by [PCG](https://www.pcg-random.org/). [OpenMP](https://www.openmp.org/) has been used to speed up cavity search. Documentation is written in [reStructuredText](https://www.zverovich.net/2016/06/16/rst-vs-markdown.html) and built by [Sphinx](https://www.sphinx-doc.org/), while API documentation is built by [Doxygen](https://www.doxygen.nl/). There are many other smaller changes; if you are interested in details, until the release notes are written we invite you to check the project commit history on [GitLab](https://gitlab.com/rxdock/rxdock/-/commits/master) or [GitHub](https://github.com/rxdock/rxdock/commits/master) for details.

The development of a streamlined command-line interface using [cxxopts](https://github.com/jarro2783/cxxopts) was started during the project. Development of graphical and web user interfaces are planned in future projects.

#### Learn more

* RxDock website: [home page](https://rxdock.gitlab.io/), [comparison with rDock](https://rdock.gitlab.io/)
* RxDock documentation: [HTML](https://rxdock.gitlab.io/documentation/devel/html), [PDF](https://rxdock.gitlab.io/documentation/devel/pdf/rxdock-documentation-devel.pdf)
* RxDock API documentation [HTML](https://rxdock.gitlab.io/api-documentation/devel/html/), [PDF](https://rxdock.gitlab.io/api-documentation/devel/pdf/rxdock-api-documentation-devel.pdf)
* RxDock source code: [GitLab](https://gitlab.com/rxdock/rxdock), [GitHub](https://github.com/rxdock/rxdock)
