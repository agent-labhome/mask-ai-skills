# Ethical Hacking

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## 📋 Metadata
- **Category**: Cybersecurity / Offensive Security
- **Prerequisites**: Basic networking, Linux command line, programming fundamentals
- **Difficulty Level**: Intermediate to Advanced
- **Time to Proficiency**: 6-12 months with consistent practice
- **Legal Note**: Always practice on systems you own or have explicit permission to test

## 🎯 Core Competencies

### 1. **Reconnaissance & Information Gathering**
**Practical Skills:**
- **Passive Reconnaissance**: 
  - WHOIS lookups (`whois target.com`)
  - DNS enumeration (`dig`, `nslookup`, `dnsrecon`)
  - Subdomain discovery (`sublist3r`, `amass`, `crt.sh`)
  - Google Dorking techniques
  - Social media intelligence gathering

- **Active Reconnaissance**:
  - Network scanning with `nmap`:
    ```bash
    # Basic scan
    nmap -sS -sV -O target_ip
    
    # Full port scan
    nmap -p- -T4 target_ip
    
    # Script scanning
    nmap -sC -sV target_ip
    ```
  - Service fingerprinting
  - Banner grabbing with `netcat`:
    ```bash
    nc -nv target_ip 80
    ```

### 2. **Vulnerability Assessment**
**Practical Skills:**
- **Automated Scanning**:
  - Nessus/OpenVAS setup and scanning
  - Nikto for web server assessment:
    ```bash
    nikto -h http://target.com
    ```
  - WPScan for WordPress sites

- **Manual Testing**:
  - Version checking for known vulnerabilities
  - Configuration review
  - Default credential testing

### 3. **Exploitation**
**Practical Skills:**
- **Metasploit Framework**:
  ```bash
  msfconsole
  use exploit/windows/smb/ms17_010_eternalblue
  set RHOSTS target_ip
  exploit
  ```
  
- **Manual Exploitation**"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":450,"total_tokens":469,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /ethical-hacking
- Ethical Hacking
