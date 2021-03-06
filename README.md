# london-hackday-2018
Notes and code for the London Lucene Hackday 2018

# Task 1: How can we build a command-line application for inspecting Lucene indexes? Some of these may be very large and use versions of Lucene from 4.x upwards. Considering various existing projects such as:
* Marple https://github.com/flaxsearch/marple
* Solr Chrome Debugger https://chrome.google.com/webstore/detail/solr-query-debugger/
* Quepid www.quepid.com
* Sense plugin for Elasticsearch https://www.elastic.co/guide/en/sense/current/installing.html
* Luke https://github.com/DmitryKey/luke
* Clue https://github.com/javasoze/clue
![whiteboard1](https://github.com/flaxsearch/london-hackday-2018/blob/master/IMAG2335.jpg)

# Task 2: Review Alessandro's various Lucene and Solr JIRA tickets:
* Bugs
* https://issues.apache.org/jira/browse/LUCENE-6687 More Like This Bug
* https://issues.apache.org/jira/browse/LUCENE-8329 Size Estimator Bug
* https://issues.apache.org/jira/browse/SOLR-12304 More Like This Bug Solr side

* Improvements
* https://issues.apache.org/jira/browse/LUCENE-8326 More Like This Params Refactor
* https://issues.apache.org/jira/browse/LUCENE-8347 BlendedInfixSuggester Improvement* 
* https://issues.apache.org/jira/browse/SOLR-12238 Synonym Query Style Boost By Payload
* https://issues.apache.org/jira/browse/SOLR-12243 Edismax Bug ( Elizabeth Haubert, me)

Reference for the Existing Bugs tracks:
* https://github.com/SeaseLtd/lucene-solr
Reference for how to contribute to Lucene/Solr:
* https://wiki.apache.org/lucene-java/HowToContribute
* https://wiki.apache.org/solr/HowToContribute

# Task3: Review issue 'Different Solr replicas give different result positions' from https://github.com/flaxsearch/london-hackday-2016 item 3 - what's the current state of play with this? *

* References: https://mail-archives.apache.org/mod_mbox/lucene-solr-user/201301.mbox/%3Czarafa.51006f06.0ea4.1386468330e702d7@mail.openindex.io%3E

* Here is our working branch: https://github.com/fguery/lucene-solr/tree/replicaChoice

* Useful command: cd solr/core ant test -Dtestcase=DistributedQueryComponentReplicaMarkerTest
