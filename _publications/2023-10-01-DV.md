---
title: "Same or Different? Diff-Vectors for Authorship Analysis"
collection: publications
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'A paper about diff-vectors'
date: 2009-10-01
venue: 'ACM Transactions on Knowledge Discovery from Data'
paperurl: 'http://AlexMoreo.github.io/files/DV-TKDD.2023.pdf'
citation: 'Corbara, S., Moreo, A., & Sebastiani, F. (2023). Same or different? diff-vectors for authorship analysis. ACM Transactions on Knowledge Discovery from Data, 18(1), 1-36.'
---

In this article, we investigate the effects on authorship identification tasks (including authorship verification,
closed-set authorship attribution, and closed-set and open-set same-author verification) of a fundamental
shift in how to conceive the vectorial representations of documents that are given as input to a supervised
learner. In “classic” authorship analysis, a feature vector represents a document, the value of a feature rep-
resents (an increasing function of) the relative frequency of the feature in the document, and the class label
represents the author of the document. We instead investigate the situation in which a feature vector repre-
sents an unordered pair of documents, the value of a feature represents the absolute difference in the relative
frequencies (or increasing functions thereof) of the feature in the two documents, and the class label indi-
cates whether the two documents are from the same author or not. This latter (learner-independent) type of
representation has been occasionally used before, but has never been studied systematically. We argue that
it is advantageous, and that, in some cases (e.g., authorship verification), it provides a much larger quantity
of information to the training process than the standard representation. The experiments that we carry out
on several publicly available datasets (among which one that we here make available for the first time) show
that feature vectors representing pairs of documents (that we here call Diff-Vectors) bring about systematic
improvements in the effectiveness of authorship identification tasks, and especially so when training data are
scarce (as it is often the case in real-life authorship identification scenarios). Our experiments tackle same-
author verification, authorship verification, and closed-set authorship attribution; while DVs are naturally
geared for solving the 1st, we also provide two novel methods for solving the 2nd and 3rd that use a solver
for the 1st as a building block. The code to reproduce our experiments is open-source and available online.
