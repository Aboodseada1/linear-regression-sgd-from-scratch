# Linear Regression with Stochastic Gradient Descent (SGD)

## 📋 Assignment Overview

This project implements **Assignment 1** for the AI course, which consists of two main tasks:

1. **10 Types of ML Optimizers** - Listed and explained in the PDF document
2. **Linear Regression Implementation** - Complete SGD implementation from scratch

## 🎯 Project Description

A comprehensive implementation of Linear Regression using Stochastic Gradient Descent (SGD) algorithm, built entirely from scratch without using any pre-built machine learning libraries. The implementation includes professional terminal output with colors, comprehensive visualizations, and detailed performance analysis.

## 📊 Dataset

The project uses `MultipleLR-Dataset.csv` containing:

- **25 samples** with **4 columns** total
- **3 input features** + **1 target variable**
- Format: `feature1,feature2,feature3,target`

### Sample Data Preview:

```
73,80,75,152
93,88,93,185
89,91,90,180
96,98,100,196
...
```

## 🚀 Features

### ✨ **Core Implementation**

- **Pure Python Implementation** - No external ML libraries
- **Stochastic Gradient Descent** - Complete SGD algorithm from scratch
- **Feature Normalization** - Min-max scaling to [0,1] range
- **Train/Test Split** - 80/20 data splitting
- **Performance Metrics** - R², MSE, MAE calculations

### 🎨 **Professional Interface**

- **Colored Terminal Output** - Professional ANSI color coding
- **Progress Indicators** - Real-time training progress
- **Status Messages** - Success/error indicators with emojis
- **Formatted Results** - Clean, organized output display

### 📈 **Comprehensive Visualizations**

- **Training Loss Plot** - Loss convergence over iterations
- **Predictions vs Actual** - Scatter plots for training and test sets
- **Residual Analysis** - Error pattern visualization
- **Feature Importance** - Bar chart of model weights
- **Professional Styling** - Consistent color scheme and formatting

## 🛠️ Installation & Setup

### Prerequisites

- Python 3.7+
- Required packages (see requirements.txt)

### Installation Steps

```bash
# Clone or download the project
# Navigate to project directory
# Install required packages
pip install -r requirements.txt
```

## 📖 Usage

### Professional Version (Recommended for Submission)

```bash
python main.py
```

- **Features**: Colored terminal output, comprehensive visualizations, professional interface
- **Best for**: Final submission, demonstration, professional presentation

### Simple Version (Recommended for Discussion)

```bash
python main_simple.py
```

- **Features**: Clean, simple output, educational comments, easy to explain
- **Data**: Uses ALL 25 samples for training (no train/test split)
- **Best for**: Academic discussion, lecturer questions, code explanation

### What Happens When You Run (Both Versions):

1. **📁 Data Collection** - Loads MultipleLR-Dataset.csv (25 samples, 4 columns)
2. **✂️ Data Preprocessing** - 80% training, 20% testing + feature normalization (main.py) OR all data for training (main_simple.py)
3. **🔍 Data Exploration** - Basic data analysis and understanding
4. **🎯 Model Selection** - Linear Regression with SGD algorithm
5. **🚀 Model Training** - SGD training with progress updates
6. **📊 Model Evaluation** - R², MSE, MAE metrics on train/test sets
7. **🔧 Model Optimization** - Hyperparameter tuning (learning rates)
8. **🎯 Sample Predictions** - Test set predictions with error analysis
9. **📈 Model Deployment** - **7 IMPRESSIVE visualizations** (main.py) or **text-only results** (main_simple.py)

### Expected Output:

```
============================================================
Linear Regression with Stochastic Gradient Descent
============================================================

[1] Loading data from MultipleLR-Dataset.csv...
    ✓ Loaded 25 samples with 3 features (4 columns total)

[2] Splitting data (80% train, 20% test)...
    ✓ Training samples: 20
    ✓ Testing samples: 5

[3] Normalizing features...
    ✓ Features normalized to [0, 1] range

[4] Training Linear Regression model...
Iteration 100/1000, Loss: 45.2341
Iteration 200/1000, Loss: 23.5678
...
    ✓ Model training completed!

============================================================
📊 RESULTS
============================================================

🔧 Model Parameters
  Weights: ['0.1234', '0.5678', '0.9012']
  Bias: 0.3456

📈 Training Performance
  R² Score: 0.8765
  MSE: 12.3456
  MAE: 2.7890

🎯 Testing Performance
  R² Score: 0.8234
  MSE: 15.6789
  MAE: 3.1234

🔍 Sample Predictions on Test Set
  Sample 1: Actual = 152.00, Predicted = 148.23, Error = 3.77
  Sample 2: Actual = 185.00, Predicted = 182.45, Error = 2.55
  ...

📊 Creating Visualizations...
  1. Plotting training loss...
  2. Plotting training predictions vs actual...
  3. Plotting test predictions vs actual...
  4. Plotting residuals...
  5. Plotting feature importance...
  ✓ All visualizations completed!

============================================================
🎉 Training completed successfully!
============================================================
```

## 📁 Project Structure

```
Assignment-1/
├── main.py                    # Professional implementation with colored terminal output
├── main_simple.py             # Simple version for academic discussion
├── MultipleLR-Dataset.csv     # Dataset file (25 samples, 4 columns)
├── Assignment-1.pdf          # Assignment document with optimizer explanations
├── README.md                 # This documentation file
└── requirements.txt          # Python dependencies
```

## 🔄 ML Pipeline Implementation

Both Python files follow the complete **9-step ML Pipeline**:

### 📋 **Pipeline Sequence:**

1. **Problem Definition** - Clear problem statement and requirements
2. **Data Collection** - Load MultipleLR-Dataset.csv (25 samples, 4 columns)
3. **Data Preprocessing** - Train/test split (80/20) + feature normalization
4. **Data Exploration & Visualization** - Data analysis and understanding
5. **Model Selection** - Linear Regression with SGD algorithm
6. **Model Training** - SGD implementation with progress monitoring
7. **Model Evaluation** - R², MSE, MAE metrics on train/test sets
8. **Model Optimization** - Hyperparameter tuning (learning rates)
9. **Model Deployment** - Comprehensive visualizations and predictions

### 🎯 **File Differences:**

| Feature                     | main.py                                        | main_simple.py                               |
| --------------------------- | ---------------------------------------------- | -------------------------------------------- |
| **Purpose**           | Professional submission                        | Academic discussion                          |
| **Terminal Output**   | Colored, emoji-rich                            | Simple text                                  |
| **Comments**          | Professional documentation                     | Educational explanations                     |
| **Visualizations**    | **7 IMPRESSIVE plots** (1 big dashboard) | **No plots** (text only)               |
| **Data Usage**        | **Train/test split** (20 train, 5 test)  | **All data for training** (25 samples) |
| **Code Organization** | Modular functions                              | Sequential execution                         |
| **Best For**          | Final submission                               | Lecturer discussion                          |

## 🔧 Technical Details

### Algorithm Implementation

- **SGD Algorithm**: Implements stochastic gradient descent with random sampling
- **Input Features**: 3 features from CSV columns 1-3
- **Target Variable**: 1 target from CSV column 4
- **Loss Function**: Mean Squared Error (MSE)
- **Learning Rate**: 0.01 (configurable)
- **Iterations**: 1000 (configurable)
- **Weight Initialization**: Random uniform distribution [-0.1, 0.1]

### Performance Metrics

- **R² Score**: Coefficient of determination
- **MSE**: Mean Squared Error
- **MAE**: Mean Absolute Error

### Visualization Features

- **Matplotlib Integration**: Professional plotting
- **Color Schemes**: Consistent blue/red/orange palette
- **Interactive Plots**: Separate windows for each visualization
- **Grid Layouts**: Clean, organized plot formatting

## 🎓 Assignment Requirements Fulfilled

### ✅ Task 1: 10 ML Optimizers

- **Document**: `Assignment-1.pdf`
- **Content**: 10 optimizer types with explanations
- **Format**: PDF document with detailed descriptions

### ✅ Task 2: Linear Regression Implementation

- **Implementation**: Complete SGD from scratch
- **No External ML Libraries**: Pure Python implementation
- **Dataset**: Uses provided MultipleLR-Dataset.csv
- **Features**: Professional interface, visualizations, comprehensive analysis

## 🚀 Advanced Features

### Customization Options

- **Learning Rate**: Adjustable in configuration section (`LEARNING_RATE = 0.01`)
- **Iterations**: Configurable training epochs (`N_ITERATIONS = 1000`)
- **Test Split Ratio**: Customizable train/test split (`TEST_SIZE = 0.2`)
- **Random Seed**: Reproducible results (`RANDOM_SEED = 42`)
- **Visualizations**: Enable/disable plots (`SHOW_PLOTS = True`)
- **Progress Updates**: Control training output frequency (`PRINT_PROGRESS_EVERY = 100`)

### Error Handling

- **File Not Found**: Graceful handling of missing dataset
- **Data Validation**: Checks for proper data format
- **Progress Monitoring**: Real-time training updates
- **Visualization Errors**: Fallback handling for plot issues

## 📊 Performance Analysis

The implementation provides comprehensive analysis including:

- **Training Convergence**: Loss reduction over iterations with visual tracking
- **Model Generalization**: Performance on unseen test data with comparison plots
- **Feature Analysis**: Importance of each input feature with exact weight values
- **Error Patterns**: Residual analysis for model improvement and diagnostics
- **Statistical Validation**: Multiple metrics (R², MSE, MAE) with visual comparisons
- **Hyperparameter Optimization**: Learning rate tuning with performance tracking

## 🎨 Visual Output

The program generates **7 IMPRESSIVE professional visualizations**:

### 📊 **Dashboard 1: Complete Analysis (7 plots in one figure)**

1. **📈 Training Loss Convergence** - Shows how your model learned over time with filled areas
2. **🎯 Training Set Performance** - Predictions vs actual (training data) with perfect prediction line
3. **🎯 Test Set Performance** - Predictions vs actual (test data) with perfect prediction line
4. **📊 Residual Analysis** - Shows error patterns and model quality diagnostics
5. **⚖️ Feature Importance** - Which features matter most with exact weight values displayed
6. **📈 Error Distribution** - Histogram showing prediction accuracy with mean error line

### 📊 **Dashboard 2: Performance Comparison**

7. **📊 Performance Metrics Comparison** - Training vs Test set comparison (R², MSE, MAE) with exact values

### ✨ **Professional Features:**

- **Color-coded plots** with professional color schemes
- **Emojis in titles** for visual appeal and modern look
- **Exact values displayed** on bars and plots for precision
- **Grid lines** for easy reading and professional appearance
- **Perfect prediction lines** for reference and validation
- **Filled areas** and **edge colors** for depth and visual impact
- **Multiple subplots** in organized, dashboard-style layout

## 📝 Notes

- **Reproducible Results**: Uses fixed random seed (42) for consistent outputs
- **Professional Output**: Colored terminal with emojis and modern formatting
- **Educational Value**: Clear, well-documented code for learning ML fundamentals
- **Complete Solution**: Handles entire ML pipeline from data loading to visualization
- **Impressive Visualizations**: 7 professional plots that showcase data science expertise
- **Configurable Settings**: Easy-to-modify parameters at the top of the file
- **Error Handling**: Robust error handling for missing files and visualization issues

## 👨‍💻 Author

**Student**: Abd El-Rahman Mahmoud Seada
**ID:** 201801343
**Course**: AI - Fall 2026

## 📄 License

MIT License
