---
title: "WORT: Write Optimal Radix Tree for Persistent Memory Storage Systems"
collection: publications
permalink: /publication/fast17
venue: 'The 15th USENIX Conference on File and Storage Technology (FAST 2017)'
date: 2017-02-27
citation: '<strong>Se Kwon Lee</strong>, K. Hyun Lim, Hyunsub Song, Beomseok Nam, and Sam H. Noh. In Proceedings of <i>the 15th USENIX Conference on File and Storage Technology</i> (<strong>FAST 2017</strong>).'
---
[[pdf]](http://sekwonlee.github.io/files/fast17.pdf)

## Abstract
Recent interest in persistent memory (PM) has stirred development of index structures that are efficient in PM. Recent such developments have all focused on variations of the B-tree. In this paper, we show that the radix tree, which is another less popular indexing structure, can be more appropriate as an efficient PM indexing structure. This is because the radix tree structure is determined by the prefix of the inserted keys and also does not require tree rebalancing operations and node granularity updates. However, the radix tree as-is cannot be used in PM. As another contribution, we present three radix tree variants, namely, WORT (Write Optimal Radix Tree), WOART (Write Optimal Adaptive Radix Tree), and ART+CoW. Of these, the first two are optimal for PM in the sense that they only use one 8-byte failure-atomic write per update to guarantee the consistency of the structure and do not require any duplicate copies for logging or CoW. Extensive performance studies show that our proposed radix tree variants perform considerable better than recently proposed B-tree variants for PM such NVTree, wB+Tree, and FPTree for synthetic workloads as well as in implementations within Memcached.
