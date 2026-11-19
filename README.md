# Recommender Systems: A Graph Theory Approach (20-Slide Seminar Deck)

An interactive, step-by-step 20-slide presentation explaining how recommender systems work from first principles using graph theory, with a dedicated 2-slide real-world case study on Netflix.

- **Live 20-Slide Deck (Main):** [https://priyanshub18.github.io/recommender-systems-case-study/](https://priyanshub18.github.io/recommender-systems-case-study/)
- **Direct Link (`recommender-systems.html`):** [https://priyanshub18.github.io/recommender-systems-case-study/recommender-systems.html](https://priyanshub18.github.io/recommender-systems-case-study/recommender-systems.html)
- **Previous 11-Slide Netflix Deck (`netflix.html`):** [https://priyanshub18.github.io/recommender-systems-case-study/netflix.html](https://priyanshub18.github.io/recommender-systems-case-study/netflix.html)

---

## 20-Slide Outline

### Part 1 — Foundations of Recommender Systems (Slides 1–6)
1. **Title:** Recommender Systems: A Graph Theory Approach
2. **Presentation Outline:** 4-part roadmap
3. **Information Overload:** Millions of catalogue items vs. 10–30 screen slots; Search vs. Recommendation
4. **Real-World Applications:** E-commerce (Amazon/Flipkart), Audio/Video (Spotify/YouTube), Streaming (Netflix/Prime), Social (LinkedIn/Instagram)
5. **Data Signals:** Explicit feedback (ratings, likes, reviews) vs. Implicit feedback (dwell/watch time, purchases, repeat plays)
6. **Three Classic Paradigms:** Content-Based Filtering, Collaborative Filtering, and Hybrid Graph Models

### Part 2 — The Graph Theory Model (Slides 7–10)
7. **Why Switch from a Table to a Graph?** $>99\%$ matrix sparsity vs. storing only active edges
8. **Graph Theory Definitions:** Vertex ($v$), Edge ($e$), Degree ($\deg(v)$), and Path
9. **The User–Item Bipartite Graph $G = (U, I, E)$:** Users ($U_1 \dots U_4$) and Items ($I_1 \dots I_5$)
10. **Weighted Edges & Bi-Adjacency Matrix $\mathbf{B}$:** Engagement weights $w(u, i)$ and time decay

### Part 3 — Graph Algorithms for Recommendation (Slides 11–16)
11. **Collaborative Filtering via Paths:** 1-hop (known items), 2-hop (peer users), and 3-hop (unseen candidate items) + bipartite parity rule
12. **2-Hop Graph Projections:** Folding the graph into User–User similarity ($\mathbf{B}\cdot\mathbf{B}^T$) and Item–Item similarity ($\mathbf{B}^T\cdot\mathbf{B}$)
13. **Scoring by Path Counts:** Ranking candidate items by length-3 path counts ($\mathbf{S} = \mathbf{B}\cdot\mathbf{B}^T\cdot\mathbf{B}$)
14. **Degree Normalization:** Controlling high-degree hub bias via Cosine and Jaccard similarity
15. **Random Walk with Restart (Personalized PageRank):** Animated 100,000-step random walker approximating path scores at million-node scale
16. **Solving Cold Start with Attribute Vertices:** Adding content attribute nodes ($A_1, A_2$) to connect zero-degree new items ($I_{\text{new}}$)

### Part 4 — Netflix Case Study & Production Systems (Slides 17–20)
17. **Case Study: Netflix (Slide 1 of 2):** Mapping the Viewer–Show graph and generating explainable rows (*"Because you watched Dark"*)
18. **Case Study: Netflix (Slide 2 of 2):** 80% of hours streamed, $\$1\text{B+}/\text{yr}$ retention value, 90-second attention window, and production edge weights
19. **Production Pipeline & Challenges:** 4-stage pipeline (Collect $\to$ Build Graph $\to$ Retrieve $\to$ Rank & Serve) and limitations (Popularity bias, Filter bubbles, Privacy)
20. **Summary & References:** Key takeaways, academic citations, and Q&A

---

## Controls
`Space` / `→` next · `←` back · `F` fullscreen · `N` speaker notes · `M` slide list · `Home` / `End`
