# Nano Empire AI

**Machine-payable recall intelligence (`RecallGuard`), deterministic procurement/appeal document defense (`BidShield`), and 5-stage MCP tool verification (`SkillProof`) for autonomous agents and engineering teams.**

![Status: Live Production](https://img.shields.io/badge/gateway-nanoempireai.com-10b981)
![x402 Settlement: Base Mainnet USDC](https://img.shields.io/badge/x402-Base_Mainnet_USDC-3b82f6)
![Self-Test Settlements: 1 ($0.05 USDC)](https://img.shields.io/badge/verified_settlements-1_self--test-6366f1)
![Outside Paying Customers: 0](https://img.shields.io/badge/outside_paying_customers-0-f59e0b)

---

## 1. The Four Agent Commerce Rails

| Rail | Standard | Live Implementation |
|------|----------|---------------------|
| **1. Talk (Discovery & Coordination)** | Google `A2A v0.3.0` + Meta/Sierra `PAP/1.0` + Anthropic `MCP` | [`/.well-known/agent-card.json`](https://www.nanoempireai.com/.well-known/agent-card.json) · [`/.well-known/poppy.json`](https://www.nanoempireai.com/.well-known/poppy.json) · [`/.well-known/mcp.json`](https://www.nanoempireai.com/.well-known/mcp.json) |
| **2. Mandate (Cryptographic Intent)** | EIP-3009 `TransferWithAuthorization` + SHA-256 Evidence Chains | Bounded per-call authorization on Base Mainnet (`eip155:8453`) with deterministic receipt verification |
| **3. Checkout (Human & Enterprise)** | Stripe Live Checkout + `offers.json` (`v1.4.0`) | [`https://www.nanoempireai.com/offers.json`](https://www.nanoempireai.com/offers.json) (`$99` MCP Audit Pilot · `$99/$299` BidShield Triage · `$30/$99` RecallRadar) |
| **4. Settlement (Machine-to-Machine)** | Linux Foundation / Coinbase `x402 v2` (`Base USDC`) | Instant HTTP 402 micropayments (`$0.05` / `$0.10` USDC) to `0x90E23A7b6F6494A879d05DDC4278D0e55Dec1e01` |

---

## 2. Live Endpoints & Pricing

| Endpoint / Surface | Protocol | Price | Status |
|--------------------|----------|-------|--------|
| [`GET https://recallguard-api.vercel.app/api/v1/health`](https://recallguard-api.vercel.app/api/v1/health) | REST / JSON | **Free** | **LIVE** (`46,642` CPSC/FDA/Health Canada recalls) |
| `GET https://recallguard-api.vercel.app/api/v1/feed` | `x402` (`eip155:8453`) | **$0.05 USDC** (`50000` atomic) | **LIVE** (HTTP 402 challenge active) |
| `POST https://recallguard-api.vercel.app/api/v1/match` | `x402` (`eip155:8453`) | **$0.10 USDC** (`100000` atomic) | **LIVE** (HTTP 402 challenge active) |
| [`https://www.nanoempireai.com/grok-mcp/`](https://www.nanoempireai.com/grok-mcp/) | Stripe / Web | **$99** (3-Tool Pilot) | **LIVE** |
| [`https://www.nanoempireai.com/bidshield/triage/index.html`](https://www.nanoempireai.com/bidshield/triage/index.html) | Stripe / Web | **$99** (Annex Gap Scan) | **LIVE** |

---

## 3. Verified On-Chain Settlement & Epistemic Ledger

- **Base Mainnet Block `51961194`:** [`0x0581b819b2e5b481cbbcfb8fe81e6fe57a0d0ef9c6f8fc04952164761586da64`](https://basescan.org/tx/0x0581b819b2e5b481cbbcfb8fe81e6fe57a0d0ef9c6f8fc04952164761586da64) (`0.05 USDC` settled via x402 for `GET /api/v1/feed`).
- **Current Truth:** `1` verified on-chain self-test settlement (`$0.05 USDC`). `0` outside paying customers to date.

---

## 4. Canonical Repositories

| Repository | Role | Install / Access |
|------------|------|------------------|
| **[`Nano-Empire-Ai/nanoempire-web`](https://github.com/Nano-Empire-Ai/nanoempire-web)** | Sovereign gateway, `A2A`/`PAP`/`MCP` manifests, `BidShield` & `MCP Auditor` portals | [`nanoempireai.com`](https://www.nanoempireai.com) · [`llms.txt`](https://www.nanoempireai.com/llms.txt) |
| **[`Nano-Empire-Ai/nano-empire-tollbooth`](https://github.com/Nano-Empire-Ai/nano-empire-tollbooth)** | Python decorator SDK for HTTP 402 machine paywalls and Base USDC metering | `pip install nano-empire-tollbooth` |
| **[`Nano-Empire-Ai/nano-x402-client`](https://github.com/Nano-Empire-Ai/nano-x402-client)** | Client SDK for autonomous agents to negotiate and settle HTTP 402 challenges | `npm i @nanoempireai/nano-x402-client` |
| **[`Nano-Empire-Ai/nano-empire-mcp-suite`](https://github.com/Nano-Empire-Ai/nano-empire-mcp-suite)** | Model Context Protocol (MCP) server suite with `x402` metering and trial onramps | [`/.well-known/mcp.json`](https://www.nanoempireai.com/.well-known/mcp.json) |
| **[`roblambert9/recallguard-mcp`](https://github.com/roblambert9/recallguard-mcp)** | Smithery-certified (`Grade A`) MCP server for CPSC/FDA/Health Canada recall screening | `npx recallguard-mcp` |
| **[`roblambert9/bidshield-kernel`](https://github.com/roblambert9/bidshield-kernel)** | Open-source deterministic RFP/SOW & ERISA claim document-defense kernel (`v0.2`) | `python bidshield_kernel.py` |

---

**Contact:** Robert Lambert (`rob@nanoempireai.com`) · **Machine Index:** [`https://www.nanoempireai.com/llms.txt`](https://www.nanoempireai.com/llms.txt)
