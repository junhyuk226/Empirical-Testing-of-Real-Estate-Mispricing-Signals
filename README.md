# Empirical Testing of Real Estate Mispricing Signals

### 부동산 저평가 신호의 실증 검증

A reproducible research framework for detecting apartment mispricing in Seoul and empirically testing whether historical undervaluation signals are associated with future benchmark-relative excess returns across multiple investment horizons.

## Research Question

Given information observable at a historical decision date, can we estimate a conditional value for an apartment, identify potential mispricing, and test whether the resulting signal is associated with future benchmark-relative excess returns?

## Research Area

* Seoul, South Korea
* Initial study area: Nowon-gu
* Asset: Residential apartments
* Initial unit of analysis: Complex × Exact Exclusive Area

## Research Approach

The project follows a reproducible empirical research pipeline:

```text
Historical Information
        ↓
Transaction Data
        ↓
Data Cleaning & Standardization
        ↓
Conditional Price Estimation
        ↓
Mispricing Signal
        ↓
Future Excess Returns
        ↓
Walk-Forward Validation
```

The project is designed to distinguish between:

* price prediction accuracy
* mispricing detection
* future return prediction
* economic investability

A strong price prediction model does not automatically imply that a mispricing signal is economically useful.

## Current Status

**Phase:** Data Preparation & Historical Panel Construction

Completed:

* Initial research question revision
* Raw transaction data acquisition
* Data dictionary construction
* Transaction-level data audit
* Cancellation-status identification
* Duplicate-candidate identification
* Provisional apartment complex identification
* Complex × Exact Area grouping

Next:

* Historical data acquisition
* Historical information/snapshot protocol
* Decision-date construction
* Future-return calculation
* Benchmark construction
* Baseline valuation models
* Mispricing signal construction
* Walk-forward validation

## Research Principles

1. Preserve raw data whenever possible.
2. Do not silently delete ambiguous observations.
3. Separate data cleaning from research assumptions.
4. Use only information available at the historical decision date.
5. Avoid look-ahead bias.
6. Separate statistical prediction from economic return.
7. Document methodological changes and research decisions.
8. Treat empirical findings as predictive relationships rather than causal conclusions unless causality is explicitly established.

## Repository Structure

```text
docs/
├── research_log.md
├── data_audit_v2.md
└── data_dictionary_v1.1.md

src/
notebooks/
results/
```

## Data Source

Initial transaction data are sourced from the Korean Ministry of Land, Infrastructure and Transport Real Transaction Price Disclosure System.

Public release of raw transaction-level data will be subject to applicable source terms and data-use conditions.

## Status

This repository documents an ongoing independent research project.
Methods, data construction procedures, and research conclusions may change as the empirical design develops.
