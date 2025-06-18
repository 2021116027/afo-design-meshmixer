# afo-design-meshmixer
# 🦿 Ankle-Foot Orthosis (AFO) Design & Finite Element Analysis using COMSOL

## 📚 Project Overview
This project focuses on the design and finite element analysis (FEA) of an Ankle-Foot Orthosis (AFO) to support individuals with spinal cord injuries. The orthosis is designed using **Meshmixer** and structurally analyzed using **COMSOL Multiphysics** to assess its durability, stress distribution, and deformation under realistic loading conditions.

---

## 🛠️ Tools & Technologies
- Meshmixer (AFO Design)
- COMSOL Multiphysics (Finite Element Analysis)
- STL 3D Modelling
- Biomedical Simulation
- Carbon Fiber Composite Material

---

## 🔧 Key Design Steps (Meshmixer)
1. **Import STL File** – Optimized scanned leg model
2. **Trim Lines** – Drawn along ankle and foot region
3. **Smooth Boundaries & Extrude AFO** – 4mm thick orthosis created
4. **Separate AFO from Leg**
5. **Edge Refinement** – Using Sculpt & Smooth
6. **Final Extrusion for Strength**
7. **Export as STL for FEA**

---

## 🧪 Finite Element Analysis (COMSOL)

### 🔹 Domain Partitioning:
- 3 Regions: Shank, Ankle, and Foot

### 🔹 Material Used:
- **Carbon Fiber Epoxy Composite**
  - Young’s Modulus: 7 GPa
  - Poisson’s Ratio: 0.28
  - Density: 1600 kg/m³
  - Shear Modulus: 5 GPa

### 🔹 Simulation Setup:
- Fixed constraint: Foot region
- Loads applied:
  - Shank: 700 N
  - Ankle: 1000 N
  - Foot: Cyclic load – 700 × sin(2πt)

### 🔹 Mesh:
- Free tetrahedral mesh, normal element size

---

## 📊 Simulation Results

### 📍 Stationary Study:
- Max displacement: 1.09 nm (very low, material won't yield)

### 📍 Cyclic Load Study:
- Max von Mises
