# Analysis of point-count data in the presence of variable survey methodologies and detection error

> This course was originally developed for [BIOS2](https://bios2.usherbrooke.ca/2021/02/21/training-point-count-data-analysis/) held on March 16, 18, 23, 25 - Pacific: 9am-12pm, Mountain: 10am-1pm, Central: 11am-2pm, Eastern: 12-3pm

This course is aimed towards researchers analyzing field observations, who are often faced by data heterogeneities due to field sampling protocols changing from one project to another, or through time over the lifespan of projects, or trying to combine 'legacy' data sets with new data collected by recording units.

Such heterogeneities can bias analyses when data sets are integrated inadequately, or can lead to information loss when filtered and standardized to common standards. Accounting for these issues is important for better inference regarding status and trend of species and communities.

Analysts of such 'messy' data sets need to feel comfortable with manipulating the data, need a full understanding the mechanics of the models being used (i.e. critically interpreting the results and acknowledging assumptions and limitations), and should be able to make informed choices when faced with methodological challenges.

The course emphasizes critical thinking and active learning through hands on programming exercises. We will use publicly available data sets to demonstrate the data manipulation and analysis. We will use freely available and open-source R packages.

The expected outcome of the course is a solid foundation for further professional development via increased confidence in applying these methods for field observations.

<img src="https://github.com/psolymos/qpad-workshop/raw/main/images/qpad-sketch.jpg" alt="QPAD overview" width="50%" />


## Instructor

[**Dr. Peter Solymos**](https://peter.solymos.org) \
[Boreal Avian Modelling Project](https://borealbirds.ca) and the [Alberta Biodiversity Monitoring Institute](https://abmi.ca) \
[Department of Biological Sciences](https://www.ualberta.ca/biological-sciences/), [University of Alberta](https://ualberta.ca)

## Outline

Each day will consist of 3 sessions, roughly one hour each, with short breaks in between.

> The video recordings from the workshop can be found on [YouTube](https://www.youtube.com/watch?v=cXGXvAOqEng&list=PLH424kyZX5ip0PfOo7g13nJEQNVxZlMOh).

| Session | Topic | Files | Videos |
| --- | --- | :---: | :---: |
| **Day 1** |  **Naive techniques** |    |    |
|  |  1. Introductions |  [Slides](https://peter.solymos.org/qpad-workshop/day1-1-intro.pdf)  | [Video](https://youtu.be/cXGXvAOqEng) |
|  |  2. Organizing point count data |  [Notes](https://peter.solymos.org/qpad-workshop/day1-2-data-processing.html)  | [Part 1](https://youtu.be/4PLyaU6bqRc), [Part 2](https://youtu.be/dcsiv-v0UgA) |
|  |  3. Regression techniques  |  [Notes](https://peter.solymos.org/qpad-workshop/day1-3-regression.html)  | [Part 1](https://youtu.be/z_TpcF0FD4o), [Part 2](https://youtu.be/ZdTgdTqxFSM) |
| **Day 2** |  **Behavioral complexities**  |    |    |
|  |  1. Statistical assumptions and nuisance variables  |  [Slides](https://peter.solymos.org/qpad-workshop/day2-1-intro.pdf)  | [Video](https://youtu.be/8v3Uf_aILxI) |
|  |  2. Behavioral complexities  |  [Notes](https://peter.solymos.org/qpad-workshop/day2-2-behavior.html)  | [bSims](https://youtu.be/gJ11_wlsEfU), [Video](https://youtu.be/UgGeaxMCs2c) |
|  |  3. Removal modeling techniques  |  [Notes](https://peter.solymos.org/qpad-workshop/day2-3-removal.html)  | [Video](https://youtu.be/ny0ED9cxzeg) |
|  |  4. Finite mixture models and testing assumptions  |  [Notes](https://peter.solymos.org/qpad-workshop/day2-4-mixtures.html)  | [Mixtures](https://youtu.be/A1cnzXMMlxU), [Testing](https://youtu.be/flF5NL73ZZE) |
| **Day 3** |  **The detection process** |    |    |
|  |  1. The detection process  |  [Slides](https://peter.solymos.org/qpad-workshop/day3-1-intro.pdf)  | [Video](https://youtu.be/CkdYEF_hZqY) |
|  |  2. Distance sampling and density |  [Notes](https://peter.solymos.org/qpad-workshop/day3-2-detection.html)  | [Video](https://youtu.be/x8GfKDEJcrA) |
|  |  3. Estimating population density |  [Notes](https://peter.solymos.org/qpad-workshop/day3-2-detection.html)  | [Video](https://youtu.be/yeoGxRQd6o0) |
|  |  4. Assumptions |  [Notes](https://peter.solymos.org/qpad-workshop/day3-2-detection.html)  | [Video](https://youtu.be/o0bx-vNCaL0) |
| **Day 4** |  **Coming full circle**  |    |    |
|  |  1. QPAD overview  |  [Slides](https://peter.solymos.org/qpad-workshop/day4-1-intro.pdf)  | [Video](https://youtu.be/TU9rcwY2Y-g) |
|  |  2. Models with detectability offsets  |  [Notes](https://peter.solymos.org/qpad-workshop/day4-2-offsets.html)  | [Offsets](https://youtu.be/vw_WO2hgNwk), [Models](https://youtu.be/Cy68E1GyNVU) |
|  |  3. Model validation and error propagation  |  [Notes](https://peter.solymos.org/qpad-workshop/day4-2-offsets.html)  | [Validation](https://youtu.be/lRcJzfE838k), [Error](https://youtu.be/na5cTYNq2HM) |
|  |  4. Recordings, roadsides, closing remarks  |  [Notes](https://peter.solymos.org/qpad-workshop/day4-3-recordings.html)  | [Video](https://youtu.be/ckEDGdLA_J4) |


## Before the course

Follow the instructions at the [R website](http://cran.r-project.org) to download and install the most up-to-date base R version suitable for your operating system (the latest R version at the time of writing these instructions is 4.0.4).

Then run the following script in R:

```R
source("https://raw.githubusercontent.com/psolymos/qpad-workshop/main/src/install.R")
```

Having RStudio is not absolutely necessary, but it will make life easier. RStudio is also available for different operating systems. Pick the open source desktop edition from [here](http://www.rstudio.com/products/rstudio/download/) (the latest RStudio Desktop version at the time of writing these instructions is 1.4.1106).

Prior exposure to R programming is not necessary, but knowledge of basic R object types and their manipulation (arrays, data frames, indexing) is useful for following hands-on exercises. Software Carpentry's [Data types and structures in R](http://swcarpentry.github.io/r-novice-inflammation/13-supp-data-structures/index.html) is a good resource to brush up your R skills.

## During the course

The course will be delivered online using Zoom. The course will be recorded with the intention of editing the material into a series of video tutorials in the future. Camera on is not required, but is encouraged when engaging in live discussions.

We will keep course related conversation and questions in the following collaborative markdown file: [https://hackmd.io/@psolymos/qpad-2021](https://hackmd.io/@psolymos/qpad-2021) Please scroll down to the Parking Lot section to add your ideas and questions.

### Get course materials

I might make last minute changes, so it is recommended to update your files before the sessions.

If you don't want to use git:

1. Visit [https://github.com/psolymos/qpad-workshop/releases](https://github.com/psolymos/qpad-workshop/releases)
2. Download the latest release into a folder
3. Extract the zip/tar.gz archive
4. Open the `workshop.Rproj` file in RStudio (or open any other R GUI/console and `setwd()` to the directory where you downloaded the file)
5. (You can delete the archive)

If you want to use git: fork or clone the repository

```bash
cd into/your/dir
git clone https://github.com/psolymos/qpad-workshop.git
```

To avoid conflicts as we update the workshop material: work in a LOCAL copy of the R markdown files

```R
source("src/functions.R")
qpad_local(day=1)
```

LOCAL copies will not be tracked and overwritten by git.

## After the course

Expect some follow up :)

## References

Sólymos, P., Toms, J. D., Matsuoka, S. M., Cumming, S. G., Barker, N. K. S., Thogmartin, W. E., Stralberg, D., Crosby, A. D., Dénes, F. V., Haché, S., Mahon, C. L., Schmiegelow, F. K. A., and Bayne, E. M., 2020. Lessons learned from comparing spatially explicit models and the Partners in Flight approach to estimate population sizes of boreal birds in Alberta, Canada. _Condor_, 122: 1-22. [PDF](https://drive.google.com/file/d/115WgtPd4zUSIFfSTHbWYs8OCHNdpKkh5/view?usp=sharing) 

Sólymos, P., Matsuoka, S. M., Cumming, S. G., Stralberg, D., Fontaine, P., Schmiegelow, F. K. A., Song, S. J., and Bayne, E. M., 2018. Evaluating time-removal models for estimating availability of boreal birds during point-count surveys: sample size requirements and model complexity. _Condor_, 120: 765-786. [PDF](https://drive.google.com/file/d/13Czd_A82P0ZhIlvAEabxdHfmaZcJaNU3/view?usp=sharing)

Sólymos, P., Matsuoka, S. M., Stralberg, D., Barker, N. K. S., and Bayne, E. M., 2018. Phylogeny and species traits predict bird detectability. _Ecography_, 41: 1595-1603. [PDF](https://drive.google.com/file/d/1CRKl-bh1tqxddijEWZoNcDO_xFIgOfWZ/view?usp=sharing)

Van Wilgenburg, S. L., Sólymos, P., Kardynal, K. J. and Frey, M. D., 2017. Paired sampling standardizes point count data from humans and acoustic recorders. _Avian Conservation and Ecology_, 12(1):13. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPOTZyTXlDb0xFQTA/view?usp=sharing)

Yip, D. A., Leston, L., Bayne, E. M., Sólymos, P. and Grover, A., 2017. Experimentally derived detection distances from audio recordings and human observers enable integrated analysis of point count data. _Avian Conservation and Ecology_, 12(1):11. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPQ2F6d1llQ3lPTzg/view?usp=sharing)

Sólymos, P., and Lele, S. R., 2016. Revisiting resource selection probability functions and single-visit methods: clarification and extensions. _Methods in Ecology and Evolution_, 7:196-205. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPRE5tVlRMSmhLWmM/view?usp=sharing)

Matsuoka, S. M., Mahon, C. L., Handel, C. M., Sólymos, P., Bayne, E. M., Fontaine, P. C., and Ralph, C. J., 2014. Reviving common standards in point-count surveys for broad inference across studies. _Condor_ 116:599-608. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPcGZNS3JSRUlBdDQ/view?usp=sharing)

Sólymos, P., Matsuoka, S. M., Bayne, E. M., Lele, S. R., Fontaine, P., Cumming, S. G., Stralberg, D., Schmiegelow, F. K. A. & Song, S. J., 2013. Calibrating indices of avian density from non-standardized survey data: making the most of a messy situation. _Methods in Ecology and Evolution_ 4:1047-1058. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPV0RNUFU1N1dmS1E/view?usp=sharing)

Matsuoka, S. M., Bayne, E. M., Sólymos, P., Fontaine, P., Cumming, S. G., Schmiegelow, F. K. A., & Song, S. A., 2012. Using binomial distance-sampling models to estimate the effective detection radius of point-counts surveys across boreal Canada. _Auk_ 129:268-282. [PDF](https://drive.google.com/file/d/0B-q59n6LIwYPbFhhRUtZNWQyMk0/view?usp=sharing)

## License

The course material is licensed under [Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) license. Source code is under [MIT](LICENSE) license.
