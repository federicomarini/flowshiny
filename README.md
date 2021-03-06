# flowshiny

## Introduction

This [Docker](http://www.docker.com/) container provides a [`shiny`](http://shiny.rstudio.com/) web application that implements and displays most of the functionality of the [R](http://r-project.org/)/[Bioconductor](http://bioconductor.org) package [`flowcatchR`](http://bioconductor.org/packages/flowcatchR). It is based on the [`rocker/shiny`](https://github.com/rocker-org/shiny) Docker image.

## Installation

This app needs a recent version of Docker:

 * [Docker installation instructions](https://docs.docker.com/installation/#installation)
 * type `docker pull federicomarini/flowshiny` 
 * ... or alternatively clone this repository (`git clone https://github.com/federicomarini/flowshiny.git`) and build the image locally with `cd flowshiny && docker build -t flowshiny .` 

## Usage

 * `docker run -p 3838:3838 federicomarini/flowshiny`
 * If all goes well
    - On Linux, browse to [http://localhost:3838/shinyFlow](http://localhost:3838/shinyFlow) for the [`shiny`](http://shiny.rstudio.com/) web application illustrating the usage of the [`flowcatchR`](http://bioconductor.org/packages/flowcatchR) package
    - On MacOS or Windows running [`Docker Toolbox`](https://www.docker.com/toolbox) find the Docker host URL with `docker-machine ip default|[name of the virtual machine]` and browse to `http://[thatIPaddress]:3838/shinyFlow`

## Other components of the `dockerflow` workflow solution

* [`flowstudio`](https://github.com/federicomarini/flowstudio) - https://github.com/federicomarini/flowstudio
* [`flowjupy`](https://github.com/federicomarini/flowjupy) - https://github.com/federicomarini/flowjupy
* [`dockerflow`](https://github.com/federicomarini/dockerflow) - https://github.com/federicomarini/dockerflow


## Contact
For additional details regarding the functions of [`flowcatchR`](http://bioconductor.org/packages/flowcatchR), please consult the package documentation, the package vignette or write an email to marinif@uni-mainz.de. 

## Bug reports/Issues/New features

Please use https://github.com/federicomarini/flowcatchR/issues for reporting bugs, issues or for suggesting new features to be implemented.
