# pytest-distributed
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![Code style: black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)


### Description

> Given when people touch on large codebases, and run pytest they burn a significant period of time in the order of hours on test suites. 
> `pytest-distributed` greatly simplify that process, in hence, we are creating an complementary plugin to `pytest-xdist`,  with true parralelism at play


So let's begin!

### Ideas Bank

* True Parallelism: first thing that comes to mind here, is use of parallel algorithms.

    - What if we can go beyond Parallel Task Queue implementation? Say, MapReduce - Divide test suites into micro-units (map) and aggregate results (reduce)

* Dynamic Test Distribution: distribute tests across available CPU cores to optimize performance

Possible Strats for True Parallelism:

    Test Distribution by Module?

    Test Distribution by Dependency Graph - I would have to research on this...

    Dynamic Work Stealing: a work-stealing algorithm where idle workers steal work from busy workers, ensuring optimal CPU core utilization.

* Customization Options: Give users access to customize settings based on their specific requirements but not too much power.


### Success Criteria

The project is considered success if:

- It could perform successful parallel test execution in the slightest way possible
