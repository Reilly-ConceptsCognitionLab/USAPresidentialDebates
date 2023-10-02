
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
candidate (e.g. name, party) election outcome (e.g., party_winner), and
various other statistics about the US in that debate year including:
<br/> 1) Democrat candidate age <br/> 2) Republican candidate age <br/>
3) Age difference between candidates <br/> 3) Inflatiion rate in the
year of the debate <br/> 4) GDP % change from prior year of debate <br/>

We edited each raw transcript to omit commentator questions and remarks
(e.g., “What is the most important issue facing the economy?”). We also
ommitted parenthetical transcription notes (e.g., \[…coughing\]). <br/>

We initially compiled debate transcripts from the Commission on
Presidential Debates (debates.org). Since each of the debates we
included were widely televised and publicly available, the data are
considered fair use (<https://www.copyright.gov/fair-use/>). That is,
their intended use is for academic/scholarly research. <br/>

Researchers are free to make use of this data for any purpose. We
optimized the format to work well with our companion R-package
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
