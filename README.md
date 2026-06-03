# Capstone2025

## 🚗 Dynamic Parking Pricing System  
A real-time parking pricing system that adjusts prices based on demand, occupancy, and various environmental factors using streaming data processing.

---

## 🚀 Overview  
This project implements two dynamic pricing models for parking lots:

- **Model 1**: Baseline Linear Model with time-based and occupancy-based pricing  
- **Model 2**: Advanced Demand-Based Model with a multi-factor pricing algorithm  

The system processes real-time parking data and generates dynamic prices to optimize parking lot utilization and revenue.

---

## 🛠️ Tech Stack  

### Core Technologies
- **Python 3.x** – Primary programming language  
- **Pathway** – Stream processing framework for real-time data  
- **Pandas** – Data manipulation and analysis  
- **NumPy** – Numerical computing  

### Visualization & Analysis
- **Bokeh** – Interactive visualization library  
- **Google Colab** – Development environment  

### Data Processing
- **CSV Ingestion** – Real-time data input  
- **Streaming Pipelines** – Continuous data processing using Pathway  

---

## 📊 Architecture Flow  

### Model 1: Baseline Linear Model  
`Raw Data → Schema Validation → Time Features → Price Calculation → Visualization`

### Model 2: Demand-Based Model  
`Raw Data → Schema Validation → Multi-Factor Analysis → Demand Calculation → Price Optimization → Visualization`

---

### 🏗️ System Architecture 

                ┌──────────────┐  
                │ CSV Dataset  │  
                └─────┬────────┘  
                      │  
              ┌───────▼────────┐  
              │ Pathway Schema │  
              └───────┬────────┘  
                      │  
          ┌───────────▼───────────┐  
          │  Enrichment & Features│  
          └───────┬─────┬─────────┘  
                  │     │  
         ┌────────▼┐   ┌▼──────────────┐  
         │ Model 1 │   │ Model 2       │  
         │ Baseline│   │ Demand-Based  │  
         └────┬────┘   └────┬──────────┘  
              │             │  
       ┌──────▼──────┐ ┌────▼───────┐  
       │ model1.csv  │ │ model2.csv │  
       └──────┬──────┘ └────┬───────┘  
              │             │  
     ┌────────▼─────────┐ ┌─▼────────────┐  
     │ Bokeh Plots HTML │ │ Bokeh Plots  │  
     └──────────────────┘ └──────────────┘  
     
---

## 📁 Files  

| File                    | Description                                        |
|-------------------------|----------------------------------------------------|
| `dataset.csv`           | Dataset provided to us and used in both models     |
| `model1_code.ipynb`     | Complete code for Model 1                          |
| `model2_code.ipynb`     | Complete code for Model 2                          |
| `model1_plot.html`      | Bokeh visualization output for Model 1             |
| `model2_plot.html`      | Bokeh visualization output for Model 2             |
| `model1_result.csv`     | Output of Model 1 used for plotting                |
| `model2_result.csv`     | Output of Model 2 used for plotting                |
| `model1_backupplot.jpg` | Plot for model 1 in case html file doesnt work     |
| `model2_backupplot.jpg` | Plot for model 2 in case html file doesnt work     |

