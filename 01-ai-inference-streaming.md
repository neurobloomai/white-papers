# AI Inference Streaming — The WPM-for-Compute Primitive

**NeuroBloom AI Research**  
**Date:** June 2026  
**Status:** Draft v0.1

---

## Abstract

The precious metals streaming model is one of the highest-margin business structures in modern finance. It generates 85%+ gross margins by providing upfront capital to operators in exchange for a perpetual, low-cost toll on their output. No operational risk. No infrastructure. Pure spread between fixed acquisition cost and floating market price.

This paper argues that the same financial primitive is structurally absent from AI compute — and that its absence represents one of the most significant white spaces in the current AI infrastructure cycle. We call this primitive **AI Inference Streaming**: an instrument through which capital providers fund model training or GPU infrastructure in exchange for a perpetual, fixed-cost percentage of inference revenue.

The instrument does not yet exist. This paper defines its structure, maps the analogy, and outlines the conditions under which it becomes viable.

---

## 1. The Streaming Model — A Primer

In traditional mining, margins are destroyed by operational complexity: labor, energy, equipment, permitting, geopolitical risk. The miner bears all of it. The streaming model observed that the miner's core need is **capital**, not operational partnership. So it separated the two:

```
  Traditional miner:   capital + operations + risk = thin margins
  Streamer:            capital only, zero operations = 65%+ net margins
```

The streamer provides capital upfront. In return, it receives the right to purchase a fixed percentage of production **forever**, at a pre-agreed low price. The spread is the business. As spot prices rise, the streamer's margin grows without any corresponding increase in cost or effort.

Critically, the best streaming deals come from **base metal miners** — copper, zinc, nickel — for whom precious metals are byproducts. These miners need capital to build the primary mine. They sell the byproduct stream cheaply to get it. The streamer arbitrages the attention gap: it values what others treat as secondary.

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

None of these capture what the streaming model captures: **a perpetual, low-cost toll on the output of an asset you helped create**.

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
    BUT volume:           100x year 1
    Net:                  margin compressed, volume compensates
```

The capital provider's bet is on **volume compounding**, not price appreciation — the inverse of precious metals streaming, which bets on price appreciation. Both are valid. AI inference is deflationary in price but exponential in volume. The instrument needs to be structured to capture volume, not margin.

---

## 4. Why This Seat Is Empty

Several conditions have prevented this instrument from emerging:

**4.1 Measurement problem**  
Gold is fungible and physically audited. Inference tokens are not standardized across models or providers. An AISA requires a trusted, tamper-proof accounting layer for token and call attribution. This is a solved problem technically but not yet institutionalized contractually.

**4.2 Model deprecation risk**  
Gold doesn't become obsolete. Models do. A streaming agreement on a specific model faces the risk that the model is superseded and usage migrates. This is manageable — AISAs should be structured at the **organization and API level**, not the model level, giving the streaming right over all inference from the operator regardless of underlying model version.

**4.3 No natural seat holder**  
The streaming model required someone to originate, structure, and hold the streams. In precious metals, that required geological expertise and operator relationships. In AI, the seat requires:
- Deep understanding of model economics
- Relationships with frontier labs and infrastructure operators
- Ability to structure novel financial contracts
- Credibility with both capital allocators and AI builders

This seat is currently **unclaimed**.

**4.4 Regulatory ambiguity**  
Streaming agreements in mining are well-understood by tax and securities regulators. AISAs are not. Early movers will need to work through classification — royalty vs. revenue share vs. financial instrument — across multiple jurisdictions.

---

## 5. Who Holds the Natural Seat

Three candidate seat holders exist:

**Frontier AI Labs**  
Already sit at the intersection of model economics and API infrastructure. Could structure AISAs as a financing mechanism for compute — raising capital through streaming agreements rather than equity, preserving ownership while funding training runs. The lab becomes the operator; external capital takes the stream.

**Sovereign Wealth and Infrastructure Funds**  
Long-duration capital that currently struggles to get clean AI exposure. An AISA offers a contractual, auditable cash flow from AI infrastructure — closer to infrastructure debt than equity. This matches their return horizon and risk appetite better than venture.

**A Purpose-Built Streaming Intermediary**  
The streaming model itself — an entity that raises capital, deploys it across multiple AISAs with different labs and operators, and holds a diversified portfolio of inference streams. Lower risk per agreement, portfolio diversification, and a natural secondary market as the agreements mature.

---

## 6. The Coordination Layer Requirement

One condition not present in precious metals streaming: AI inference output is not self-certifying. Gold can be assayed. Tokens require a coordination layer that:

- Attributes inference output to specific agreements
- Audits usage in real time without operator manipulation
- Enforces payment triggers automatically
- Handles model version transitions transparently

The primitives that enable trusted state, relational accounting, and verifiable handoff across distributed systems are the natural substrate for this coordination layer. The financial instrument and the coordination infrastructure are not separate problems — they are the same problem at different layers of abstraction.

---

## 7. Implications

If this instrument emerges:

```
  For AI labs:          new non-dilutive capital channel
                        aligned incentives — more usage = more payment
                        separation of research funding from monetization

  For capital markets:  first perpetual AI cash flow instrument
                        portfolio diversification into AI infrastructure
                        without operational exposure

  For the industry:     inference becomes an asset class
                        streaming agreements create long-term alignment
                        between funders and operators

  For compute:          GPU buildout can be pre-financed by future inference
                        removes the capital constraint on frontier scaling
```

---

## 8. Open Questions

1. What is the right unit of account — tokens, API calls, or revenue?
2. How should model deprecation and version transitions be contractually handled?
3. What coordination infrastructure is needed for trustworthy metering?
4. How does an AISA interact with existing equity and debt in a lab's capital structure?
5. Which jurisdiction first provides regulatory clarity?

---

## 9. Conclusion

The streaming model is not a mining anomaly. It is a generalizable financial primitive: **provide capital, take a perpetual low-cost toll on output, bear no operational risk**. It has already replicated into pharma royalties, energy, and media.

AI inference is the next frontier for this primitive. The instrument is structurally sound. The conditions are nearly met. The seat is empty.

The entity that claims it will hold one of the most defensible positions in the AI economy.

---

*NeuroBloom AI — founders@neurobloom.ai*  
*This paper represents speculative research. Not financial advice.*
