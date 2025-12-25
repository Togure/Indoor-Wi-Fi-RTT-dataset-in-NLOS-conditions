# Indoor-Wi-Fi-RTT-dataset-in-NLOS-conditions
This is a Wi-Fi RTT dataset collected under severe NLOS conditions using Google Pixel 6 smartphones and Google Nest Wi-Fi access points. Due to signal blockage and multipath propagation, the RTT measurements are significantly impaired by NLOS effects, making this dataset particularly challenging and suitable for evaluating robust indoor
## 📍 Experimental Environment

The experiment was conducted in a **student hall** environment characterized by **severe NLOS conditions and strong multipath effects**.  
The measurement area includes three representative trajectories:

- **Lounge**
- **Corridor**
- **Suite**

- ## 📊 Dataset Structure

The dataset consists of the following components:

### 1. Access Point Locations (`AP`)
The positions of deployed Wi-Fi Access Points.

`{AP_X_coordinate | AP_Y_coordinate}`

Each row corresponds to one AP.

### 2. RTT Measurements (`RTToutput`)
RTT measurements collected from multiple APs.

`{measurement_index | timestamp | AP1_RTT | AP2_RTT | AP3_RTT}`

- `measurement_index`: index of the RTT measurement
- `timestamp`: measurement time
- `APi_RTT`: RTT value measured from the i-th AP

---

### 3. Ground Truth Trajectory (`GTLidar`)
Ground-truth user positions obtained using LiDAR-based tracking.

`{user_X_coordinate | user_Y_coordinate}`

Each entry corresponds to the true position of the user at the given measurement instance.

---

## ⚠️ Dataset Characteristics

- High proportion of **NLOS receptions**
- Strong **multipath propagation**
- Suitable for:
  - NLOS detection
  - Robust indoor localization
  - Visibility-aware positioning
  - RTT error modeling and mitigation

---
[trajectory.pdf](https://github.com/user-attachments/files/24334833/trajectory.pdf)


## 📖 Citation

If you use this dataset in your research, please cite the following paper:

[1] Lyu, S. Bai, X. Wang, L. Li, and G. Zhang, “Wi-fi rtt indoor positioning using visibility matching with nlos receptions,” IEEE Internet of Things Journal, vol. 12, no. 12, pp. 18 779–18 790, 2025.

[2] Lyu Z, Li L, Meng Q, et al. Improving Wi-Fi indoor positioning based on matching visibility with virtual simulation[C]//2024 14th International Conference on Indoor Positioning and Indoor Navigation (IPIN). IEEE, 2024: 1-6.
