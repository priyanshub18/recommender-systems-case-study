# Netflix Recommender System Architecture: A Graph Theory Walkthrough

An interactive, animated presentation walking through Netflix's recommendation engine through the rigorous lens of Graph Theory, Bipartite Topologies, Personalized PageRank, and Graph Neural Networks.

🌐 **Live GitHub Pages URL:** [https://priyanshub18.github.io/recommender-systems-case-study/](https://priyanshub18.github.io/recommender-systems-case-study/)

---

## 📽️ Interactive Presentation Features
- **1280×720 Responsive Presentation Stage**: Automatic viewport scaling (`fit()`) for any screen size or projector.
- **Narrated Step-by-Step Delivery**: Real-time presenter notes panel (`N` key) explaining each topological concept in natural spoken English.
- **Dynamic Animated Wires & Graph Topologies**: Visualizes subscribers, media items, directors, genres, and live edge attributes using pulsing SVG circuits.
- **Segmented Interactive Progress Bar**: Track chapter and step progression in real time.
- **Keyboard Navigation**: Full support for Space, Arrow keys, PageUp/Down, Fullscreen (`F`), Clean view (`H`), and Chapter jump modal (`M`).

---

## 🗺️ Chapter Roadmap

1. **The Netflix Graph Problem**: Beyond the flat matrix — why tabular matrices fail under 99.8% sparsity across 3.9 Trillion potential cells.
2. **The Core Bipartite Graph $\mathcal{G} = (U, V, E)$**: User and Media item partitions, weighted implicit telemetry edges ($w_{uv}$), and block adjacency matrix structure.
3. **Graph Projections & 2-Hop Paths**: Item-Item co-viewing projections ($S = R^T R$), User-User affinity ($S = R R^T$), and 2-hop walks explaining "Because you watched".
4. **Personalized PageRank & Random Walks with Restart**: Simulating 10,000 particle walks with teleport probability $\alpha = 0.15$ to converge on stationary visitation vectors $\mathbf{\pi}_u$.
5. **Heterogeneous Information Networks (HIN) & Cold Start**: Solving zero-view new releases with typed director, actor, and genre vertices via PathSim metapaths.
6. **Graph Neural Networks (GNNs) & Message Passing**: Multi-hop convolutions aggregating structural neighborhood context into 64-dimensional continuous embeddings.
7. **Matrix Factorization as Graph Laplacian Smoothing**: Proving that classical SVD/MF is mathematically equivalent to Dirichlet energy minimization and low-frequency harmonic filtering on $\mathbf{L} = \mathbf{D} - \mathbf{A}$.
8. **Community Detection & 76,000 Micro-Genres**: Discovering algorithmic taste clusters using Louvain modularity optimization ($Q$).
9. **Real-Time Edge Streaming & Dynamic Reweighting**: Sub-15ms local push graph updates on Apache Flink when an episode finishes.
10. **Production Architecture Blueprint**: End-to-end distributed pipeline serving 260 million subgraphs with sub-15ms p99 SLA.
11. **Summary & The 6 Laws of Recommender Graph Theory**: Key takeaways unifying graph theory and recommender systems.

---

## ⌨️ Presentation Controls
| Key | Action |
|---|---|
| `Space` / `→` / `Enter` | Advance to next step |
| `←` / `Backspace` | Return to previous step |
| `]` / `[` | Jump to next / previous chapter |
| `M` | Open Chapter Jump Menu |
| `N` | Toggle Presenter Speech Notes |
| `F` | Toggle Fullscreen Mode |
| `H` | Toggle Clean Mode (hide header/footer) |
| `?` | Toggle Keyboard Shortcuts Help |
| `Esc` | Close open overlays |
