### Overview
This repository provides **six shapefile folders** representing spatial decay-rate parameters for **six ground-motion intensity measures** across California:

- **PGA** (Peak Ground Acceleration)  
- **PGV** (Peak Ground Velocity)  
- **PSA(0.1 s)**  
- **PSA(0.3 s)**  
- **PSA(1.0 s)**  
- **PSA(3.0 s)**  

Each shapefile contains the **posterior mean** and **posterior standard deviation** of the spatial decay-rate parameter estimated for **322 grid cells** (each 50 km × 50 km) covering California.

---

### File Naming Convention
Shapefile folders are named as:

CA_cells_50_xx

where `xx` indicates the corresponding intensity measure (e.g., `pga`, `pgv`, `psa0p1`, `psa0p3`, `psa1`, `psa3`).

---

### Data Description
Each shapefile’s attribute table includes **eight columns**:

| Column Name | Description |
|--------------|-------------|
| `id`    | Unique identifier for each 50 km × 50 km grid cell |
| `left`, `top`, `right`, `bottom` | Bounding coordinates (in **WGS_1984_Web_Mercator** projection) |
| `lamb`       | Posterior mean of the spatial decay-rate parameter |
| `lamb_sd`    | Posterior standard deviation of the spatial decay-rate parameter |
| `cov`        | Coefficient of variation (`lamb_sd / lamb`) |

