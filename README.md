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
## Downloading the project from Github
The easiest way is cloning from the command line with 
* `git clone --recurse-submodules https://github.com/geobe/tbp-base`
## Running the project
* Open a terminal window in the base directory `tbp-base` and run `gradlew bootRun` there.
* Then open [localhost:8080/ui/main](http://localhost:8080/ui/main) in a browser.
## Adding more submodules
On the command line in the base project tbp-base, 
run git command for every additional subproject
* `git submodules add https://github.com/PATH-TO-SUBMODULE [module directory name]`

`module directory name` is optional, default is to use git repository name