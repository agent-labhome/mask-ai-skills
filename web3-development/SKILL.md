# SKILL.md: Web3 Development

## Metadata
- **Category**: Software Development / Blockchain
- **Experience Level**: Intermediate to Advanced
- **Prerequisites**: 
  - JavaScript/TypeScript proficiency
  - Basic understanding of blockchain concepts
  - Familiarity with React/Node.js
  - Understanding of REST APIs
- **Related Skills**: Smart Contract Development, Decentralized Application Architecture, Cryptography, Distributed Systems
- **Tools**: Hardhat/Truffle, Ethers.js/web3.js, MetaMask, IPFS, The Graph
- **Ecosystems**: Ethereum, Polygon, Solana, Cosmos, Polkadot

## Core Competencies

### 1. Smart Contract Development
**Practical Knowledge:**
- **Solidity/Vyper**: Write secure, gas-efficient smart contracts
  ```solidity
  // Example: Basic ERC-20 token
  pragma solidity ^0.8.0;
  import \"@openzeppelin/contracts/token/ERC20/ERC20.sol\";
  
  contract MyToken is ERC20 {
      constructor() ERC20(\"MyToken\", \"MTK\") {
          _mint(msg.sender, 1000000 * 10**decimals());
      }
  }
  ```
- **Security Patterns**: Reentrancy guards, access control, overflow protection
- **Testing**: Unit tests with Hardhat/Waffle, fuzzing with Echidna
- **Deployment**: Scripting deployments, verifying contracts on explorers

### 2. Frontend Integration
**Practical Implementation:**
- **Wallet Connection**: Implement Web3Modal or RainbowKit for multi-wallet support"},"logprobs":null,"finish_reason":"length"}],"usage":{"prompt_tokens":19,"completion_tokens":350,"total_tokens":369,"prompt_tokens_details":{"cached_tokens":0},"prompt_cache_hit_tokens":0,"prompt_cache_miss_tokens":19},"system_fingerprint":"fp_eaab8d114b_prod0820_fp8_kvcache"}
