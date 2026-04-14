# 🌍 Life Expectancy Prediction using Decision Trees & Random Forests

[![Python 3.13](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.6.0-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Project Overview

This project explores the application of tree-based machine learning models to predict a country's overall life expectancy (`Both_LE`) using female and male life expectancy data. It demonstrates key concepts in decision tree modeling, ensemble methods, and model evaluation through a real-world dataset of 199 countries.

The notebook provides a comprehensive, step-by-step guide to building, evaluating, and optimizing tree-based models with practical insights into overfitting, hyperparameter tuning, and feature importance analysis.

## 🎯 Key Objectives

- Build and compare **Decision Tree** and **Random Forest** classifiers
- Visualize and interpret decision tree structures for better understanding
- Address **overfitting** through depth constraints and ensemble methods
- Perform **hyperparameter tuning** using GridSearchCV
- Analyze **feature importance** for model interpretability
- Apply cross-validation for robust performance evaluation

## 📊 Dataset

The dataset contains life expectancy statistics for **199 countries** with the following features:

| Column | Description |
|--------|-------------|
| `Country` | Country name |
| `Female_LE` | Female life expectancy (years) |
| `Male_LE` | Male life expectancy (years) |
| `Both_LE` | Overall life expectancy (target variable) |

**Target Classes** (created via quantile binning):
- 🟢 **Low**: < 71.3 years
- 🟡 **Medium**: 71.3 – 77.6 years  
- 🔴 **High**: > 77.6 years

The dataset is balanced with approximately 66 countries in each class, making it ideal for classification tasks.

## 🧠 Models Implemented

| Model | Description | Training Acc | Test Acc |
|-------|-------------|--------------|----------|
| **Decision Tree (Full)** | Unconstrained tree – demonstrates overfitting | 100.00% | 92.50% |
| **Decision Tree (Depth=3)** | Depth-limited tree – more interpretable | 98.11% | 92.50% |
| **Random Forest (Default)** | 100-tree ensemble – reduces variance | 100.00% | 97.50% |
| **Random Forest (Optimized)** | Tuned via GridSearchCV – best balance | 99.37% | **95.00%** |

## 📈 Results Summary

### Performance Comparison
