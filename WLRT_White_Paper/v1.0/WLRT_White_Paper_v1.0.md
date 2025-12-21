# WLRT — Wave Liquidity Redistribution Theory
White Paper v1.0 \
  \
 **Author**: Petr Popov  \
  **Status**: Research White Paper  \
**Version**: 1.0  \
**License**: CC BY 4.0  \
**Date**: 2025-12-19
## Abstract

This white paper introduces the Wave Liquidity Redistribution Theory (WLRT), a conceptual and mathematical framework describing price dynamics as an emergent consequence of liquidity redistribution across price space. Unlike classical price-centric or equilibrium-based models, WLRT treats liquidity as the primary state variable and models market behavior as wave-like propagation, concentration, and dissipation of liquidity under external and internal forces.

The theory formalizes price space as a continuous medium in which liquidity flows generate observable market regimes, including trends, consolidations, volatility expansions, and structural breaks. By framing price movement as a secondary effect of liquidity gradients, WLRT provides a unified interpretation of market dynamics across timeframes and asset classes.

WLRT is proposed as a foundational framework for liquidity-based market analysis, offering potential applications in market microstructure research, risk modeling, and the development of adaptive trading and monitoring systems. This paper presents the core principles, mathematical intuition, and conceptual implications of the theory, serving as a basis for further empirical validation and applied research.

## 1. Motivation

Classical models of financial markets predominantly describe price dynamics as the primary object of analysis, treating liquidity as a secondary or implicit variable. Such approaches include equilibrium-based frameworks, stochastic price processes, and order-flow-driven models that focus on price changes as fundamental signals. While these models have achieved partial empirical success, they often fail to provide a unified explanation for regime shifts, volatility clustering, persistent trends, and sudden structural breaks observed across markets and timeframes.

Empirical evidence from modern electronic markets suggests that liquidity distribution, rather than price itself, plays a central role in shaping market behavior. Variations in order book depth, concentration of resting liquidity, and the migration of liquidity across price levels frequently precede observable price movements. However, liquidity is typically modeled locally, statically, or as a response variable, rather than as a dynamic medium governing market evolution.

The motivation behind the Wave Liquidity Redistribution Theory (WLRT) is to reverse this perspective by treating liquidity as the primary state variable of the market system. In this framework, price dynamics emerge as a secondary effect resulting from spatial and temporal gradients of liquidity within a continuous price space. Market behavior is therefore interpreted as the propagation, interaction, and dissipation of liquidity waves under external inputs and internal feedback mechanisms.

By conceptualizing liquidity redistribution as a wave-like process, WLRT provides an intuitive and mathematically tractable framework capable of unifying diverse market phenomena—such as trends, consolidations, volatility expansions, and abrupt transitions—within a single theoretical structure. This perspective enables a regime-independent description of market dynamics and offers a foundation for developing liquidity-centric analytical tools that extend beyond traditional price-based indicators.

The primary motivation of this work is to establish a foundational theory that shifts market analysis from price observation to liquidity dynamics, opening new avenues for empirical research, model validation, and applied systems in market monitoring and risk analysis. The term "wave" is used to denote a dynamical redistribution pattern of liquidity governed by transport and diffusion mechanisms, rather than a physical oscillation.

## 2. Core Liquidity Dynamics

Let \( L(p,t) \) denote the continuous liquidity density distributed over price space \( p \in \mathbb{R} \) at time \( t \). Liquidity is interpreted as the aggregated availability of executable volume at a given price level, encompassing both visible and latent components.
Liquidity is not interpreted as executed volume, but as the availability and spatial distribution of executable volume across price levels.

The evolution of liquidity over price space is modeled as a redistribution process driven by local imbalances and external inputs. In its minimal form, the dynamics of liquidity can be expressed as:

dL(p,t)/dt = -(d/dp)(v(p,t)L(p,t)) + D(d^2L(p,t)/dp^2) + S(p,t)  

where:

- \( v(p,t) \) represents the local liquidity drift velocity induced by order flow pressure and strategic repositioning,
- \( D \) is a diffusion coefficient capturing stochastic liquidity dispersion and cancellation effects,
- \( S(p,t) \) denotes external liquidity sources and sinks, including limit order arrivals, removals, and exogenous shocks.

This equation describes liquidity as a dynamic field undergoing transport, diffusion, and injection over price space. Price movement is not treated as an independent stochastic process but emerges as a secondary observable resulting from persistent liquidity gradients and asymmetric redistribution dynamics.

Within this framework, wave-like liquidity behavior arises naturally when transport and diffusion interact under bounded or heterogeneous liquidity conditions, leading to propagation, reflection, and dissipation patterns across price space.

## 3. Price Space Representation
Price space is defined as a continuous one-dimensional domain representing ordered price levels over which liquidity is distributed.
The market is represented as a one-dimensional price space P:  
- the space is divided into discrete price sectors;
- each sector contains an amount of effective liquidity;
- liquidity may redistribute between neighboring sectors.  \
The geometry of price space is fixed and uniform in this version.
## 4. Fundamental Quantities
The model introduces the following quantities:
- rho(P,t): liquidity density;
- grad rho: liquidity gradient;
- J(P,t): liquidity flux;
- c: characteristic redistribution speed;
- gamma: dissipation (market friction);
- S(P,t): external liquidity sources and sinks.  \
Causal structure: liquidity gradient -> liquidity flux -> liquidity waves -> observed price.
## 5. Definition of Price
Observed price is defined as the liquidity-weighted center of the system:  \
P(t) = integral(P * rho(P,t) dP) / integral(rho(P,t) dP).  \
Price reflects the instantaneous configuration of the liquidity field and does not represent discrete transactions.
## 6. Liquidity Dynamics
Liquidity redistribution is described by a damped wave equation:  \
d2 rho / dt2 + gamma * d rho / dt = c^2 * d2 rho / dP2 + dS / dt.  \
This equation captures:
- inertia of liquidity;
- propagation across price levels;
- and dissipation due to friction and execution costs.
## 7. Market Regimes
Different classes of solutions correspond to common market regimes: 
- standing waves correspond to range-bound markets;
- traveling waves to directional trends;
- critical damping to flat or inactive markets;
- and impulse responses to news-driven movements.  \
Regime transitions arise from changes in boundary conditions or external inputs.
## 8. Conservation Properties
In the absence of external sources S:
- total liquidity is conserved;
- local inflows equal local outflows;
- and system behavior is scale-invariant.  \
Violations of conservation indicate external intervention.
## 9. Interpretation of Volatility
Volatility corresponds to the amplitude of liquidity oscillations and the intensity of redistribution processes. High volatility reflects strong internal dynamics rather than randomness or noise.
## 10. GRID Trading Systems
A GRID trading system is interpreted as a discrete wave resonator:
- grid boundaries create standing liquidity waves;
- repeated reflections generate dissipation;
- and profit arises from energy loss during oscillations.  \
GRID systems are effective only in oscillatory regimes.
## 11. Failure Conditions of GRID Systems
GRID systems fail when:
- directional liquidity flux dominates;
- standing waves collapse;
- or boundary conditions are violated.  \
Failure represents a regime transition rather than an execution error.
## 12. Scope and Non-Claims
WLRT does not predict exact prices, does not rely on indicators, and does not assume rational or optimal agents. The theory models structural dynamics rather than forecasts.
## 13. Model Assumptions and Limitations
WLRT:
- assumes linear liquidity response;
- fixed price-space geometry;
- and passive liquidity behavior.  \
These assumptions define the scope of applicability.

## 14. Conclusion

This white paper presented the Wave Liquidity Redistribution Theory (WLRT) as a foundational framework for interpreting market dynamics through the evolution of liquidity rather than direct price observation. By modeling liquidity as a continuous medium distributed across price space, WLRT reframes price movement as an emergent outcome driven by spatial and temporal liquidity gradients.

The theory offers a unified conceptual structure capable of explaining a wide range of market phenomena, including directional trends, range-bound regimes, volatility expansions, and abrupt structural transitions. In contrast to classical equilibrium and price-centric approaches, WLRT emphasizes the dynamic redistribution of liquidity as the primary mechanism underlying observable market behavior.

While the present work focuses on the core principles and mathematical intuition of WLRT, it establishes a theoretical baseline for liquidity-centric market analysis. The framework is intentionally general and asset-agnostic, allowing its application across different market structures, time horizons, and instruments. As such, WLRT serves as a foundation for both theoretical exploration and practical analytical systems centered on liquidity dynamics.


## 15. Future Work

Several directions for future research naturally follow from the WLRT framework:

1. **Empirical Validation**  
   Systematic empirical studies using high-resolution order book and liquidity data are required to validate the proposed wave-like behavior of liquidity redistribution and its relationship to observed price dynamics.

2. **Model Formalization and Extensions**  
   Further formalization of the governing equations, boundary conditions, and stability properties of liquidity waves will enhance the mathematical rigor of the theory and enable analytical and numerical solutions.

3. **Regime Classification**  
   The development of liquidity-based regime classification methods may provide a robust alternative to volatility- or trend-based frameworks, improving market state detection and monitoring.

4. **Cross-Market and Cross-Asset Analysis**  
   Applying WLRT to different asset classes and market microstructures may reveal universal patterns of liquidity redistribution and highlight structural differences between markets.

5. **Applied Systems and Tooling**  
   The WLRT framework may serve as a theoretical basis for liquidity-aware analytical tools, risk monitoring systems, and adaptive market models that respond to real-time liquidity dynamics rather than price signals alone.

These research directions aim to transform WLRT from a conceptual framework into a quantitatively validated theory with broad applicability in market microstructure research and liquidity-driven market analysis.

## 16. References

1. Kyle, A. S. (1985). Continuous Auctions and Insider Trading. *Econometrica*, 53(6), 1315–1335.

2. O’Hara, M. (1995). *Market Microstructure Theory*. Blackwell Publishers.

3. Bouchaud, J.-P., Farmer, J. D., & Lillo, F. (2009). How Markets Slowly Digest Changes in Supply and Demand. *Handbook of Financial Markets: Dynamics and Evolution*, Elsevier.

4. Gatheral, J. (2010). No-Dynamic-Arbitrage and Market Impact. *Quantitative Finance*, 10(7), 749–759.

5. Cont, R., Stoikov, S., & Talreja, R. (2010). A Stochastic Model for Order Book Dynamics. *Operations Research*, 58(3), 549–563.

6. Mandelbrot, B. B. (1997). *Fractals and Scaling in Finance*. Springer.

7. Farmer, J. D., & Skouras, S. (2013). An Ecological Perspective on the Future of Computer Trading. *Foresight*, 15(5), 365–374.

8. Bouchaud, J.-P. (2018). Trades, Quotes and Prices: Financial Markets Under the Microscope. *Cambridge University Press*.

9. Eisler, Z., Bouchaud, J.-P., & Kockelkoren, J. (2012). Models for the Impact of All Order Types. *Quantitative Finance*, 12(9), 1395–1417.

10. Popov, P. (2025). Wave Liquidity Redistribution Theory (WLRT). *Research White Paper*, Version 1.0.


## 17. Disclaimer
This document describes a theoretical research model and does not constitute financial or investment advice.
