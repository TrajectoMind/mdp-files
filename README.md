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
