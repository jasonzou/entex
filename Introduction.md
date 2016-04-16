# Motivation #

Timex recognition has been attempted with both rule-based and ML-based approaches, and both work reasonably well.

However, it's clear that to solve the timex normalisation problem, we need some rule set.

It's also clear that many researchers have built rule-based normalisation system and achieved high - but not complete - resolution.


We can build a framework for a modular community tool for timex extraction and normalisation, and achieve vastly higher performance than seen at either Tempeval challenge. Our goal is to enable and encourage our community to work on these problems, through the creation and maintenance of an open-source project.

# Plan #

Acquire a codebase that's modular and can be extended in the way we wish. Possible candidates that fit these criteria are:
  * HeidelTime (entrant in Tempeval-2, UIMA component)
  * TERNIP (structured Python re-write of GUTime, GATE component)

Create a testing architecture for both extraction and normalisation, that reports on:
  * Timex recognition rates
  * Per-rule and overall timex normalisation accuracy
  * Timex partial matching in cases where the timex is normalised overlapping but not matching the gold standard

Expand the amount of TIMEX annotated literature

Grow the rulebase:
  * First, include all rules from existing published / open projects
  * Secondly, improve performance through error analysis

Improve recognition, through rule tweaks and the inclusion of a trainable BIO tagger.

# References #

  * [HeidelTime](http://dbs.informatik.uni-heidelberg.de/fileadmin/Team/jannik/StroetgenGertz2010_semeval.pdf)
  * [Tempeval-2](http://www.timeml.org/tempeval2/)
  * [TERNIP](http://svn.pling.org.uk/ternip/trunk/docs/dissertation.pdf)