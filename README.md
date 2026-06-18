# 🌾 FoodBridge - NGO Food Supply Network

[![C++](https://img.shields.io/badge/C++-17-blue.svg)](https://isocpp.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Leaflet](https://img.shields.io/badge/Leaflet-1.9.4-green.svg)](https://leafletjs.com/)
[![License](https://img.shields.io/badge/License-MIT-red.svg)](LICENSE)

> **An intelligent food distribution network using priority-based greedy algorithms to connect surplus food with those who need it most.**

---

## 🌟 Overview

**FoodBridge** is a comprehensive NGO food supply management system that optimizes food distribution using priority-based algorithms. The system connects food donors (hostels, restaurants, events) with NGOs, ensuring that food reaches the most urgent beneficiaries first.

### 🎯 Problem Statement
- Food wastage is a global issue
- NGOs often lack efficient distribution systems
- Manual allocation is time-consuming and suboptimal

### 💡 Solution
- Automated priority calculation based on urgency and beneficiaries
- Greedy allocation algorithm for optimal food distribution
- Interactive map interface for real-time NGO tracking
- C++ backend for high-performance computations

---

## ✨ Features

### 🗺️ Interactive Map (Dehradun - Clement Town)
- **Real-time NGO visualization** with color-coded markers
- **Priority-based coloring**:
  - 🟣 Purple - Newly added NGOs
  - 🔴 Red - High priority (800+ score)
  - 🟡 Orange - Medium priority (500-799)
  - 🟢 Green - Low-medium priority (300-499)
  - 🔵 Blue - Low priority (<300)
- **Locality labels** for easy identification
- **Click to view** complete NGO details
- **Zoom and pan** for detailed exploration

### 🏢 NGO Management
- ✅ **Valid NGO verification** - Only pre-approved NGOs can register
- 📊 **Priority score calculation** using C++ algorithms
- 🔍 **Search and filter** functionality
- 📋 **Sortable table** with all NGO details
- 🗑️ **Delete NGOs** from the system

### 🍱 Food Donation Management
- 📝 **Record donations** from suppliers
- 📊 **Track food stock** in real-time
- 📈 **View donation history** with timestamps

### ⚡ Allocation Engine
- 🎯 **Greedy allocation algorithm** (O(n) time complexity)
- 📊 **Multiple sorting algorithms**:
  - QuickSort - O(n log n)
  - MergeSort - O(n log n)
  - HeapSort - O(n log n)
  - BubbleSort - O(n²)
  - SelectionSort - O(n²)
  - InsertionSort - O(n²)
- 📈 **Real-time allocation results** with status
- 📊 **Efficiency metrics** and summaries

### 📋 Reports & Analytics
- 📄 **Generate comprehensive reports**
- 📊 **System statistics** dashboard
- 📈 **Complexity analysis** visualization
- 🖨️ **Print reports** for documentation

---

## 🛠️ Tech Stack

### Backend
| Technology | Version | Purpose |
|------------|---------|---------|
| C++ | 17 | Core algorithms and server logic |
| cpp-httplib | Latest | HTTP server for API endpoints |
| JSON | - | Data interchange format |

### Frontend
| Technology | Version | Purpose |
|------------|---------|---------|
| HTML5 | - | Structure |
| CSS3 | - | Styling and animations |
| JavaScript | ES6 | Frontend logic and interactivity |
| Leaflet | 1.9.4 | Interactive maps |
| OpenStreetMap | - | Map tiles |

### Algorithms Implemented
| Algorithm | Type | Complexity |
|-----------|------|------------|
| Priority Calculator | Custom | O(n) |
| Greedy Allocation | Greedy | O(n) |
| QuickSort | Sorting | O(n log n) |
| MergeSort | Sorting | O(n log n) |
| HeapSort | Sorting | O(n log n) |
| BubbleSort | Sorting | O(n²) |
| SelectionSort | Sorting | O(n²) |
| InsertionSort | Sorting | O(n²) |
| Binary Search | Search | O(log n) |
| Linear Search | Search | O(n) |

---

## 🏗️ Architecture
┌─────────────────────────────────────────────────────────────┐
│ FRONTEND (Browser) │
├─────────────────────────────────────────────────────────────┤
│ index.html │ style.css │ app.js │ Leaflet Map │
├─────────────────────────────────────────────────────────────┤
│ HTTP API Calls │
├─────────────────────────────────────────────────────────────┤
│ C++ BACKEND SERVER (cpp-httplib) │
├─────────────────────────────────────────────────────────────┤
│ ApiHandler │ PriorityCalculator │ GreedyAllocation │
│ SortAlgorithms │ NGO │ AllocationResult │
├─────────────────────────────────────────────────────────────┤
│ DATA STORAGE │
├─────────────────────────────────────────────────────────────┤
│ Memory (Vector) │ JSON Serialization │
└─────────────────────────────────────────────────────────────┘

---


### Data Flow
1. **User Action** → Frontend JavaScript
2. **API Request** → HTTP call to C++ server
3. **Processing** → C++ algorithms compute results
4. **Response** → JSON data returned to frontend
5. **Display** → Frontend updates UI with results

---

## 🚀 Installation

### Prerequisites
- **C++ Compiler** (GCC 7+ or MSVC 2019+)
- **Git** (for cloning)
- **Web Browser** (Chrome, Firefox, Edge)

### Step 1: Clone Repository
git clone https://github.com/r20j/foodbridge.git
cd foodbridge


### Step 2: Download dependencies
Download cpp-httplib
git clone https://github.com/yhirose/cpp-httplib.git

Create frontend directory
mkdir -p frontend

---
## 📁 Project Structure
text
foodbridge/
├── NGO_backend/
│   ├── main.cpp
│   ├── ApiHandler.cpp
│   ├── ApiHandler.h
│   ├── algorithm/
│   │   ├── GreedyAllocation.cpp
│   │   ├── GreedyAllocation.h
│   │   ├── PriorityCalculator.cpp
│   │   ├── PriorityCalculator.h
│   │   ├── SortAlgorithms.cpp
│   │   └── SortAlgorithms.h
│   ├── models/
│   │   ├── AllocationResult.cpp
│   │   ├── AllocationResult.h
│   │   ├── NGO.cpp
│   │   └── NGO.h
│   ├── cpp-httplib/
│   │   └── httplib.h
│   └── frontend/
│       ├── index.html
│       ├── style.css
│       ├── app.js
│       └── leaflet/
│           ├── leaflet.css
│           ├── leaflet.js
│           └── images/
│               ├── layers.png
│               ├── layers-2x.png
│               ├── marker-icon.png
│               ├── marker-icon-2x.png
│               └── marker-shadow.png
├── LICENSE
├── README.md
└── .gitignore

---

## 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
