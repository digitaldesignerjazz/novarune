# Integration with QCoin and NovaCoin Repositories

## Overview
NovaRune is the infrastructure-focused rune within the broader QCoin economy and is designed to work closely with the NovaCoin base settlement layer.

## Key Connections

### With QCoin Repo
- Rune mechanics and general economy design live primarily in the qcoin repository
- NovaRune is the main "workhorse" rune for real infrastructure
- Shared agents (especially Wizard Q and Swarm Coordinator) interact with both

### With NovaCoin Repo
- The NovaRune ↔ NovaCoin bridge is a critical cross-repo component
- Staking and rewards may eventually settle on the NovaCoin chain
- Nexus acts as the common orchestration layer for both

## Recommended Development Flow
1. Design rune-specific logic in novarune repo
2. Design base chain logic in novacoin repo
3. Document cross-layer concerns in both repos (see docs/qcoin-novacoin-bridge.md in novacoin)
4. Implement bridge as a joint effort
5. Use Nexus as the real-time coordinator and data plane

This modular structure keeps concerns clean while maintaining tight integration through Nexus and the bridge.