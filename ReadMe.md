    ## Code for the manuscript ``Partition MCMC for inference on acyclic digraphs''
    #
    ## Jack Kuipers and Giusi Moffa
    ## ETH
    #
    ## Last modified: April 19, 2015
    #
    ## Disclaimer: The code in this archive is not guaranteed to be optimised or free of bugs.
    ##        Please report any issues to the authors (jack.kuipers@bsse.ethz.ch and giusi.moffa@gmail.com).

* * * * *

The R files in the main directory run the various MCMC schemes for
simulated and real data as follows:

`simpleexample.R` runs a small example on three nodes where the score is
proportional to the number of edges in the DAG

`smallsimmain.R` runs a simulated example with 5 nodes and the BGe score

The plots resulting from running the R files are stored in the
corresponding directory with `graphs` appended after the identifier.

In the `runningexamples` directory, knitr code and the output pdf files
for both these small examples are provided.

`BHmain.R` runs an example with the Boston Housing data with 14 nodes
and the BGe score.

`medsimmain.R`, “largesimmain.R” and “largersimmain.R” run larger
simulated examples with 14, 18 and 20 nodes respectively.

The underlying MCMC codes are stored in the directories
`edgerevandstructure` and `orderandpartition` respectively with the
`initialisation` and `scoring` codes in those directories.

To change the scoring for DAGs, the `DAGcorescore` function, for example
in `scoring/numedgescore.R` can be modified to any function of the
parent nodes.
