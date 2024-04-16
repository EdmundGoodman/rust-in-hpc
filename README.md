# Assessing the suitability of Rust for performant and productive implementations of HPC codebases

A third year project in partial requirement for a Computer Science BSc at the
University of Warwick, supervised by Dr Richard Kirk.

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
