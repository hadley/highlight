# highlight (development version)

# highlight 0.5.2

* Remove C++11 requirement

# highlight 0.5.1

* Fix R CMD check failure

# highlight 0.5.0

* highlight has been un-orphaned; it won't be resuming active development,
  but I will keep it alive on CRAN in the future.

# highlight 0.4.5

* Abandon highlight.httpd.handler.

# highlight 0.4.2

* Dealing with spaces that were inserted where they should not have. Reported
  by Yihui Xie.
* Removing the last line from highlighted code chunks in the sweave driver.
  Requested by Dirk Eddelbuettel.
* Supporting VignetteBuilder: highlight.

# highlight 0.4.1

* Using sprintf instead of snprintf (for solaris).

# highlight 0.4.0

* Eliminated dependency on Rcpp and parser.
* Depends on R 3.0.0 (needed for getParseData).

# highlight 0.3.2

* highlight gains the show_line_numbers argument. Suggestion by Yihui Xie.
* The Sweave driver gains a `<<file=>>` option to highlight the content
  of a file.
* The latex renderer created a global variable "txt", reported by Yihui Xie.

# highlight 0.3.1

* Bug fix in the html renderer. Thanks to @tonybreyal for pointing out
  the bug on twitter.

# highlight 0.3.0

* Using sprintf instead of snprintf to make Solaris happy.
* New R function external_highlight that uses the C++ code from Andre
  Simon highlight library. The code is called directly, no more using a system
  dependency as before.

# highlight 0.2-6

* Small bug fixed in the latex renderer. Reported by Collin Gillepsie.

# highlight 0.2-5

* Superfluous lines were added at the end of code chunks in the sweave driver.
* Multiple lines character strings were not rendered properly by the
  latex renderer.

# highlight 0.2-3

* Sweave blocks now respond to the size option, as in:
  `<<size=footnotesize>>=` and adapts the generated latex code accordingly.

# highlight 0.2-1

* Sweave code chunks can set prompt=FALSE to remove the prompt and continue
  prompt: `<<eval=FALSE,prompt=FALSE>>=`.

# highlight 0.2-0

* The sweave driver accepts argument boxes, bg and border to control
  the appearance of the R code chunks.
* The sweave driver interprets code chunks like `<<lang=foo>>=` as source
  code in language foo and uses highlight (http://www.andre-simon.de/)
  to render the code if available.

# highlight 0.1-9

* The latex renderer header added useless information.
* The latex renderer gains a "minipage" argument that is passed
  down to header and footer to include the resulting highlighted code
  in a minipage environment.

# highlight 0.1-8

* Custom http handler to handle http request of the prefix
  /custom/highlight/fun or /custom/highlight/package/fun.

# highlight 0.1-6

* Fixed latex rendering (initial line of input and output) was indented.

# highlight 0.1-5

* Fixed handling of prompts.
* Added an example of how to debug a renderer. Suggestion by Gabor Grothendieck.
* 'highlight' now tests that parser.output is of class 'parser' to prevent
  uses of the 'parse' function in place of 'parser'. Suggestion by
  Hadley Wickham.

# highlight 0.1-3

* All headers and footers now include line feeds.
* Headers and footers can now be NULL (no content).

# highlight 0.1-2

* Initial release.
