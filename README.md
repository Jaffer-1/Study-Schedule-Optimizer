# Study Schedule Optimizer (0/1 Knapsack) 📚

A web-based tool designed to help students maximize their exam performance. By treating study subjects as "items" in a knapsack, the application uses **Dynamic Programming** to determine exactly which subjects to study within a limited time frame to achieve the highest possible marks.

## ✨ Key Features
*   **Optimal Task Selection:** Uses the 0/1 Knapsack algorithm to find the mathematically best study plan.
*   **DP Table Visualization:** Generates a real-time heat map and "backtracking path" showing exactly how the algorithm calculated the result.
*   **Dynamic Task Management:** Add, delete, and modify subjects, hours, and marks weightage on the fly.
*   **Efficiency Analytics:** Displays total marks, hours utilized, and overall time efficiency.

## 🧪 The Algorithm: 0/1 Knapsack
Unlike the Greedy approach (which picks the best ratio first), this project uses **Dynamic Programming (DP)**. This ensures a global optimum by considering whether to include or exclude each task based on previously calculated sub-problems.

**The Recurrence Relation:**
For a task $i$ with weight $w_i$ and value $v_i$:
$$dp[i][j] = \max(dp[i-1][j], v_i + dp[i-1][j - w_i])$$

**Complexity:**
*   **Time Complexity:** $O(n \times W)$, where $n$ is the number of tasks and $W$ is the total study hours.
*   **Space Complexity:** $O(n \times W)$ to store the DP table.

## 📂 File Structure
*   `index.html`: The user interface and task input forms.
*   `style.css`: Modern, responsive styling with Inter typography.
*   `app.js`: Handles state management, UI events, and table rendering.
*   `dp.js`: Contains the core Dynamic Programming and Greedy comparison logic.

## 🛠️ Setup
1.  Clone the repository.
2.  Open `index.html` in your browser.
3.  No external dependencies or installations are required!

---
* Built by Jaffer Shaik - AP24110011174
* Course: Coding Skills - II (B.Tech-CSE, 4th Semester)
* Submission Date: April 30, 2026
