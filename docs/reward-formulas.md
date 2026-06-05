# NovaRune Reward Formulas

## Base Relay Reward

```
Reward = BaseRate × BandwidthGB × UptimeFactor × StakeMultiplier
```

- **BaseRate**: Dynamically set by Nexus based on network demand
- **UptimeFactor**: 0.0 – 1.0 (exponential penalty below 95% uptime)
- **StakeMultiplier**: log(1 + staked_amount) for diminishing returns and fairness

## Task Bounty Rewards
Higher rewards for critical infrastructure tasks assigned by Nexus (e.g., new region peering, high-traffic relay).

## Self-Improvement Bonus
Nodes and agents that contribute to measurable network improvement (latency reduction, new peer onboarding) receive bonus multipliers.

All rates are continuously tuned by the live Nexus orchestrator.