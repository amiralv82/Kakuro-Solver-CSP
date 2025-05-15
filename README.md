🧠 Kakuro Puzzle Solver

This project implements an AI-based Kakuro Puzzle Solver using backtracking search, optionally enhanced with heuristics like the Least Constraining Value (LCV) and Minimum Remaining Values (MRV). It is designed to run in Google Colab, allowing interactive puzzle solving with selectable difficulty levels and solving strategies.

📌 Features

	•	✅ Solves Kakuro puzzles using backtracking search
	•	🧩 Supports multiple difficulty levels: Easy, Medium, Hard, Expert
	•	⚙️ Optional heuristics:
	•	Standard Backtracking
	•	LCV (Least Constraining Value)
	•	🔍 Smart clue selection using MRV heuristic
	•	📉 Visualizes the puzzle grid after each assignment

🧱 How It Works

	1.	The puzzle is built using a combination of:
	•	Black cells (unusable)
	•	Clue cells (define target sums for rows/columns)
	•	White cells (fillable with digits 1–9)
	2.	The agent uses backtracking to explore potential values that satisfy all constraints.
	3.	With heuristics enabled, the solver prioritizes clues and values that are least restrictive.

▶️ Run in Google Colab

Or manually:

	1.	Upload the .py file or paste the code into a new Colab notebook.
	2.	Run the notebook cell.
	3.	Follow the console prompts to select:
	•	Difficulty level (1–4)
	•	Heuristic method (1–2)

🧪 Example Usage


When you run the notebook, you’ll be prompted like this:


Choose a level:

1. Easy
2. Medium
3. Hard
4. Expert

Enter the number of the level: 1

Choose a heuristic:
1. Standard Backtracking Search
2. Backtracking Search with Least Constraining Value (LCV) heuristic
Enter the number of the heuristic: 2

Then the puzzle is solved step-by-step, printing the board after each change.

📁 Project Structure

kakuro_solver/

├── kakuro_solver.py   # Full source code with puzzle setup and solver logic

├── README.md          # Project overview and usage instructions

🧠 Algorithms & Heuristics

	•	Backtracking Search: Tries possible values recursively with rollback on conflict
	•	MRV (Minimum Remaining Values): Prioritizes clues with fewer unknowns
	•	LCV (Least Constraining Value): Prefers values that allow more future options

🛠 Requirements

No external libraries are needed. Everything is built using Python 3’s standard library.

🏗️ TODO / Extensions

	•	Add more levels and randomized puzzles
	•	Export solved puzzles
	•	Implement forward checking
	•	Visual GUI for puzzles

👨‍💻 Author

Developed by Amir-abbas Alvand.
