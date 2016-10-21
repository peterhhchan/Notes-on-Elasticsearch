# Notes-on-Elasticsearch
These are my notes as an Elasticsearch newbie.  

Elasticsearch is a search engine, not a database.  Documents in elasticsearch can be lost, so do use a permanent store to backup your documents. 

https://qbox.io/blog/optimizing-elasticsearch-how-many-shards-per-index

Nodes:  An Elasticsearch server

Cluster: A group of of nodes form an Elasticsearch cluster

Index: A collection of documents.

Shard: A Lucene index.  

[How many shards should Elasticsearch indexes have?] (http://cpratt.co/how-many-shards-should-elasticsearch-indexes-have/)
Quick answer:  One for each node.  

http://stackoverflow.com/questions/22544461/elasticsearch-optimal-number-of-shards-per-node

The optimal number of shards per index is 1.
The optimal number of shards per node is 1.

## Elasticsearch Best Practices

* Heap Size
  https://www.elastic.co/guide/en/elasticsearch/guide/current/_limiting_memory_usage.html

  Set your heap size to a maximum of 32 GB, and no more than 50% of your RAM.
  
* Avoiding [split-brain](http://blog.trifork.com/2013/10/24/how-to-avoid-the-split-brain-problem-in-elasticsearch/) problem

* Don't store the seconds and milliseconds in the date if you don't need it.

* [Rename] (http://logz.io/blog/the-top-5-elasticsearch-mistakes-how-to-avoid-them/) your production cluster to prevent other nodes from joining it :p.  

Sources:
https://www.quora.com/What-are-some-good-practices-when-using-Elasticsearch
