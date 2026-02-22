# Penetration Testing

## 功能
- 自动执行任务
- 提供专业建议
- 生成优化方案

## Metadata
- **Category**: Offensive Security
- **Difficulty**: Intermediate to Advanced
- **Prerequisites**: 
  - Networking fundamentals (TCP/IP, DNS, HTTP/S)
  - Operating systems (Linux/Windows)
  - Basic programming/scripting
  - Understanding of common vulnerabilities
- **Tools Commonly Used**: Nmap, Burp Suite, Metasploit, Wireshark, John the Ripper, Hydra, sqlmap
- **Certifications**: OSCP, GPEN, CEH, PNPT
- **Ethical Considerations**: Always have written authorization, respect scope, protect data

## Practical Skill Development Path

### Phase 1: Foundation & Reconnaissance
**Objective**: Learn legal frameworks and passive information gathering.

**Practical Exercises**:
1. **Legal Documentation Practice**
   - Draft a sample penetration testing agreement
   - Create scope of work templates
   - Practice writing rules of engagement

2. **Passive Reconnaissance**
   - Use OSINT tools on your own domain (with permission):
     - `theHarvester` for email/domain discovery
     - `Maltego` for relationship mapping
     - Shodan/Censys searches for exposed services
   - Practice Google dorking on test sites:
     - `site:example.com filetype:pdf`
     - `inurl:admin site:example.com`

3. **Active Reconnaissance Basics**
   - Scan your home lab with Nmap:
     ```bash
     # Basic scan
     nmap -sV -O 192.168.1.0/24
     
     # Script scanning
     nmap -sC -sV target_ip
     
     # UDP scan (slower)
     nmap -sU -p 53,161 target_ip
     ```

### Phase 2: Vulnerability Assessment
**Objective**: Identify potential weaknesses systematically.

**Practical Exercises**:
1. **Service Enumeration**
   - Enumerate SMB shares:
     ```bash
     enum4linux target_ip
     smbclient -L //target_ip/
     ```
   - Enumerate web technologies"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":20,"completion_tokens":450,"total_tokens":470,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":20},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}


## 使用场景
本技能适用于需要帮助的用户，可应用于多种工作场景。

## 触发词
- /penetration-testing
- Penetration Testing
