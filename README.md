# 🎯 Hard Target Auto – WindCube Scanning

---

## 🧭 General Project Presentation

The **Hard Target Auto** project aims to develop a semi-automatic workflow for **WindCube Scanning LiDAR systems**.

Its purpose is to assist users during field interventions by guiding them step by step to:

- 🎯 identify **static hard targets**
- 📐 refine their **angular position**
- 🧭 compute the **LiDAR north offset** in a reliable and repeatable way

The process is **human-in-the-loop**, meaning the user validates every critical step to ensure robustness and field reliability.

---

## 🚀 Project Objectives

- Detect **static hard targets** (buildings, masts, antennas, terrain)
- Initialize scans using **GPS-based approximations**
- Validate hard target visibility through **CNR analysis**
- Refine azimuth and elevation using **iterative scans**
- Compute angular quantities used for alignment
- Compute the **LiDAR north offset**
- Reduce manual trial-and-error during field operations
- Produce results reusable in **WindForge / OpenGen**

---

## 🔁 Hard Target Auto – High-Level Workflow

> The workflow progressively converges toward an accurate hard target alignment.

1. 📍 User inputs approximate GPS coordinates of a hard target  
2. 🧮 Geographic **azimuth, elevation, and range** are computed  
3. 🔄 A **PPI scan** is launched around the estimated azimuth  
4. 📊 A **CNR analysis** checks hard target visibility  
5. ⚠️ If no target is detected, the user verifies GPS inputs  
6. 📦 A **wide azimuth/elevation volume scan** is launched  
7. 📈 Hard target visibility is displayed *(elevation vs azimuth)*  
8. ✅ User confirms hard target visibility  
9. 🎛️ User refines azimuth, elevation, and resolution  
10. 🔍 Narrower volume scans are launched iteratively  
11. ✔️ User validates the final hard target position  
12. 📐 Angular quantities are computed  
13. 🧭 The **LiDAR north offset** is calculated and displayed  

---

## 📚 Variable List (Shared Variable Library)

The following variables are shared across the **workflow**, **calculations**, and **UI**.  
They represent the internal state of the Hard Target Auto process and are updated at runtime.

### 🧮 Angular Variables


---

### 🌍 Geographic Variables


---

### 🧠 Runtime / Session Variables


---

## 🧰 Git / GitHub Command List

### 📥 Clone the repository
```bash
git clone <repository-url>
```

### Check repository status
```bash
git status
git branch
git remote -v
```
### Create a new feature branch
```bash
git checkout -b feature/my-feature
```
### Commit changes
```bash
git add .
git commit -m "Meaningful commit message"
```
### Push a branch to GitHub
```bash
git push -u origin feature/my-feature
```
### Update local branch from main or dev
```bash
git checkout dev
git pull
```
### Switch branches
```bash
git checkout main
git checkout dev
```

