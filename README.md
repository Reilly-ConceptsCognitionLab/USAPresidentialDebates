
<!-- README.md is generated from README.Rmd. Please edit that file -->

# USAPresidentialDebates

<!-- badges: start -->
<!-- badges: end -->

<figure>
<img src="man/figures/nixon.jpeg" alt="Richard Nixon Peace Sign" />
<figcaption aria-hidden="true">Richard Nixon Peace Sign</figcaption>
</figure>

## Overview

This R data package loads a concatenated dataframe composed of two-party
US Presidential debate transcripts from 1960 to 2020. Each debate
transcript is delineated in a one-row per utterance format marked by a
distinct document_id (debate and year), candidate (e.g., REAGAN) and
turn#. <br/>

Each utterance is also marked with associated metadata regarding the
candidate (e.g. name, party) and the election outcome (e.g.,
party_winner). We initially compiled debate transcripts from the
Commission on Presidential Debates (debates.org). Since the debates were
widely televised and publicly available, the data are being distributed
under fair use (<https://www.copyright.gov/fair-use/>) in that their
intended use is for academic/scholarly research. We edited each raw
transcript to omit commentator questions and remarks (e.g., “What is the
most important issue facing the economy?”). We also ommitted
parenthetical transcription notes (e.g., \[…coughing\]). <br/>

Researchers are free to make use of this data for any purpose. However,
we optimized the format to pair with a companion package
(ConversationAlign) designed to analyze alignment between two
interlocutors. <br/>

## Installation

Install the development version of USAPresidentialDebates from
[GitHub](https://github.com/) by typing the following in your console or
script (make sure you have devtools installed):

``` r
install.packages("devtools")
devtools::install_github("Reilly-ConceptsCognitionLab/USAPresidentialDebates")
```

## Call the transcripts

Could not be more simple… call the library, then type the word debates.

``` r
library(USAPresidentialDebates)
str(debates)
```

## Get in touch!

Contact <jamie_reilly@temple.edu> for feedback and assistance.
