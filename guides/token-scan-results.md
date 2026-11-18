# AI Smart Contract Review Guide

[中文](token-scan-results.zh-CN.md) · [Open tool](https://token-security.aegixe.com/) · [Index](../README.md)

Scope: the on-chain contract checker linked as AI smart contract review on the AEGIXE website. Workflow checked on 12 November 2026 in the Chinese interface.

## 1. Prepare the input

Obtain the full token contract address and network from the project's established channels or the appropriate block explorer. Matching symbols do not establish matching contracts. The input mentions token or LP addresses; this check covered a token contract on Ethereum Mainnet, rather than LP addresses or every network.

## 2. Start a scan

1. Open the tool and confirm the chain under “选择链”. Ethereum Mainnet was the default during the check.
2. Paste the full contract into “按地址或者 LP 地址搜索令牌”.
3. Click “开始扫描”. Wait for the result page, then verify the token name, symbol, chain and contract. A name alone does not authenticate a project.
4. Read “检测通过” (passed), “注意项” (attention), “风险项” (risk) and “综合净分” (overall net score), then inspect the details.

## 3. Read results and details

| Area | What to check |
| --- | --- |
| Token information | Symbol, name, contract, creator and owner. For shortened addresses, use the copy control and compare the full value with original public sources. |
| Holder information | Holder count, creator/owner holdings and top-10 share. “查看详情” opens the information offered by the page. Do not infer actual distribution from anomalous statistics. |
| Risk assessment | Read each title and explanation. Distinguish a permission's existence, its potential misuse and an action that has actually occurred. |
| Multidimensional details | Click “多维检测详情” for “安全分数” (safety score) and liquidity, token control, contract trust, community and market transparency dimensions, with component descriptions and values. “返回” returns to the overview. |

The interface uses both “overall net score” and “safety score”. The complete formula and thresholds were not verified, nor was it established whether every description represents a triggered finding. Do not classify safety from one value or describe a perfect score as a guarantee.

## 4. Handle findings that need verification

- **Minting, blacklist or pause permissions:** check code, controllers and project rules. Having a permission does not prove malicious use.
- **No detected pool lock or liquidity information:** check the object and data coverage before drawing conclusions. It does not establish an actual liquidity withdrawal.
- **Anomalous holder counts or inconsistent overview/detail descriptions:** both kinds of issue were observed during the workflow check. Preserve the original records, verify against sources such as a block explorer and keep affected fields unresolved. Do not circulate them as formal technical conclusions.
- **No result, chain mismatch or request failure:** verify chain and address and retry later. Absence of results is not a passed scan.

## 5. Scope

Submission, result overview and multidimensional navigation were checked. Result accuracy has not undergone independent technical verification. Automated scanning supports further investigation; it does not replace a full manual audit of business logic, deployment and external dependencies.

Record time, network, full contract and unresolved items. Resolve contradictory data before interpreting it. [Security service enquiries](https://aegixe.com/contact-us-form/)
