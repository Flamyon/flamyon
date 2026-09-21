# Francisco Rodríguez-Carretero — quant research in training

Software engineer (BSc, Universidad de Sevilla, 2026) doing an MSc in Quantitative Finance and
Computational Methods, and a research fellow at IMUS working on interval-valued multi-objective
optimisation. I like problems where the honest answer is a measured number with an interval
around it, and I build the tooling to get that number reproducibly.

**Looking for:** quant research / quant developer internships and graduate roles, 2026–27.

## Research

**Forecasting Bitcoin realised volatility from high-frequency data** — BSc thesis, 9/10
[`btc-volatility`](https://github.com/Flamyon/btc-volatility/tree/tfg-final) ·
[`mvp-web`](https://github.com/Flamyon/mvp-web) · [live demo](https://mvp-web-tfg.streamlit.app/)
- 245k BTCUSDT 5-minute candles (Binance, 2024–26); target is one-hour-ahead log realised variance.
- Persistence, BIC-selected AR(49), intraday HAR-logRV and a kNN predictor in a Takens-reconstructed
  state space, evaluated walk-forward on a chronological split with label purging.
- HAR-logRV wins (RMSE 0.861, R²_OOS 0.54 vs 0.40 for persistence). The kNN cuts persistence RMSE
  by 10 % but does not beat the linear benchmarks.
- Surrogate-data tests (shuffled, phase-randomised, AAFT) and a logistic-map control: no evidence of
  low-dimensional deterministic chaos. Every estimator (ADF/KPSS, BDS, correlation dimension,
  Lyapunov, permutation entropy) implemented from scratch.

**Interval preference orders in multi-objective optimisation** — PI3 research fellowship, IMUS,
Universidad de Sevilla (06/2026 – present)
- How does the choice of order on intervals change the efficient set? Closed-form efficient sets
  under three orders for a two-variable problem and two published interval-native problems; a
  strict nesting on one of them and a counterexample to a published optimality claim.
- 540 seeded NSGA-II / MOPSO-CD / random-search runs (pymoo) on interval-valued ZDT1 and DTLZ2:
  sampling-based overlap overstates the exact value (0.19 vs 0.10), and NSGA-II covers the efficient
  set worse than uniform sampling under two of the three orders.
- 1,000+ tests; predictions registered before each run. Code and write-up to be released after the
  September 2026 review.

**Face recognition, deepfakes and latent-space generative models** — research student, IMSE-CNM
(CSIC), 02–04/2026. Literature survey and internal seminars on embedding interpretability and
diffusion autoencoders; an LBP face-recognition demo and a bibliometric analysis of 16.5k deepfake
papers from the OpenAlex API.

## Projects

**[othello-mcts-zero](https://github.com/Flamyon/othello-mcts-zero)** — Othello engine with a
self-play value network. Bitboard rules (numba, 225k playouts/s), UCT MCTS, 28k-parameter value
net trained by gated iterated self-play, seeded colour-balanced arena with Wilson intervals.
Five generations take the win rate against 4-ply α–β minimax from 25 % (pure MCTS) to 44 %
(n = 400); 96 % against pure MCTS at equal playouts. Not at parity yet, and the README says so.

**MarketScope** — Streamlit dashboard for exploring financial time series with configurable
backtests of simple strategies.

## Competitions

Spanish Mathematical Olympiad, 1st place in the Córdoba regional round (2022) ·
Jane Street monthly puzzles, several top-10 finishes · Project Euler, +100 problems solved.

## Tools

Python (NumPy, pandas, statsmodels, scikit-learn, PyTorch/TensorFlow, numba), R, SQL, C++, Java,
Git, Linux, LaTeX. Volatility modelling (realised variance, HAR, AR), nonlinear time-series analysis,
walk-forward validation, multi-objective metaheuristics.

Spanish (native) · English (C1) · French (B1)

[LinkedIn](https://www.linkedin.com/in/franciscorcr/) · [franrodriguezcarretero@gmail.com](mailto:franrodriguezcarretero@gmail.com)
