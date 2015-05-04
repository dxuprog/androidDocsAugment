## Augmenting Android Documentation with example code usages from StackOverflow

![alt tag](https://raw.github.com/dxuprog/androidDocsAugment/master/screenshot2.png)

This is a script to be used with the TaperMonkey Chrome-Plugin that will augment official Android Documentation with code usage examples from StackOverflow.

Official Android Documentation is somewhat lacking in code usage examples. This tool aims to fill in this information gap by providing links to relevant code usage examples based on the Android class being browsed.

When browsing Android Documentation, the tool extracts the Android Class in question, and injects in-line links to StackOverflow questions that have code snippets using that Android Class. The tool provides links sorted by complexity, which is a <b>tf-idf weighted</b> score defined by the number of different Fully Qualified Names (FQNs) that are used in the snippet. A low non-zero complexity means the snippet contains very few FQNs and is mostly made up of the FQN in question. While a high complexity means the snippet contains many different FQNs in addition to the one in question. This allows the user to pick how 'detailed' their example will be.

This work is outlined in section 5.0 in the whitepaper: [a relative link](androidDocsAugmentWhitePaper.pdf)

The FQN extraction process is the work of Subramanian et al.: http://dl.acm.org/citation.cfm?id=2568313

## Installation

## Usage

