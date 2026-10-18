<p align="center">
  <img src="logo.png" alt="Vi Rock Chess Logo" width="250"/>
</p>

<h1 align="center">Vi Rock Chess (VRC)</h1>
<p align="center"><i>Formerly known as Vinu Chess Zero (VC0)</i></p>
<p align="center">A chess engine built from scratch in C++ on Android (Termux).</p>

---

## 📖 About

**Vi Rock Chess** is the direct descendant of Vinu Chess Zero. What started as a 5-day experiment on an Android phone using Termux has evolved into a dedicated open-source chess engine project.

Our goal is to build a fast, stable, and highly competitive engine, progressing from classic Alpha-Beta search to Bitboards and eventually integrating Neural Networks (NNUE).

## 🚀 Features (Current - v1.0)

*   **Search**: Alpha-Beta + Iterative Deepening
*   **Quiescence Search**: Avoids the horizon effect
*   **Transposition Table**: Zobrist hashing (1M entries)
*   **Move Ordering**: MVV-LVA + Killer + History
*   **Evaluation**: Material + Full Piece-Square Tables (PST)
*   **Opening Book**: 50+ common opening lines
*   **Protocol**: UCI compatible

## 📈 Strength

| Opponent | Result |
| :--- | :--- |
| Stockfish level 5 | Win (2x) |
| Stockfish level 6 | Loss |
| **Estimated ELO** | **~2050** |

## 🛠️ How to Build

To compile the engine on Termux or any Linux environment:

```bash
# Clone the repository
git clone https://github.com/ctrandinh485-del/Vi-Rock-Chess.git

# Navigate to the directory
cd Vi-Rock-Chess

# Compile with clang++ (optimized)
clang++ -O3 -march=native main.cpp -o vrc

# Run the engine
./vrc
