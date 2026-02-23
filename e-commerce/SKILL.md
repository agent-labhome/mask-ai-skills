# E Commerce

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Domain**: E-commerce
- **Complexity Level**: Intermediate to Advanced
- **Prerequisites**: Web development fundamentals, database knowledge, payment systems understanding
- **Key Technologies**: React/Vue/Angular, Node.js/Python/Django, PostgreSQL/MongoDB, Stripe/PayPal, AWS/GCP
- **Time Investment**: 3-6 months for full implementation
- **Market Demand**: High (continuous growth in online retail)

## Core Competencies

### 1. Platform Architecture
**Essential Knowledge:**
- Monolithic vs. Microservices architecture
- Headless commerce vs. traditional platforms
- API-first design principles
- Database design for e-commerce (products, users, orders, inventory)
- Caching strategies (Redis, CDN, browser caching)

**Practical Implementation:**
```javascript
// Example: Basic e-commerce schema structure
const ecommerceSchema = {
  products: {
    id: 'UUID',
    sku: 'String',
    name: 'String',
    description: 'Text',
    price: 'Decimal',
    inventory: 'Integer',
    categories: ['Array'],
    attributes: {Object},
    images: ['Array'],
    variants: ['Array']
  },
  users: {
    id: 'UUID',
    email: 'String',
    password_hash: 'String',
    addresses: ['Array'],
    payment_methods: ['Array'],
    order_history: ['Array']
  },
  orders: {
    id: 'UUID',
    user_id: 'Reference',
    items: ['Array'],
    total: 'Decimal',
    status: 'String',
    shipping_address: 'Object',
    payment_status: 'String'
  }
};
```

### 2. Product Management System
**Key Features to Implement:**
- Product catalog with filtering and search
- Inventory management with real-time updates
- Product variants (size, color, etc.)
- Categories and tags system
- Bulk import/export capabilities

**Code Example - Product Filtering:**
```javascript
class ProductFilter {
  constructor(products) {
    this.products = products;
  }

  filterByCategory(categoryId) {
    return this.products.filter(product => 
      product.categories.includes(categoryId)
    );
  }

  filterByPriceRange(min, max) {
    return this.products.filter(product => 
     "},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":20,"completion_tokens":500,"total_tokens":520,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":20},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /e-commerce
- E Commerce

## 使用示例
请提供具体需求，我将为你生成结果。

## 定价参考
- 基础版: $19
- 专业版: $49
