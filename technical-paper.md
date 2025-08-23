# Optimization Using Full Text Search
---
## Problem Statement 

Performance and scaling issue analysis via full text search approch

## Overview

A FTS is used while a system face issues while performing different actions on a large amount of text data. It allows us for more complex queryng and better matching.

## Possible solution

### 1. PostgreSQL with Elastic Search

- PostgreSQL is a Realtional database with support for complex queries and ACID compliance. 
- It can be used to store transactional data.
- Elasticsearch is a highly scalable, distributed search engine designed for fast full-text searching.
- It excels at handling large datasets and unstructured data, providing advanced features like fuzzy search, ranking, and faceted search.
- PostgreSQL into Elasticsearch can be used for fast, real-time search capabilities.

References :
- [PostgreSQL Full-Text Search](https://www.postgresql.org/docs/current/textsearch.html)
- [Elasticsearch Documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html)

### 2. Redis with RedisSearch 

- Redis is a fast, in-memory data store commonly used for caching, session management, and real-time applications.
- RedisSearch is build on lucene.
- RedisSearch extends Redis with advanced full-text search capabilities
- RedisSearch operates directly within Redis, providing a seamless integration for real-time.

References:
  - [RedisSearch Documentation](https://oss.redis.com/redisearch/)
  - [RedisSearch GitHub Repository](https://github.com/RedisLabs/RediSearch)

### 3. MongoDB with Solr

- MongoDB is a flexible, NoSQL document database that stores data in BSON (binary JSON) format.
- Solr provides full-text search capabilities, advanced indexing, and high scalability for document-oriented data.
- MongoDB is ideal for unstructured or semi-structured data, while Solr excels at providing fast search on large-scale text data.
- Solr can index the content of MongoDB documents, making it available for efficient searching.

References:

- [MongoDB and Solr Integration Guide](https://www.mongodb.com/blog/post/using-apache-solr-for-full-text-search-in-mongodb)
- [Solr with MongoDB](https://cwiki.apache.org/confluence/display/solr/MongoDB+Integration)

## Conclusion
Full-text search engines like Elasticsearch, Solr, and RedisSearch enhance database performance by enabling scalable, real-time, and advanced querying capabilities, optimizing search for large datasets and improving overall system responsiveness.

---