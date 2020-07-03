# Ensemble
# Language: Python
# Input: TXT
# Output: CSV (correlations)
# Tested with: PluMA 1.0, Python 3.6
# Dependency: sparcc, numpy==1.16.0

PluMA plugin that computes correlations using an ensemble (Weiss et al, 2016) approach
involving Pearson, Spearman and SparCC (Freidman, 2012) correlations.

The plugin accepts as input a TXT file of counts with columns representing samples.
Entry (i, j) corresponds to the abundance of variable i in sample j.  The output CSV
file will contain correlations computed using the ensemble approach, with entry
(i, j) representing the computed correlation between variable i and variable j.

Note: The source code for SparCC, contained within the sparcc/ directory, was obtained
open source from BitBucket at the following location:
https://bitbucket.org/yonatanf/sparcc

The example/ directory also contains one of their examples, fake_data.txt.  This can
also be used to test the Ensemble plugin with PluMA.



