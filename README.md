## Augmenting Android Documentation with example code usages from StackOverflow

![alt tag](https://raw.github.com/dxuprog/androidDocsAugment/master/screenshot2.png)

This is a script to be used with the TaperMonkey Chrome-Plugin that will augment official Android Documentation with code usage examples from StackOverflow.

Official Android Documentation is somewhat lacking in code usage examples. This tool aims to fill in this information gap by providing links to relevant code usage examples based on the Android class being browsed.

When browsing Android Documentation, the tool extracts the Android Class in question, and injects in-line links to StackOverflow questions that have code snippets using that Android Class. The tool provides links sorted by complexity, which is a <b>tf-idf weighted</b> score defined by the number of different Fully Qualified Names (FQNs) that are used in the snippet. This allows the user to pick how 'detailed' their example will be.

The clusting scheme is outlined in section 5.0 in our [whitepaper](androidDocsAugmentWhitePaper.pdf).

The FQN extraction process is the work of [Subramanian et al](http://dl.acm.org/citation.cfm?id=2568313).

## Installation

1. Install the [TaperMonkey Chrome Extension](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)

2. Insert a new userscript into TaperMonkey and copy and paste in the [script](androidDocsAugment.js).

## Usage

1. With TaperMonkey enabled, navigate to any official Android Documentation, here is an [example](http://developer.android.com/reference/android/database/sqlite/SQLiteQueryBuilder.html).

## Contributors
David Xu (dxuprog) and Adriaan Labuschagne (adriaanlabusc).

Special thanks to Siddharth Subramanian (siddhukrs) et al. for development of Baker.