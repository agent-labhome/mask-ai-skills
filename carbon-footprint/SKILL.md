-e {"id":"ead7821c-fe24-4a40-8bc6-6ee38b043a09","object":"chat.completion","created":1771652680,"model":"deepseek-chat","choices":[{"index":0,"message":{"role":"assistant","content":"# SKILL.md: Carbon Footprint

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Skill Name**: Carbon Footprint Calculator
- **Category**: Sustainability & Environmental Analytics
- **Complexity**: Intermediate
- **Use Case**: Business sustainability reporting, ESG compliance, supply chain analysis
- **Data Requirements**: Energy consumption, transportation logs, procurement data, waste metrics
- **Output Formats**: CO₂e metrics, compliance reports, reduction recommendations
- **Integration Points**: ERP systems, utility APIs, sustainability platforms (EcoVadis, CDP)

---

## Overview
The Carbon Footprint skill enables businesses to measure, analyze, and report greenhouse gas (GHG) emissions across Scopes 1, 2, and 3. It transforms operational data into actionable sustainability insights for compliance, reporting, and strategic decarbonization.

---

## Core Capabilities

### 1. **Emissions Calculation**
- **Scope 1 (Direct Emissions)**
  - Stationary combustion (boilers, furnaces)
  - Mobile combustion (company vehicles)
  - Process emissions (manufacturing, chemical reactions)
  - Fugitive emissions (refrigerants, methane leaks)

- **Scope 2 (Indirect Energy Emissions)**
  - Purchased electricity
  - Purchased steam, heating, and cooling
  - Market-based vs. location-based calculations

- **Scope 3 (Value Chain Emissions)**
  - Upstream: Purchased goods/services, capital goods, fuel/energy-related activities
  - Downstream: Transportation/distribution, product use, end-of-life treatment
  - Business travel, employee commuting, waste generation

### 2. **Data Processing Engine**
```
Input Data → Normalization → Emission Factors → Calculation → Validation → Reporting
```
- **Normalization**: Converts diverse units (kWh, liters, km) to standard measures
- **Emission Factors**: Integrates databases (EPA, DEFRA, IPCC, industry-specific)
- **Calculation Methods**: 
  - Spend-based (economic input-output)
  - Activity-based (physical units × emission factor)
  - Hybrid approaches for accuracy

### 3. **Reporting & Compliance**
- **Standards Alignment**: GHG Protocol, ISO 14064, GRI, SASB, TCFD
- **Automated Reporting**: CDP, SEC climate disclosures, EU CSRD
- **Visualization**: Emission hotspots, trend analysis, benchmarking

---

## Business Implementation Guide

"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":23,"completion_tokens":500,"total_tokens":523,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":23},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /carbon-footprint
- Carbon Footprint
