# Database Design

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Category**: Data Engineering / Backend Development
- **Proficiency Levels**: Beginner → Intermediate → Advanced → Expert
- **Related Skills**: SQL, Data Modeling, System Design, Normalization, Performance Tuning
- **Common Tools**: ERD tools (Lucidchart, draw.io), SQL databases (PostgreSQL, MySQL), NoSQL databases (MongoDB, Redis)
- **Typical Applications**: Web applications, enterprise systems, data warehouses, real-time systems

## Practical Knowledge

### Core Concepts
**Entities and Relationships**: Identify real-world objects (entities), their attributes, and how they connect (one-to-one, one-to-many, many-to-many).

**Normalization**: Eliminate data redundancy through normal forms (1NF, 2NF, 3NF, BCNF). Know when to denormalize for performance.

**Keys and Constraints**: Primary keys (natural vs. surrogate), foreign keys, unique constraints, check constraints.

**Indexing Strategy**: Understand B-tree, hash, and specialized indexes. Know what to index (frequently queried columns) and what to avoid (frequently updated columns).

### Practical Patterns
**Starter Template for Common Relationships**:
```sql
-- One-to-Many (e.g., User → Posts)
CREATE TABLE users (id SERIAL PRIMARY KEY, email VARCHAR UNIQUE);
CREATE TABLE posts (id SERIAL PRIMARY KEY, user_id INT REFERENCES users(id));

-- Many-to-Many (e.g., Students ↔ Courses)
CREATE TABLE students (id SERIAL PRIMARY KEY);
CREATE TABLE courses (id SERIAL PRIMARY KEY);
CREATE TABLE enrollments (
    student_id INT REFERENCES students(id),
    course_id INT REFERENCES courses(id),
    PRIMARY KEY (student_id, course_id)
);

-- Hierarchical (e.g., Category tree)
CREATE TABLE categories (
    id SERIAL PRIMARY KEY,
    parent_id INT REFERENCES categories(id),
    name VARCHAR
);
```

**Performance Checklist**:
- Use `EXPLAIN ANALYZE` on slow queries
- Add composite indexes for multi-column filters
- Consider partitioning for large tables (>10M rows)
- Set appropriate `VARCHAR"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":18,"completion_tokens":450,"total_tokens":468,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":18},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /database-design
- Database Design
