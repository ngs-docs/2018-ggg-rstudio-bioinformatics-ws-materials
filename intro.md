# Intro to data analysis in the UNIX shell and with R

C. Titus Brown, ctbrown@ucdavis.edu

## Front matter

Please adhere to the [Carpentries Code of Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html). Two key points:

* this isn't a venue to show off your own experience
* this isn't a dating scene

### Venue information

Bathrooms are just outside! Water is around the corner in the kitchen! Elevator is in the corner outside the side door!

### Recording

**Note** that this will be recorded and made available to others; probably only audio from the audience. Please let me know if you need something removed from the audio, thanks!

### Introduction and thoughts

Hi! I'm Titus, I'm a prof here, I do a lot of data analysis :).

This ~3 hour workshop is meant to show you how most research data analysis workflows work, in my experience; and especially how we connect significant computing at the command line to data exploration and analysis in R.

The only way you'll really learn to do all of this is by applying it to your own research and spending time on it :).

### Rough schedule

9 - 10:15 - command line and BLAST
10:15-10:30 - break
10:30 - noon - R and RStudio

### More resources on campus

The UC Davis [Data Science Initiative](http://dsi.ucdavis.edu/) offers [workshops](http://dsi.ucdavis.edu/workshops.html)!

The UC Davis bioinformatics core has a [training program](https://bioinformatics.ucdavis.edu/training/)!

The [Davis R Users Group](https://d-rug.github.io/) is a great resource for R!

My lab runs regular [office hours, called Meet and Analyze Data](https://dib-training.readthedocs.io/en/pub/#meet-and-analyze-data-mad) on Wednesday afternoon.

[Check out DIBSI](http://ivory.idyll.org/dibsi/), which is a set of summer workshops that my lab runs. (Not yet announced for 2019, but it will be July 1-July 12).

## Workshop materials

First, click on the "launch binder" button, below. This will launch RStudio.

[![Binder](http://mybinder.org/badge.svg)](http://beta.mybinder.org/v2/gh/ngs-docs/2018-ggg-rstudio-bioinformatics-ws/master?urlpath=rstudio)

Then, [start here, with command-line BLAST](https://github.com/ngs-docs/2018-ggg-rstudio-bioinformatics-ws-materials/blob/master/running-command-line-blast.md).

[Continue here, with visualizing BLAST scores](https://github.com/ngs-docs/2018-ggg-rstudio-bioinformatics-ws-materials/blob/master/visualizing-blast-scores-with-RStudio.md)

### Extra: create an R script

(if we have time)

## Other links

[The binder repository source](https://github.com/ngs-docs/2018-ggg-rstudio-bioinformatics-ws/)

Globbing: https://en.wikipedia.org/wiki/Glob_(programming)

To get the zebrafish TSV file that is the output of the command line BLAST section do:
```
curl -L -o mm-second.x.zebrafish.tsv https://osf.io/svprg/download
```

Ghetto data analysis:
```
blast_out$ratio <- blast_out$bitscore / (blast_out$pident  * (blast_out$qend - blast_out$qstart))
hist(blast_out$ratio)
```

## Key summary points

* Do "big (automated) compute" and large file manipulations at the command line!
* Do data set exploration, plotting, and statistical analysis in R.
* Record your commands!

