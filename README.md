# Architecture of Modern Production Recommender Systems — Netflix Case Study

A high-performance, strictly monochromatic engineering presentation and whitepaper detailing how modern machine learning recommender systems operate at massive scale (100M+ items down to 10 sub-millisecond personalized recommendations).

## Key Content & Topics Covered
1. **The Multi-Stage Retrieval Funnel**:
   - Stage 1: Candidate Retrieval (10M &rarr; 1,000 items, &lt;5ms) using Two-Tower DNNs and Vector ANN (FAISS/ScaNN).
   - Stage 2: First-Stage Scoring (1,000 &rarr; 200 items, &lt;15ms) using DCN / LightGBM.
   - Stage 3: Heavy Multi-Task Reranking (200 &rarr; 50 items, &lt;30ms) using Sequence Transformers (BST / MMoE).
   - Stage 4: Page Slate, Diversity & Dedup (50 &rarr; 10-20 items, &lt;10ms) using Determinantal Point Processes (DPP).
2. **Mathematical Formulations & Interactive Models**:
   - Latent Matrix Factorization ($R \approx P \times Q^T$).
   - Interactive 3D vector embedding dot-product simulator.
   - Two-Tower Dual Encoders & Maximum Inner Product Search (MIPS).
3. **Netflix Production Case Study**:
   - 2D Page Generation: optimizing vertical row order and horizontal video rank simultaneously.
   - Dynamic Artwork Personalization: Contextual Multi-Armed Bandits (LinUCB / Thompson Sampling) that dynamically select thumbnail posters based on user viewing preferences.
   - Interactive Persona Switcher demonstrating real-time bandit arm selection and confidence bounds.
4. **Offline vs. Online Evaluation & Position Bias**:
   - Offline metrics: NDCG@K, Recall@K, MRR, Intra-list diversity.
   - Online metrics: Session Take-rate, Median time to play, Day-28 retention, and Inverse Propensity Scoring (IPS).

## Design System
- **Strict Monochromatic Palette**: High-contrast pure black, pure white, and neutral technical grays.
- **Dual Presentation Modes**:
  - Full-length Whitepaper / Document mode.
  - Interactive Slide Deck mode (press `D` or click "Deck View").
- **Keyboard Shortcuts**:
  - `D`: Toggle Deck / Doc view.
  - `T`: Toggle Dark / Light monochrome theme.
  - `←` / `→`: Navigate presentation slides.
