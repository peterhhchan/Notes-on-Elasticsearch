# Notes-on-Elasticsearch
These are my notes as an Elasticsearch newbie.  

Elasticsearch is a search engine, not a database.  Documents in elasticsearch can be lost, so do use a permanent store for your documents. 

Nodes:  An Elasticsearch server
Cluster: A group of of nodes form an Elasticsearch cluster
Index: A collection of documents.
Shard: A Lucene index.  

[How many shards should Elasticsearch indexes have?] (http://cpratt.co/how-many-shards-should-elasticsearch-indexes-have/)
Quick answer:  One for each node.  

http://stackoverflow.com/questions/22544461/elasticsearch-optimal-number-of-shards-per-node
The optimal number of shards per index is 1.
The optimal number of shards per node is 1.
