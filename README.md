# Evaluating the Effectiveness of Public Subsidies for Electric Vehicles

## Project Overview

This project was developed within the *Policy Evaluation* course and focuses on the evaluation of a hypothetical public policy aimed at promoting the adoption of electric vehicles (EVs) through monetary subsidies. The core objective is to design an empirical strategy capable of identifying the **causal effect** of subsidies on individual EV adoption decisions, going beyond simple correlations.

The project is structured as a methodological exercise: starting from a clearly defined policy intervention, it discusses the main econometric challenges involved in evaluation and proposes credible identification strategies grounded in modern causal inference.

## Policy Description

The policy under analysis consists of a **public subsidy for the purchase of electric vehicles**, targeted at individuals below a given income threshold (e.g. €30,000). Eligibility is therefore determined by income, while actual take-up of the subsidy may depend on individual choices, information, and administrative factors.

The intended goal of the policy is twofold:

* Encourage the transition towards low-emission mobility;
* Reduce greenhouse gas emissions by accelerating EV adoption.

## Research Question

The central research question of the project is:

> *What is the causal impact of public subsidies on the probability of purchasing an electric vehicle?*

Answering this question requires isolating the effect of the subsidy from other confounding factors that may simultaneously affect EV adoption, such as environmental preferences, fuel prices, or local infrastructure.

## Why Simple OLS Is Not Sufficient

The project explicitly discusses why a naïve Ordinary Least Squares (OLS) regression is not appropriate for causal inference in this context. Subsidies are typically **endogenous**, because:

* They may be targeted to areas or individuals already more inclined to adopt EVs;
* Important determinants of EV adoption (e.g. environmental attitudes) may be omitted;
* Reverse causality may arise if higher EV adoption leads governments to expand subsidies.

As a result, OLS estimates capture correlation rather than causal effects and are generally biased.

## Ideal Experimental Benchmark

As a benchmark, the project describes an ideal randomized controlled experiment in which eligible individuals are randomly assigned to a treatment group (receiving the subsidy) or a control group. In this setting, the difference in average EV adoption between the two groups would identify the causal effect.

Since such an experiment is typically infeasible in practice, the project then turns to **quasi-experimental methods**.

## Regression Discontinuity Design (RDD)

The main identification strategy proposed is a **Regression Discontinuity Design (RDD)** based on the income eligibility threshold.

* **Running variable**: individual income
* **Cutoff**: €30,000
* **Treatment**: eligibility for the EV subsidy
* **Outcome**: probability of purchasing an electric vehicle

Individuals just below and just above the income threshold are assumed to be comparable, allowing for credible causal inference in a neighborhood around the cutoff.

### Fuzzy RDD

Because eligibility does not perfectly translate into subsidy receipt, the project adopts a **Fuzzy RDD** framework. Eligibility acts as an instrument for actual subsidy take-up, and the causal effect is estimated using a two-stage least squares (2SLS) approach.

This strategy identifies a **local average treatment effect** for individuals whose subsidy receipt is influenced by the income cutoff (compliers).

## Alternative Methods

For completeness, the project briefly discusses alternative empirical strategies that could be employed with richer data:

* **Instrumental Variables (IV)** using external political or institutional variation;
* **Difference-in-Differences (DiD)** exploiting regional or temporal policy variation;
* **Fixed Effects models** using panel data to control for time-invariant unobservables.

Each method is presented with its main strengths and limitations.

## Policy Relevance

Beyond the econometric framework, the project emphasizes the relevance of causal evaluation for policy design. Understanding whether subsidies effectively increase EV adoption is crucial for:

* Allocating public resources efficiently;
* Designing complementary policies (e.g. charging infrastructure, information campaigns);
* Assessing the long-term sustainability of subsidy schemes.

## Skills Acquired

Through this project, I developed and consolidated skills in:

* Policy evaluation and causal inference;
* Identification strategies under endogeneity;
* Regression Discontinuity Design and instrumental variables;
* Translating policy questions into empirical research designs.

Overall, the project demonstrates the ability to critically assess public policies using rigorous economic and econometric reasoning.
