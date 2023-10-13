# BTE TRAPI Results Summary

Goal: Make a diff-able report for a BTE TRAPI results file.

We observed variability between identical BTE queries via the Benchmarks tool. The notebook helps organize the information we thought to be useful for figuring out where differences are occuring, as to focus our efforts for finding the source of this variability. It also details an example analysis on two inconsistent BTE results files (included in this repository).

TRAPI results summary follows this format:

```
== SUMMARY STATS ==
# nodes
# edges
# results
# auxiliary graphs

== LOG ==
Errors:

Execution Summaries:
ex. "Execution Summary: (514) nodes / (1758) edges / (500) results; (37/149) queries returned results from (6) unique APIs"

== INFORES == 
infores:abc: count
infores:lmn: count
infores:xyz: count
ex. infores:semmeddb: 341

== SCORES ==
node1_id-node2_id: score
node3_id-node4_id: score
ex. PUBCHEM.COMPOUND:448601-MONDO:0020479: 0.9965088294560911
```
