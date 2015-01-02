Requirements
============

Install s3cmd via:

```
sudo apt-get install s3cmd

s3cmd --configure
```
Proceed with your aws information

Install Hanzo warc tools as detailed here: http://code.hanzoarchives.com/warc-tools/wiki/Home


Background
==========

The Common crawl corpus (www.commoncrawl.org) is a non-profit a digital archive of "snapshots" of the web.   

query_wet_news
==============

Looking through the common crawl archives news entries


Parallelization strategy
========================

Currently prototyping Map-Reduce principles using BASH fork. 
For example:

```

./CycleThroughFilterShuf.sh & ./CycleThroughFilterShuf.sh ... 

```

![Program execution sequence](https://github.com/andrewdefries/query_wet_news/blob/master/ParallelBatch.png "Breakdown of Program execution sequence")
