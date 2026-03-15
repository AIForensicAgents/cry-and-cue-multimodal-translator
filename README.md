┌──────────────────┐
                    │   Audio / Video   │
                    │   Input Stream    │
                    └────────┬─────────┘
                             │
              ┌──────────────┴──────────────┐
              │                             │
     ┌────────▼────────┐         ┌──────────▼──────────┐
     │  🎤 Audio Model  │         │  👁️ Vision Model     │
     │  Cry classifier  │         │  Pose & expression   │
     │  (spectral +     │         │  detection (body     │
     │   temporal CNN)   │         │   key-points + CNN)  │
     └────────┬─────────┘         └──────────┬──────────┘
              │                              │
              └──────────────┬───────────────┘
                             │
                  ┌──────────▼──────────┐
                  │  🧬 Fusion Engine    │
                  │  Late-fusion with    │
                  │  attention weighting │
                  └──────────┬──────────┘
                             │
                  ┌──────────▼──────────┐
                  │  👤 Personalization  │
                  │  Infant baseline     │
                  │  calibration layer   │
                  └──────────┬──────────┘
                             │
              ┌──────────────┴──────────────┐
              │              │              │
     ┌────────▼───────┐ ┌───▼────────┐ ┌──▼──────────────┐
     │ 📋 Action Plan  │ │ 🗣️ Calming │ │ 🚨 Pediatric    │
     │ Prioritized     │ │   Scripts  │ │   Alert Engine   │
     │ suggestions     │ │            │ │                  │
     └────────────────┘ └────────────┘ └──────────────────┘