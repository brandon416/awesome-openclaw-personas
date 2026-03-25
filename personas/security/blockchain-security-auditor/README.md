# Blockchain Security Auditor

A relentless smart contract security researcher who assumes every contract is exploitable until proven otherwise. Systematically identifies vulnerability classes (reentrancy, oracle manipulation, flash loan attacks, access control flaws), produces professional audit reports with severity classifications and Foundry proof-of-concept exploits, and has dissected hundreds of protocols to prevent millions in losses.

## Core Capabilities

- Performs line-by-line manual code review combined with automated static analysis (Slither, Mythril) and property-based fuzz testing (Echidna/Foundry)
- Identifies DeFi-specific vulnerabilities including flash loan oracle manipulation, reentrancy through ERC-777/1155 hooks, and governance flash loan voting attacks
- Produces professional audit reports with severity classifications (Critical/High/Medium/Low/Informational) and reproducible Foundry PoC exploits for every finding
- Conducts economic and game theory analysis modeling incentive structures, extreme market conditions (99% price drops, zero liquidity), and MEV extraction
- Provides actionable remediation with specific code changes (e.g., Checks-Effects-Interactions pattern, Chainlink TWAP oracles, ReentrancyGuard)
- Runs comprehensive access control audits covering role hierarchies, initialization protection, upgrade controls, and delegatecall safety

## Files

| File | Purpose |
|------|--------|
| `SOUL.md` | Identity as paranoid, adversarial thinker with a mental database of every major DeFi exploit since The DAO hack, severity classification system, ethical standards |
| `AGENTS.md` | Audit report template structure, Foundry exploit PoC examples, 5-step workflow (scope/reconnaissance, automated analysis, manual review, economic analysis, report/remediation), communication style, pattern recognition |
| `SKILL.md` | Vulnerability detection methodology, Solidity code examples (reentrancy vulnerable vs fixed, oracle manipulation vulnerable vs fixed), access control audit checklist, Slither/Mythril/Echidna analysis scripts, advanced capabilities (formal verification, read-only reentrancy, storage collision, incident response) |

## Quick Start

```bash
cp -r blockchain-security-auditor/ ~/.openclaw/workspace/
```

## Use Cases

- Auditing a DeFi lending protocol's smart contracts for reentrancy, oracle manipulation, and flash loan attack surfaces before mainnet deployment
- Reviewing an upgradeable proxy contract for storage collision risks, unprotected initialization, and admin privilege escalation
- Writing a comprehensive audit report with severity classifications and Foundry test cases that reproduce each vulnerability
- Analyzing a post-hack incident to trace the attack transaction, identify root cause, and write a post-mortem with preventive measures
- Running Slither, Mythril, and Echidna against a protocol's contracts and triaging automated findings against manual review results
