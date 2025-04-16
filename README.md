# 👋 Hey there, I'm Karan

🔬 I’m currently diving into **Molecular Dynamics (MD)**  
⚛️ Passionate about simulating systems using **GROMACS**  
📊 Exploring post-processing and analysis with **TRAVIS**  
🧠 Learning, building, and contributing in the world of computational science

---

> “In the middle of difficulty lies opportunity.” – *Albert Einstein*

---

<!-- Badges (optional, feel free to add more) -->
![MD](https://img.shields.io/badge/Molecular-Dynamics-blueviolet)
![GROMACS](https://img.shields.io/badge/GROMACS-Simulation-blue)
![Python](https://img.shields.io/badge/Python-Scientific-yellow)

<!-- Optional: GitHub Stats (shows activity, stars, etc.) -->
<!-- Make sure to replace `username` with your actual GitHub username -->
<!-- Uncomment below if you want to use it -->

<!--
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=username&show_icons=true&theme=tokyonight)
-->


# 🧬 GROMACS MDP Files

This repository contains `.mdp` input files for running Molecular Dynamics simulations using **GROMACS**. These are standard templates for:

- ⚙️ Energy Minimization (`em.mdp`)
- 🌡 NVT Equilibration (`nvt.mdp`)
- 🧊 NPT Equilibration (`npt.mdp`)
- 🚀 Production MD (`md.mdp`)
- 💧 Ionization (`ions.mdp`)

---

## 📂 Files Overview

| File       | Purpose                          |
|------------|----------------------------------|
| `em.mdp`   | Minimizes system energy          |
| `nvt.mdp`  | Equilibrates temperature (NVT)   |
| `npt.mdp`  | Equilibrates pressure (NPT)      |
| `md.mdp`   | Full MD production run           |
| `ions.mdp` | Ion addition/neutralization      |

---

## 📥 Usage

Modify the files to fit your simulation system, then run using GROMACS:

```bash
gmx grompp -f md.mdp -c input.gro -p topol.top -o md.tpr
gmx mdrun -deffnm md
