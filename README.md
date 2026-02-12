# Data Centre Management Optimization

A metaheuristic optimization project for managing server allocation across two data centres to maximize profits while meeting dynamic customer demand.

## 📋 Problem Overview

This project solves a resource management optimization problem involving:
- **Two data centres**: Low-latency and high-latency
- **Two server types**: CPU and GPU servers
- **Dynamic demand**: Changes at each time-step (known in advance)
- **Operations**: Buy, sell, and transfer servers between data centres
- **Objective**: Maximize total profit across all time-steps

### Key Challenge
Balance the trade-offs between:
- Server purchase costs vs. potential profit from meeting demand
- Transfer costs vs. strategic server placement
- Short-term gains vs. long-term optimization

## 🎯 Algorithms Implemented

This project implements and compares multiple metaheuristic optimization algorithms:

1. **Hill Climbing (Standard)** - Basic local search with first improvement
2. **Hill Climbing (Best Ascent)** - Evaluates all neighbors, selects best
3. **Simulated Annealing** - Probabilistic approach to escape local optima
4. **Genetic Algorithm** - Population-based evolutionary approach

### Experimental Setup
- **5 independent runs** per algorithm (random seeds: 0, 1, 2, 3, 4)
- **Multiple hyperparameter configurations** tested
- **Statistical comparison** of mean performance and variance

## 🛠️ Technologies

- **Python 3.x** (standard library only)
- **NumPy** - for numerical operations
- **Matplotlib** - for visualization
- **Jupyter Notebook** - for interactive development

## 🚀 Getting Started

### Prerequisites

Python 3.x with NumPy and Matplotlib:
```bash
pip install numpy matplotlib jupyter
```

### Running the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/data-centre-management.git
   cd data-centre-management
   ```

2. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook data_centre_management.ipynb
   ```

3. **Run all cells** to see the implementation and results

## 📊 Repository Contents

```
data-centre-management/
├── README.md                           # This file
├── data_centre_management.ipynb        # Main notebook with all code and analysis
└── data/
    ├── demand.npy                      # Dynamic demand data for each time-step
    └── data.txt                        # Economic parameters (costs, prices, profits)
```

## 📈 Results Highlights

The notebook includes:
- ✅ Complete implementation of all algorithms
- ✅ Comprehensive experimental comparison
- ✅ Performance visualizations and convergence plots
- ✅ Statistical analysis of results
- ✅ Discussion of algorithmic trade-offs

**Key Findings**: Full analysis and visualizations available in the notebook.

## 💡 Key Learnings

- Understanding trade-offs between exploration and exploitation in metaheuristics
- Importance of neighborhood design in local search algorithms
- Statistical rigor in algorithm comparison
- Real-world application of optimization in resource management

## 🎓 Academic Context

This project was completed as a university assignment exploring metaheuristic optimization techniques. The implementation demonstrates:
- Multiple standard optimization algorithms
- Custom problem-specific adaptations
- Rigorous experimental methodology
- Statistical validation and comparison

## 📝 Solution Representation

Solutions are represented as arrays of shape `(n × 2 × 2 × 3)`:
- `n`: Number of time-steps
- First `2`: Data centres (0=low-latency, 1=high-latency)
- Second `2`: Server types (CPU, GPU)
- `3`: Operations (buy, sell, transfer)

Each integer represents the quantity of that operation at that time-step.

## 🤝 Contributing

This is an academic project completed for coursework. Feel free to fork and experiment with your own ideas!

## 📄 License

© 2024 Vaibhav Tamta. For educational purposes.

## ✉️ Contact

**Vaibhav Tamta**
- GitHub: [@yourusername](https://github.com/yourusername)

---

*This project demonstrates the application of metaheuristic optimization algorithms to a real-world resource management problem.*
