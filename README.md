# Recommender Systems Architecture — Interactive Presentation (PPT)

A high-performance, strictly monochromatic PowerPoint-style presentation and interactive case study on production Recommender Systems, their mathematical formulations, and Netflix's algorithmic engine.

## 📽️ PPT Features & Mathematical Animations
1. **Interactive Animated Matrix Factorization ($R \approx P \times Q^T$)**:
   - Live step-by-step dot product calculation: sweeps across User latent row $u$ and Item column $i$, calculating intermediate factor products before updating the predicted rating.
2. **Two-Tower Neural Retrieval & MIPS**:
   - Dual-encoder architecture diagram (User Tower $f_\theta(u)$ & Item Tower $g_\phi(i)$).
   - Dynamic vector space angle and cosine similarity calculator.
3. **Animated 4-Stage Candidate Funnel**:
   - Live HTML5 Canvas particle simulation visualizing candidate pruning from 10,000,000 catalog items down to 10 page recommendations.
4. **Netflix Production Walkthrough**:
   - 2D Page Generation: optimizing vertical row composition and horizontal title rankings simultaneously.
   - Dynamic Artwork Personalization with **LinUCB Contextual Bandits**:
     - Live interactive formula breakdown separating the **Exploitation** payoff ($\theta_a^T x_u$) from the **Exploration** uncertainty ellipsoid ($\alpha \sqrt{x_u^T A_a^{-1} x_u}$).
     - Real-time subscriber persona switcher (Action fan, Romance fan, Star actor fan) showing dynamic artwork transformation and confidence bounds.
5. **Position Bias & Inverse Propensity Scoring (IPS)**:
   - Mathematical correction formula for logged observational feedback and rank examination probabilities.
6. **Production Serving Blueprint**:
   - End-to-end data pipeline: Kafka $\to$ Flink $\to$ Redis/Cassandra Feature Store $\to$ Envoy gRPC sub-15ms serving.

## ⌨️ Presentation Controls
- `→` / `Space` / `PageDown`: Next slide
- `←` / `PageUp`: Previous slide
- `G`: Slide Overview Grid (jump to any slide)
- `F`: Toggle Fullscreen Presentation Mode
- `P`: Toggle Auto-Advance Slides
- `T`: Toggle Monochrome Theme (Pitch Black vs Studio White)
