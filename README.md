# 🔍 DFA Minimization Visualizer

A web-based tool to visualize and minimize Deterministic Finite Automata (DFA) using the partitioning algorithm.

![DFA Visualization Example](https://via.placeholder.com/800x400?text=DFA+Visualization+Screenshot)

## ✨ Features

- 🖥️ Interactive DFA visualization with states and transitions
- ⚡ DFA minimization using the partitioning algorithm
- 🔄 Toggle between original and minimized DFA views
- 📋 Sample DFA loading for quick demonstration
- 📊 Information panel showing DFA details and state mappings

## 🚀 How to Use

1. **Enter DFA Details**:
   - 📌 States (comma separated, e.g., `q0, q1, q2`)
   - 🔤 Alphabet symbols (comma separated, e.g., `0, 1`)
   - 🏁 Start state
   - 🎯 Final states
   - ➡️ Transitions (one per line in `state,symbol,next_state` format)

2. **Click "Create DFA"** to visualize your automaton

3. **Click "Minimize DFA"** to see the minimized version

4. **Toggle between** the original and minimized views using the tabs

## 🛠️ Technologies Used

- 🌐 HTML5, CSS3, JavaScript
- 🎨 Custom visualization with CSS and absolute positioning
- ⚙️ Partitioning algorithm for DFA minimization

## 📚 Theoretical Background

The tool implements the **table-filling algorithm** (also known as Moore's algorithm) for DFA minimization:

1. **Initial Partition**: Split states into final and non-final groups
2. **Refinement**: Repeatedly split groups where states have transitions to different partitions
3. **Termination**: When no more splits are possible
4. **Construction**: Build new DFA with merged equivalent states

## 📋 Sample Input

Use the "Load Sample" button to try a pre-configured DFA or enter:
States: q0, q1, q2, q3, q4
Alphabet: 0, 1
Start State: q0
Final States: q3, q4
Transitions:
q0,0,q1
q0,1,q2
q1,0,q1
q1,1,q3
q2,0,q1
q2,1,q2
q3,0,q4
q3,1,q2
q4,0,q1
q4,1,q3



## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

Made with ❤️ by Kartikeya Kesarwani.
