title: "Compiling Adv-r book"
author: "yuyu zhang"
date: "9/12/2020"


# download the book from website
git clone https://github.com/hadley/adv-r.git
# dowmload bookdown github repo as a zip file
https://github.com/rstudio/bookdown-demo

# the packages that needed to be downloade under the compiling
install.packages("lobstr")
devtools::install_github("hadley/emo")
install.packages("sloop")
install.packages("DBI")
install.packages("RSQLite")
install.packages("zeallot")
install.packages("dbplyr")
install.packages("profvis")
install.packages("bench")
install.packages("ggbeeswarm")
library(tinytex)
tlmgr_update()  

# Package fontspec Error: The font "Inconsolata" cannot be found

download the inconsolata from website and installed it.

# "make" is not found
download the Rtools from website and configure the environmental variables. update the rtools.
then install the package.
install.packges("make")

# LaTeX update
remotes::install_github('rstudio/rmarkdown')
update.packages(ask = FALSE, checkBuilt = TRUE)
tinytex::tlmgr_update()

# final step
Output created: _book/_main.pdf
