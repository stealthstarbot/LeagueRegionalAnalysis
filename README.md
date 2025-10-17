# Regional Playstyle Analysis in League of Legends (2023–2025)

**Author:** Preston Jarvis  
**Date:** October 2025  

---

## Project Overview
This project analyzes **regional playstyle differences** in professional League of Legends (LoL) across the four main competitive regions: **LCS (NA), LEC (EU), LCK (KR), and LPL (CN)** from 2023 to 2025. The analysis focuses on metrics like **aggression, objective control, vision control, gold difference, and CS difference** to understand how each region approaches the early and mid-game.

---

## Motivations
I love playing League of Legends and have been for a while and recently stopped playing to focus on gaining employable skills and the first project I wanted to take up would be this. In general, different league regions show distinct playstyles just as we see different dialects based on regions with language I wanted to see how different regions interact with gaming, specifically League of Legends

---

## Dataset
The analysis uses **Riot/Oracle match datasets** for the years 2023, 2024, and 2025.  

- **Columns include:**  
  - `league`: Competitive league  
  - `year`: Match year  
  - `kills`, `deaths`, `dragons`, `barons`, `gold difference at 15 min`, `CS difference at 10 min`, `vision score per minute (VSPM)`, etc.  
- **Cleaning steps:**  
  - Combined datasets across years  
  - Filtered for relevant regions (LCS, LEC, LCK, LPL)  
  - Handled league naming inconsistencies (e.g., LCS → LTA N in 2025)  
  - Computed derived metrics: aggression, objective control, vision control, tempo  

---

## Tools & Libraries
- **R** (tidyverse, data.table, ggplot2, ggthemes, plotly)  
- **Tableau** (optional, for interactive dashboards)  

---

## Metrics Analyzed across R and Tableau
1. **Aggression** – `(Kills + Deaths) / Game Length`  
2. **Objective Control** – Total Dragons, Barons Secured
3. **Vision Control** – Wards placed, wards killed, control wards bought (weighted metric)  
4. **Gold Difference at 15 min** – Average lead or deficit at 15 minutes  
5. **CS Difference at 10 min** – Average creep score difference at 10 minutes  

---

## Usage Instructions
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/lol-regional-playstyle.git
