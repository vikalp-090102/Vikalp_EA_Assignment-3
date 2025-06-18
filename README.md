# Vikalp_EA_Assignment-3
# Assignment Submission

**Author**: Vikalp Srivasatva  
**File**: `Vikalp_ASSIGNMENT_3_CODES.ipynb`  
**Platform**: Designed to run directly on Google Colab or Kaggle (no setup needed)

---

##  Question-1: Physics-Informed Neural Network (PINN) for Cardiac Activation Mapping

This question involves predicting cardiac activation times using sparse spatial samples. The problem is modeled with an Eikonal equation.

We implemented and compared three approaches:
- **Model 1**: Data-driven neural network trained only on observed values
- **Model 2**: Physics-Informed Neural Network (PINN), which includes a physics-based regularization loss
- **Baseline**: Linear interpolation using `scipy.griddata`

Each model was trained on just 30 Latin Hypercube sampled points, and evaluated over a full 2D domain. Results are presented with RMSE, MAE, contour plots, and error maps.

---

##  Question-2: Neural ODE vs. Feedforward Neural Network on a Classification Task

This question compares two models on the classic `make_moons` dataset:

- **Baseline**: A fully connected neural network with one hidden layer and ReLU activation
- **Neural ODE Model**: Uses a continuous transformation of hidden states by integrating an ODE defined with a neural network (via `torchdiffeq`)

The models are trained and evaluated on accuracy and decision boundaries. The experiment shows how Neural ODEs can offer smoother and more flexible decision regions.

---

##  How to Run the Code

No setup is needed! Just follow these steps:

1. **Open the notebook on Google Colab or Kaggle** (e.g. `assignment.ipynb`)
2. Make sure the runtime is set to Python with GPU if needed
3. Press **"Runtime → Run all"** (in Colab) or **"Run All"** (in Kaggle)
4. All code cells will execute in sequence, and the plots/results will appear automatically

---

##  Requirements

The notebook automatically installs or imports the following packages:
- `numpy`
- `torch`
- `matplotlib`
- `scikit-learn`
- `torchdiffeq` (installed via `pip` if not available)

No additional configuration is required.

---

## ⚠ Notes

- All results, plots, and performance summaries are generated inline in the notebook
- For reproducibility, random seeds are set
- The notebook is structured clearly with section titles and print statements

---

