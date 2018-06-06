# ReproAnalysisTools

Organizing thoughts on tools and approaches for reproducible analyses

## Many Approaches:

- "Good Enough Practices in Scientific Computing"
- "Excuse Me, Do You Have a Minute To Talk About Version Control"
- Ben Marwick `rrtools`
- Will Landau `drake`
- ropensci unconf summary google doc from Hadley
- Jenny Bryan: "What They Forgot to Teach You" rstudioconf 2018 tutorial
- Jenny Bryan: "Workflow vs. Script" blog post

## Components

- raw data (local/git-tracked, remote/untracked)
- intermediate data/results (.rda/.rds, .csv, .drake cache)
- dependencies (package DESCRIPTION file, NAMESPACE, roxygen imports, docker)
- outputs/reports (Rmarkdown, drake, )
- invalidating pieces (git, drake, human memory)
- run the whole thing (make, analysis.R, knit the Rmd)
- minimizing re-done work (pipeline mgmt: drake, remake, make)
- testing

## Features

- user experience: clone/download v. install
- low barrier to entry (e.g., can use just a little)
- developer-side usage only (e.g., usethis)
- authentication/private user setup
- menus / interaction

## Ideas

- my instinct is to have a friendly script that starts up by checking if necessary packages are installed, and asking the user to install

## Questions

- How do you test analysis results? Does there need to be example data in testthat folder? Can it access drake cache?
- 






