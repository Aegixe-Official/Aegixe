# How to Check USDT Address Risk Before Accepting a Payment

[中文](usdt-payment-risk.zh-CN.md) · [Published DEV version](https://dev.to/aegixe/how-to-check-usdt-address-risk-before-accepting-a-payment-4ehc)

Someone offers to pay you in USDT. The balance appears in a wallet screenshot, and the sender says the funds are “clean.” What should you actually check?

**A useful USDT risk check starts with the correct network and token contract, then examines the sending address, transaction evidence and any relevant restrictions. No single score can certify that funds are safe or guarantee an exchange will accept them.**

This AEGIXE guide explains how to screen a proposed payment and distinguish several problems often grouped together as “Black U.”

## What does “Black U” (黑U) mean?

In Chinese-speaking crypto communities, “Black U” is an informal expression often used for USDT associated with suspected scams, theft or other illicit activity. People also use it loosely when discussing frozen funds or restricted deposits.

It is not a separate token standard or a universal technical classification. USDT balances do not acquire a literal black mark that every wallet, exchange and screening provider interprets identically.

Start by separating these questions:

| Question | What needs checking |
| --- | --- |
| Is the asset genuine USDT? | The network and issuer-recognized token contract |
| Does an address have concerning exposure? | Risk labels, supporting transactions, attribution and data coverage |
| Is an address currently restricted by the token issuer? | The relevant token deployment and current restriction state |
| Will an exchange credit the deposit? | The exchange's supported networks, deposit rules and account review |

A real USDT token can still involve counterparty risk. Conversely, a token named “USDT” may be an imitation even if an address screening tool returns no warning.

## Step 1: Verify the network and the actual USDT contract

Agree on the payment network first. USDT on Ethereum and USDT on TRON are not interchangeable deposit instructions, even though both represent the same named asset.

Use [Tether's Supported Protocols and Integration Guidelines](https://tether.to/en/supported-protocols/) to locate the official contract information. At the time of checking for this article, the page lists:

| Network | USD₮ token contract |
| --- | --- |
| Ethereum | `0xdAC17F958D2ee523a2206206994597C13D831ec7` |
| TRON | `TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t` |

**These are token contract identifiers, not addresses to which you should send payment.** Verify them against the issuer's live documentation rather than relying indefinitely on a copied article.

Open the transaction in the explorer for the correct network. Inspect the token contract, transfer amount, addresses and transaction status. A token symbol, logo, balance screenshot or payment notification alone does not authenticate the asset or confirm receipt.

## Step 2: Screen the relevant public addresses

Before accepting a proposed payment, obtain the expected sending address where possible and independently confirm your receiving address. If the payment has already arrived, use the actual transaction to identify the addresses involved.

You can start an address lookup with the [AEGIXE address risk checker](https://risk.aegixe.com/):

1. Select the address's actual blockchain network. The interface checked for this article includes Ethereum and TRON.
2. Enter the complete public address.
3. Run the check and review the returned information, including its limitations.
4. Record the query time and any warnings or missing coverage.

The interface states that this lookup requires only a public address, without connecting a wallet or providing a private key. Do not provide a recovery phrase, approve token spending or sign a transaction merely to obtain an address screening result.

Screening an address does not establish who owns it. A shared exchange withdrawal address, for example, cannot by itself prove the identity of the person paying you.

## Step 3: Read the evidence behind a risk label

When a provider supplies a flag, ask:

- Does it describe the queried address itself or an indirectly connected counterparty?
- What category is assigned, and how does the provider define it?
- Are transaction hashes, sources or explanations available?
- How recent are the data?
- Does the provider cover the relevant network and activity?

Direct and indirect exposure are different. Unsolicited transfers can also appear in an address's history, so a transaction link alone does not establish intent or wrongdoing.

Do not invent a universal “safe score” threshold. Providers use different datasets and models. An unsupported network, failed query or empty result means uncertainty, not proof of clean funds.

For more detail on interpreting a score, see our earlier guide: [Crypto Wallet Address Risk Checks: What a Score Can and Cannot Tell You](https://dev.to/aegixe/crypto-wallet-address-risk-checks-what-a-score-can-and-cannot-tell-you-4jo2).

## Step 4: Keep USDT freezing separate from screening

Tether's [9 December 2023 policy announcement](https://tether.io/news/tether-introduces-new-policy-to-strengthen-ecosystem-security/) describes a voluntary wallet-freezing policy connected to persons on the OFAC Specially Designated Nationals list.

That announcement establishes that issuer restrictions are a real consideration. It does not establish the current status of a particular address or identical implementation details across every network.

A screening provider's high-risk label is not the same thing as a current issuer restriction. A low-risk score does not certify the absence of restrictions either.

When the distinction matters, inspect the relevant token deployment's current state using reliable, network-specific evidence. Record the block or time of the observation. A historic freezing event, a screenshot or an old third-party label may not establish the present state.

A failed transfer is also not sufficient evidence of a freeze: transaction failures can have other causes. Likewise, an on-chain transfer succeeding does not guarantee a later exchange deposit will be credited.

## Step 5: Keep a screening record you can revisit

Record the query time, network, address, original warnings and unknowns. An [optional blank record template](../templates/README.md) is available for your own use; it is not a product API or a formal detection document. Keep private payment records in appropriate internal systems, not public GitHub issues or article comments.

If a material warning cannot be explained, pause acceptance or onward processing and seek appropriate review. Do not treat moving funds through another wallet as evidence that the original concern has disappeared.

## Common questions about checking “Black U”

### Can I check USDT risk using only a transaction hash?

A transaction hash helps locate the transfer, token contract and participating addresses on the correct network. It is a starting point for investigation, not a certificate of lawful origin or future acceptance.

### Does receiving flagged USDT automatically freeze my entire wallet?

That is not a conclusion an address score can support. A token-level restriction, an exchange account restriction and access to other assets are different issues. Check the relevant mechanism and actual evidence rather than assuming one result applies to everything in the wallet.

### Can a small test payment prove the rest is safe?

No. It may help confirm a transfer route, but it does not establish the origin of a larger payment, eliminate counterparty risk or guarantee platform acceptance.

### Does “no risk found” mean the address is clean?

It means no relevant warning was identified within that check's coverage and data at that time. New activity, new attribution or a different provider may produce a different result.

## Check before accepting USDT

Verify the network and genuine token contract, screen the relevant addresses, inspect the evidence, and keep issuer restrictions separate from exchange decisions. Record what remains unknown.

For a public-address lookup, visit the **[AEGIXE address risk checker](https://risk.aegixe.com/)**. For information about AEGIXE's Web3 security services, visit **[aegixe.com](https://aegixe.com/)**.


Updated 12 November 2026. See [sources and review status](../SOURCES.md) for scope.
