# Nano Empire AI

**Empirical Security Benchmarks, Deterministic Procurement Defense (`BidShield`), and Cryptographic Tool Verification (`SkillProof`) for the Autonomous Agent Economy.**

[![Status: Live Production](https://img.shields.io/badge/gateway-nanoempireai.com-10b981)](https://www.nanoempireai.com)
[![2026 MCP Benchmark](https://img.shields.io/badge/Benchmark-MSHB--2026-00b5e2)](https://www.nanoempireai.com/benchmarks/mcp-security)
[![x402 Settlement: Base Mainnet USDC](https://img.shields.io/badge/x402-Base_Mainnet_USDC-3b82f6)](https://basescan.org/tx/0xf3919e8c55a4e7163cb10e88baa1d4b183d861ff379a54d0d001d932a6325999)
[![SkillProof Gate](https://img.shields.io/badge/GitHub_Action-v1-a3ff00)](https://github.com/Nano-Empire-Ai/skillproof-action)
[![Verified On-Chain Settlements](https://img.shields.io/badge/verified_settlements-1_self--test-6366f1)](https://basescan.org/block/51961194)
[![Outside Paying Customers: 0](https://img.shields.io/badge/outside_paying_customers-0-f59e0b)](https://www.nanoempireai.com/status.json)

---

## 🏆 The 2026 Model Context Protocol (MCP) Security Benchmark (MSHB-2026)

Nano Empire maintains the definitive empirical security benchmark evaluating canonical Model Context Protocol servers against 6 deterministic execution sink vectors:
1. **Shell / Subprocess Execution Sinks** (`subprocess.Popen`, `execSync`, `spawn`)
2. **Dynamic Code Evaluation Hazards** (`eval()`, `new Function()`)
3. **Filesystem Mutation Bounds** (unbounded directory writes & path traversal)
4. **Credential & Secret Isolation** (`process.env` serialization leaks)
5. **Network Egress Boundaries** (unpinned socket & HTTP egress)
6. **Governance Hygiene** (`SECURITY.md`, deterministic lockfiles, OSI licenses)

👉 **[View the Live Benchmark Leaderboard (25 Ranked Repos) →](https://www.nanoempireai.com/benchmarks/mcp-security)**

### Add the SkillProof Security Gate to Your CI/CD
Add this to `.github/workflows/skillproof.yml` in your repository:
```yaml
name: SkillProof Security Gate
on: [push, pull_request]

jobs:
  verify:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run SkillProof Gate
        uses: Nano-Empire-Ai/skillproof-action@v1
        with:
          min_score: 80
          fail_on_critical: true
```

---

## ⚡ The Four Agent Commerce Rails

| Rail | Protocol Standard | Live Production Implementation |
|---|---|---|
| **1. Discovery & Coordination** | Google `A2A v1.0` + Linux Foundation AAIF + Anthropic `MCP` | [`/.well-known/agent-card.json`](https://www.nanoempireai.com/.well-known/agent-card.json) · [`/agents.json`](https://www.nanoempireai.com/agents.json) · [`/llms.txt`](https://www.nanoempireai.com/llms.txt) |
| **2. Cryptographic Gate** | SkillProof Ed25519 Trust Manifests + FIDO AP2 Spend Bounds | [`GET /api/skillproof/status`](https://www.nanoempireai.com/api/skillproof/status) · [`POST /api/bidshield/gate`](https://www.nanoempireai.com/api/bidshield/gate) |
| **3. Machine Settlement** | Linux Foundation x402 v2 (`Base USDC`) | Streamable HTTP micropayments (`$0.05` / `$0.10` USDC) to `0x90E23A7b6F6494A879d05DDC4278D0e55Dec1e01` |
| **4. Escrow & Enterprise** | Upwork Project Catalog + Stripe Live Checkout | [Upwork RFP Compliance Matrix ($149–$499 USD)](https://www.upwork.com/services/product/writing-translation-a-compliance-matrix-of-every-mandatory-requirement-in-your-government-rfp-2074328625924014322) |

---

## 📦 Canonical Open Source Packages & Repositories

| Repository | Role | Quick Install |
|---|---|---|
| **[`Nano-Empire-Ai/skillproof-action`](https://github.com/Nano-Empire-Ai/nanoempire-web/tree/main/packages/skillproof-action)** | 6-vector static security and governance gate for GitHub Actions | `uses: Nano-Empire-Ai/skillproof-action@v1` |
| **[`Nano-Empire-Ai/recallguard-mcp`](https://github.com/roblambert9/recallguard-mcp)** | Smithery-listed MCP server for 46,642 US & Canadian product recalls | `npx recallguard-mcp` |
| **[`Nano-Empire-Ai/nano-empire-tollbooth`](https://github.com/Nano-Empire-Ai/nano-empire-tollbooth)** | Python decorator SDK for HTTP 402 machine paywalls & Base USDC settlement | `pip install nano-empire-tollbooth` |
| **[`roblambert9/bidshield-kernel`](https://github.com/roblambert9/bidshield-kernel)** | Deterministic RFP/SOW fatal disqualifier and deontic clause extractor | `python bidshield_kernel.py` |
| **[`Nano-Empire-Ai/nanoempire-web`](https://github.com/Nano-Empire-Ai/nanoempire-web)** | Production gateway, benchmark leaderboard, and programmatic search hubs | [nanoempireai.com](https://www.nanoempireai.com) |

---

## 🔍 Verified On-Chain Ledger & Honest Status

- **Base Mainnet Block `51961194`:** [`0xf3919e8c55a4e7163cb10e88baa1d4b183d861ff379a54d0d001d932a6325999`](https://basescan.org/tx/0xf3919e8c55a4e7163cb10e88baa1d4b183d861ff379a54d0d001d932a6325999) (`0.05 USDC` settled via x402 on 2026-09-29).
- **Public Epistemic Ledger:** `1` verified on-chain self-test settlement. `0` outside paying customers to date.
- **7-Day Automated Changelog:** [`https://www.nanoempireai.com/changelog.json`](https://www.nanoempireai.com/changelog.json)

---

**Executive Operations:** Hana Lambert (`hana@nanoempireai.com`) · **Founder:** Robert Lambert (`rob@nanoempireai.com`) · **Machine Context:** [`llms.txt`](https://www.nanoempireai.com/llms.txt)
