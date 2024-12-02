# Assessing the suitability of Rust for performant and productive implementations of HPC codebases

A third year project in partial requirement for a Computer Science BSc at the
University of Warwick, supervised by [Dr Richard Kirk](https://warwick.ac.uk/fac/sci/dcs/people/richard_kirk/).

## Abstract

> Rust is a type-safe programming language originally developed by Mozilla in
> 2010. Since its first release, it has gained a large community of dedicated
> followers. Designed to be memory safe and have foundations in functional
> programming, it claims to be highly performant, safe, and provide a robust
> development toolchain.
>
> The Mantevo Suite is a collection of mini-apps, largely written in C++ and
> FORTRAN. Mini-apps are small software codebases with performance
> characteristics representative of full-scale applications. They are
> traditionally used for hardware-software co-design, allowing simple but
> accurate estimates of application performance on hardware. However, they can
> also be used to assess the software stack they are run on, for example the
> language in which they are implemented.
>
> This project assesses the suitability of Rust for performant and productive
> implementations of HPC codebases through the example of HPCCG, "the original
> Mantevo mini-app". We present a Rust implementation of HPCCG, showing the
> possibility of applying both shared and distributed memory parallelism in Rust
> to HPC codebases using Rayon and MPI, along with a workflow for translation
> including a novel approach for equivalence checking between Rust and C++. We
> further present a performance analysis within a novel framework empowering
> reproducibility, which empirically shows Rust closely approaches C++ in
> performance on real-world applications. We conclude that Rust is a viable
> language for High-Performance Computing applications, despite its performance
> not matching C++, as it provides commensurate benefits in developer
> productivity such as its compiler guarantees of memory and thread safety.
  
**Keywords:** *High-Performance Computing, Parallel Computing, Mini-application, Mantevo, HPCCG, Rust, C++, OpenMP, Rayon, MPI*  

## Links

- [Dissertation](https://github.com/EdmundGoodman/CS310-dissertation/releases/download/tabula-submission/CS310_dissertation.pdf)
- [P3HPC workshop short-format talk](https://p3hpc.org/workshop/2024/program/#lightning-talks)
- [Metarepo (you are here)](https://github.com/EdmundGoodman/rust-in-hpc)

## Download

This is a meta-repository of the written and software deliverables for this
project, and as such contains nested submodules. To clone a copy containing
all nested submodules, consider running the following command:

```bash
git clone --recurse-submodules -j8 https://github.com/EdmundGoodman/rust-in-hpc
```

## Directory structure

Written project deliverables are typeset in LaTeX, and can be found in the
submodule directories `dissertation/`, `presentation/`, `progress-report/`, and
`specification/`

Software components are contained in the `code/` directory, which has four
subdirectories:

- `helper-scripts/`, software written by the author to acheive corollary goals
  such as aggregating and selecting mini-apps, or proofs-of-concept for data
  races in OpenMP and MPI
- `hpc-multibench/`, the main software component of the project, which contains
  many nested subdirectories
- `hpccg-rs/`, a softlink to within `hpc-multibench/` containing the Rust
  translations of the HPCCG mini-app
- `open-source/`, forks of software projects which were not written by me, but I
  have interacted with in the form of pull requests or issues in the course of
  the project. These are not claimed to be my work.
