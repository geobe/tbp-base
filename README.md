# Base project repository for the TimeBudgetPlanning Project
Umbrella project that uses git submodules to bring together components
from different git repositories. This project is intended as a sample
project for enterprise application development using Spring, Java, Groovy
and (at least in the beginning) Vaadin in a master course in computer science.

The project evolution starts with a monolithic design, then splits it into 
microservices.
The UI will migrate to a separate microservice when project evolves.

## Used supporting projects
The project uses other projects that are imported from github by this umbrella:
* [associations](https://github.com/geobe/associations) - a library for association 
handling in @Entity classes
* [state-machine](https://github.com/geobe/state-machine) - a simplified state machine
library used for UI behavior modeling
* [vaadin-builder](https://github.com/geobe/vaadin-builder) - a Groovy builder for
simplified construction of Vaadin user interfaces

At start, the core subproject holds all project-specific code:
* [core](https://github.com/geobe/tbp-core)
