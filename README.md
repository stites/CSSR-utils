This directory contains the various Perl scripts written over the years to work
with CSSR. All work was written by Cosma Shalizi, current maintainer is Sam
Stites <sam@stites.io>

Directory contents (alphabetically):
- bic-selector.pl does model selection, on the history length, using BIC
  and a fixed significance level.  Calls likelihood-under-CSM.pl.
- bic-selector-with-alpha.pl expands the model search to also search over
  the significance level alpha.
- bic-selector-with-siglevel-and-entropy.pl was supposed to use some
  entropy estimation to improve the range of candidate history lengths,
  but otherwise work like bic-selector-with-alpha.pl.  Sound idea, never
  finished execution.
- CSSRfilter.pl is a wrapper for using CSSR as a STDIN/STDOUT filter.
- empirical-error-of-HMM.pl calculates error measures for an inferred
  machine's performance on a binary time series.
- inferred-versus-true.pl compares an inferred machine to a generating
  machine, with the format given by those of the test-machine programs.
- inferred-versus-true-alt-version.pl is another version of the same
  program which I found living in another directory.  Unfortunately, due to the
  way I recovered from back-up after a hard disk crash some years ago, they
  now have the same date, and I'm not sure which one is actually more recent.
- likelihood-under-CSM.pl calculates the (log) likelihood of a time series
  under an inferred state machine.
- multifile-bic-selector.pl is a wrapper for running bic-selector.pl on many
  files with structured names.
- mulitple-inference.pl is a wrapper for running CSSR (with identical
  arguments) on many files with repetitive names.
- sns-inferred-vs-true.pl is like inferred-vs-true.pl, but for a special
  true machine, the "simple nondeterministic source".
- update-machine-probs.pl uses an observed time series to update the
  transition probabilities of an already-inferred machine.

See also the test-machines directory, which should accompany this.
