-e {"id":"9e560a01-c4a9-4971-8b80-5c8b5cbdf6f1","object":"chat.completion","created":1771642486,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL: SQL

## Metadata
- **Category**: Data & Databases
- **Prerequisites**: Basic computer literacy, logical thinking
- **Difficulty**: Beginner to Advanced
- **Time to Basic Proficiency**: 2-4 weeks
- **Common Tools**: PostgreSQL, MySQL, SQLite, Microsoft SQL Server, Oracle Database, DBeaver, pgAdmin, DataGrip
- **Key Paradigms**: Declarative programming, Set theory, Relational algebra

## Overview
SQL (Structured Query Language) is a domain-specific language for managing and querying relational databases. It enables you to create, read, update, and delete data while maintaining data integrity through constraints, transactions, and relationships.

## Core Concepts

### 1. **Fundamental Operations (CRUD)**
- **CREATE**: `INSERT INTO table VALUES (...)`
- **READ**: `SELECT columns FROM table WHERE conditions`
- **UPDATE**: `UPDATE table SET column = value WHERE conditions`
- **DELETE**: `DELETE FROM table WHERE conditions`

### 2. **Data Definition Language (DDL)**
```sql
CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(255) UNIQUE,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

ALTER TABLE users ADD COLUMN age INT;
DROP TABLE users;
```

### 3. **Data Querying Essentials**
```sql
-- Basic SELECT with filtering
SELECT name, email FROM users 
WHERE age > 18 
ORDER BY name ASC
LIMIT 10;

-- Aggregation
SELECT 
    department,
    COUNT(*) as employee_count,
    AVG(salary) as avg_salary
FROM employees
GROUP BY department
HAVING COUNT(*) > 5;
```

### 4. **Joins (Relational Power)**
```sql
-- INNER JOIN: Matching records only
SELECT orders.id, customers.name, orders.total
FROM orders
INNER JOIN customers ON orders.customer_id = customers.id;

-- LEFT JOIN: All from left table, matches from right
SELECT employees.name, departments.name as department
FROM employees
LEFT JOIN departments ON employees.dept_id"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":17,"completion_tokens":450,"total_tokens":467,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":17},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
