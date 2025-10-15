# 📊 Product Mix Optimization using Linear Programming

This project demonstrates how to solve a classic **Product Mix Optimization** problem using **Linear Programming** in Python, with the help of the [PuLP](https://coin-or.github.io/pulp/) library.

## 🧩 Problem Statement

A factory manufactures two products: **Product A** and **Product B**. Each product requires certain amounts of **material** and **labor**, both of which are limited resources. The objective is to determine the optimal number of units of each product to produce in order to **maximize total profit**, while not exceeding the available resources.

### 🔧 Problem Details

| Resource  | Requirement per Unit A | Requirement per Unit B | Availability |
|-----------|------------------------|-------------------------|--------------|
| Material  | 2 units                | 1 unit                  | 100 units    |
| Labor     | 1 unit                 | 2 units                 | 80 hours     |
| Profit    | $40                    | $30                     | —            |

---

## ✅ Solution Approach

The problem is modeled as a **Linear Programming (LP)** problem:

- **Decision Variables**:
  - `xA`: units of Product A to produce
  - `xB`: units of Product B to produce

- **Objective Function**:
  - Maximize `40 * xA + 30 * xB`

- **Constraints**:
  - `2 * xA + 1 * xB ≤ 100` (Material)
  - `1 * xA + 2 * xB ≤ 80` (Labor)
  - `xA, xB ≥ 0`

The problem is solved using the **CBC Solver** via the PuLP library.

---

## 📦 Dependencies

- Python 3.x
- [PuLP](https://pypi.org/project/PuLP/)
- Pandas
- Matplotlib

You can install the dependencies using:

``bash
pip install pulp pandas matplotlib

How to Run

Clone the repository:

git clone https://github.com/yourusername/product-mix-optimization.git
cd product-mix-optimization


Run the notebook:
Open Product_Mix_Optimization.ipynb in Jupyter Notebook or any supported IDE.

View results:

Optimal number of units to produce

Maximum profit

Bar chart of optimal production mix

📊 Visualization:C:\Users\Sitharam Chowdary\OneDrive\Pictures
