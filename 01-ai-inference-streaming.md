# AI Inference Streaming — The WPM-for-Compute Primitive

**NeuroBloom AI Research**  
**Date:** June 2026  
**Status:** Draft v0.1

---

## Abstract

The precious metals streaming model — pioneered by Wheaton Precious Metals (WPM) — is one of the highest-margin business structures in modern finance. It generates 85%+ gross margins by providing upfront capital to operators in exchange for a perpetual, low-cost toll on their output. No operational risk. No infrastructure. Pure spread between fixed acquisition cost and floating market price.

This paper argues that the same financial primitive is structurally absent from AI compute — and that its absence represents one of the most significant white spaces in the current AI infrastructure cycle. We call this primitive **AI Inference Streaming**: an instrument through which capital providers fund model training or GPU infrastructure in exchange for a perpetual, fixed-cost percentage of inference revenue.

The instrument does not yet exist. This paper defines its structure, maps the analogy, identifies the natural seat holders, and outlines the conditions under which it becomes viable.

---

## 1. The Streaming Model — A Primer

In traditional mining, margins are destroyed by operational complexity: labor, energy, equipment, permitting, geopolitical risk. The miner bears all of it. WPM observed that the miner's core need is **capital**, not operational partnership. So it separated the two:

```
  Traditional miner:   capital + operations + risk = thin margins
  WPM:                 capital only, zero operations = 65% net margins
```

WPM provides $1B upfront. In return, it receives the right to purchase a fixed percentage of gold or silver production **forever**, at a pre-agreed low price (~$400/oz against a spot price of ~$3,300/oz today). The spread is the business. As spot prices rise, WPM's margin grows without any corresponding increase in cost or effort.

Critically, WPM's best deals come from **base metal miners** — copper, zinc, nickel — for whom gold and silver are byproducts. These miners need capital to build the copper mine. They sell the precious metal stream cheaply to get it. WPM arbitrages the attention gap: it values what others treat as secondary.

The result is a business that looks like software — capital-light, infinitely scalable, protected by contract, compounding in value as the underlying asset appreciates.

---

## 2. The AI Compute Analog

The current AI infrastructure cycle has an identical structural tension:

```
  GPU/model operators:   need massive upfront capital
                         (training runs cost $10M–$500M+)
                         bear all operational risk
                         uncertain on inference monetization timeline

  Capital providers:     want exposure to AI upside
                         don't want to operate infrastructure
                         current instruments are too blunt
                         (equity = full risk, debt = capped upside)
```

Today's financing options for AI infrastructure are crude:

| Instrument | Problem |
|---|---|
| Equity | Full operational risk, dilution, long liquidity horizon |
| Venture debt | Fixed return, misses upside, maturity pressure |
| Cloud credits | Not capital, just deferred cost |
| GPU leasing | Spot market, no perpetual claim |

None of these capture what WPM captures: **a perpetual, low-cost toll on the output of an asset you helped create**.

---

## 3. The AI Inference Streaming Structure

We define the primitive as follows:

**AI Inference Streaming Agreement (AISA):**

> A capital provider funds a defined tranche of model training, fine-tuning, or GPU infrastructure buildout. In return, the capital provider receives a contractual right to purchase X% of all inference output — measured in tokens, API calls, or revenue — **in perpetuity**, at a fixed price agreed at deal inception.

```
  At deal time:
    Capital provider → $50M to model operator
    Model operator   → X% of all inference revenue forever
                       at $Y per million tokens (fixed)

  At inference time (year 1):
    Spot inference price: $3/M tokens
    AISA fixed cost:      $0.30/M tokens
    Spread:               $2.70/M tokens → pure margin

  At inference time (year 5):
    Spot inference price: $0.50/M tokens (commoditized)
    AISA fixed cost:      $0.30/M tokens
    Spread:               $0.20/M tokens
    BUT volume: 100x year 1
    Net: margin compressed, volume compensates
```

The capital provider's bet is on **volume compounding**, not price appreciation — the inverse of WPM, which bets on price appreciation of gold. Both are valid. AI inference is deflationary in price but exponential in volume. The instrument needs to be structured to capture volume, not margin.

---

## 4. Why This Seat Is Empty

Several conditions have prevented this instrument from emerging:

**4.1 Measurement problem**  
Gold is fungible and physically audited. Inference tokens are not standardized across models or providers. An AISA requires a trusted, tamper-proof accounting layer for token/call attribution. This is a solved problem technically (cryptographic logs, API-level metering) but not yet institutionalized contractually.

**4.2 Model deprecation risk**  
Gold doesn't become obsolete. GPT-3 did. A streaming agreement on a specific model faces the risk that the model is superseded and usage migrates. This is manageable — AISAs should be structured at the **organization/API level**, not the model level, giving the streaming right over all inference from the operator regardless of underlying model version.

**4.3 No natural seat holder**  
WPM's model required someone to originate, structure, and hold the streams. In precious metals, that required geological expertise and mining relationships. In AI, the seat requires:
- Deep understanding of model economics
- Relationships with frontier labs and infrastructure operators
- Ability to structure novel financial contracts
- Credibility with both capital allocators and AI builders

This seat is currently **unclaimed**.

**4.4 Regulatory ambiguity**  
Streaming agreements in mining are well-understood by tax and securities regulators. AISAs are not. Early movers will need to work through classification (royalty vs. revenue share vs. financial instrument) in multiple jurisdictions.

---

## 5. Who Holds the Natural Seat

Three candidate seat holders exist:

**Frontier AI Labs (e.g., Anthropic)**  
Already sit at the intersection of model economics and API infrastructure. Could structure AISAs as a financing mechanism for compute — raising capital through streaming agreements rather than equity, preserving ownership while funding training runs. The lab becomes the operator; external capital takes the stream. This preserves alignment between lab incentives and model quality while opening a new capital channel.

**Sovereign Wealth / Infrastructure Funds**  
Long-duration capital that currently struggles to get clean AI exposure. An AISA offers a contractual, auditable cash flow from AI infrastructure — closer to infrastructure debt than equity. This matches their return horizon and risk appetite better than VC.

**A Purpose-Built Streaming Intermediary**  
The WPM model itself — an entity that raises capital, deploys it across multiple AISAs with different labs and operators, and holds a diversified portfolio of inference streams. Lower risk per agreement, portfolio diversification, and a natural secondary market as the agreements mature.

---

## 6. The Coordination Layer Requirement

One condition not present in precious metals streaming: AI inference output is not self-certifying. Gold can be assayed. Tokens require a coordination layer that:

- Attributes inference output to specific agreements
- Audits usage in real time without operator manipulation
- Enforces payment triggers automatically
- Handles model version transitions transparently

This is precisely the problem that multi-agent coordination protocols — like PACT — are designed to address at a higher level. The same primitives that enable intent fidelity across agent networks (trusted state, relational ledger, verifiable handoff) can serve as the accounting substrate for an AISA.

In this framing, the PACT protocol is not just a coordination layer for agents — it is potential infrastructure for a new class of AI financial instruments.

---

## 7. Implications

If this instrument emerges, the consequences are significant:

```
  For AI labs:       new non-dilutive capital channel
                     aligned incentives (more usage = more payment)
                     separation of research funding from inference monetization

  For capital markets: first perpetual AI cash flow instrument
                       portfolio diversification into AI infrastructure
                       without operational exposure

  For the industry:  inference becomes an asset class
                     streaming agreements create long-term alignment
                     between funders and operators

  For compute:       GPU buildout can be pre-financed by future inference
                     removes the capital constraint on scaling
```

---

## 8. Open Questions

1. What is the right unit of account — tokens, API calls, or revenue?
2. How should model deprecation and version transitions be contractually handled?
3. What coordination layer is needed for trustworthy metering?
4. How does an AISA interact with existing equity and debt in a lab's capital structure?
5. Which jurisdiction first provides regulatory clarity?

---

## 9. Conclusion

The WPM model is not a mining anomaly. It is a generalizable financial primitive: **provide capital, take a perpetual low-cost toll on output, bear no operational risk**. It has already replicated into pharma royalties (Royalty Pharma), energy (TPL, VNOM), and music (Hipgnosis).

AI inference is the next frontier for this primitive. The instrument is structurally sound. The conditions are nearly met. The seat is empty.

The entity that claims it — whether a frontier lab, a purpose-built intermediary, or a new financial institution — will hold one of the most defensible positions in the AI economy.

---

*NeuroBloom AI — founders@neurobloom.ai*  
*This paper represents speculative research. Not financial advice.*
