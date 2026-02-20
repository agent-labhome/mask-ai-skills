-e # NoSQL

{"id":"3c48f447-9ae9-42f9-8aff-5ccb125d0b0e","object":"chat.completion","created":1771590817,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL.md: NoSQL

## Core Concepts
- **Non-relational databases** designed for scalability, flexibility, and specific data models
- **Schemaless design** (dynamic schemas) vs rigid SQL table structures
- **Horizontal scaling** (distributed systems) over vertical scaling
- **BASE properties** (Basically Available, Soft state, Eventual consistency) vs ACID

## Major Categories
1. **Document Stores** (MongoDB, CouchDB)
   - JSON/BSON documents with nested structures
   - Collections instead of tables
   - Rich querying capabilities

2. **Key-Value Stores** (Redis, DynamoDB, Riak)
   - Simple data model: key → value
   - High performance for simple lookups
   - Often used for caching, sessions

3. **Column-Family Stores** (Cassandra, HBase)
   - Tabular format with flexible columns per row
   -"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":15,"completion_tokens":200,"total_tokens":215,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":15},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
