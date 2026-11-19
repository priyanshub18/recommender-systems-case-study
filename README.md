# How Recommender Systems Work: A Graph Theory View

An animated, step-by-step slide deck for a college seminar. It explains how recommender systems work using graph theory — covering bipartite modelling, collaborative filtering via length-3 paths, random walks (Personalized PageRank), and content-based attribute nodes — with Netflix as a concrete running example.

**Live:** https://priyanshub18.github.io/recommender-systems-case-study/

## Slides
1. **Title:** How Recommender Systems Work (A Graph Theory View)
2. **Introduction:** Why every platform (Amazon, Spotify, YouTube, Netflix) needs a recommender system
3. **Graph theory in one minute:** Vertex, edge, degree, path
4. **Modelling:** Representing user–item interactions as a bipartite graph $G = (U, I, E)$, illustrated with a Netflix example
5. **Method 1 — Collaborative Filtering:** How length-3 paths discover recommendations (*"Because you watched Dark"*)
6. **Ranking Candidates:** Counting length-3 paths and the linear algebra link ($\mathbf{B}\cdot\mathbf{B}^T\cdot\mathbf{B}$)
7. **Scaling Up:** Random walks with restart / Personalized PageRank (live 100,000-step simulation)
8. **Method 2 — Content-Based Filtering:** Solving the cold-start problem by adding attribute vertices (creators, genres)
9. **System Architecture:** The 4-stage production recommender pipeline (Collect $\to$ Build Graph $\to$ Retrieve $\to$ Rank & Serve)
10. **Critical Evaluation:** Popularity bias, filter bubbles, and privacy
11. **Conclusion:** Key takeaways, academic references, and Q&A

## Controls
`Space` / `→` next · `←` back · `F` fullscreen · `N` speaker notes · `M` slide list · `Home` / `End`

Deep link to a slide and step: `#6.3`. Layout self-test: `?check`.
