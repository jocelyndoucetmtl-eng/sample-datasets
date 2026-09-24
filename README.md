# sample-datasets
Fluidmapper-Dual-Rushton-Sample-Dataset/
│
├── README.md
├── LICENSE.md
├── CITATION.cff
│
├── geometry/
│   ├── 20251015_Assembly_2_RUSHTON_50_MM_Agitator_Shaft.stl
│   ├── 20251015_Assembly_2_RUSHTON_50_MM-Cuve.stl
│   └── Tank_ellipse_50_mm_bottom_VOLUME-FEMMeshNetgen.vtu
│
├── datasets/
│   │
│   ├── 20251011_2_RUSHTON_300_RPM/
│   │   ├── Predicted_coordinates_and_stds.txt
│   │   ├── 20251011_094758_NN.vtu
│   │   └── post_processed_results/
│           ├── Mixing_Index/
│           ├── Distributions/
│           ├── Pumping/
│           ├── Velocity/
│           └── Wall Velocity Distributions/
│   │
│   ├── 20251012_2_RUSHTON_400_RPM/
│   │   ├── Predicted_coordinates_and_stds.txt
│   │   ├── 20251012_125920_NN.vtu
│   │   └── post_processed_results/
│           ├── Mixing_Index/
│           ├── Distributions/
│           ├── Pumping/
│           ├── Velocity/
│           └── Wall Velocity Distributions/
│   │
│   └── 20251013_2_RUSHTON_500_RPM/
│       ├── Predicted_coordinates_and_stds.txt
│       ├── 20251013_144508_NN.vtu
│       └── post_processed_results/
│           ├── Mixing_Index/
│           ├── Distributions/
│           ├── Pumping/
│           ├── Velocity/
│           └── Wall Velocity Distributions/
│
└── documentation/
    └── data_dictionary.md
    
| File | Description |
|---|---|
| `20251015_Assembly_2_RUSHTON_50_MM_Agitator_Shaft.stl` | STL geometry of the agitator assembly, including the shaft and dual 50 mm Rushton turbines |
| `20251015_Assembly_2_RUSHTON_50_MM-Cuve.stl` | STL geometry of the stirred-tank vessel |
| `Tank_ellipse_50_mm_bottom_VOLUME-FEMMeshNetgen.vtu` | Internal fluid-domain volume mesh used for reconstruction and visualization of the experimental flow field |

| Condition | File | Description |
|---|---|---|
| **300 RPM** | `Predicted_coordinates_and_stds.txt` | **Reconstructed Lagrangian time series.** Time-resolved 3D trajectory of the radioactive tracer reconstructed from detector measurements at 300 RPM. Contains the reconstructed X, Y and Z coordinates together with their associated standard deviations, providing a point-by-point estimate of positional uncertainty. |
| | `20251011_094758_NN.vtu` | **Augmented Eulerian flow field.** Three-dimensional Eulerian velocity field reconstructed from the experimental Lagrangian time series at 300 RPM and mapped onto the internal tank mesh. Contains spatially resolved experimental flow quantities for visualization, quantitative analysis, CFD validation, and physics-based AI applications. |
| **400 RPM** | `Predicted_coordinates_and_stds.txt` | **Reconstructed Lagrangian time series.** Time-resolved 3D trajectory of the radioactive tracer reconstructed from detector measurements at 400 RPM. Contains the reconstructed X, Y and Z coordinates together with their associated standard deviations, providing a point-by-point estimate of positional uncertainty. |
| | `20251012_125920_NN.vtu` | **Augmented Eulerian flow field.** Three-dimensional Eulerian velocity field reconstructed from the experimental Lagrangian time series at 400 RPM and mapped onto the internal tank mesh. Contains spatially resolved experimental flow quantities for visualization, quantitative analysis, CFD validation, and physics-based AI applications. |
| **500 RPM** | `Predicted_coordinates_and_stds.txt` | **Reconstructed Lagrangian time series.** Time-resolved 3D trajectory of the radioactive tracer reconstructed from detector measurements at 500 RPM. Contains the reconstructed X, Y and Z coordinates together with their associated standard deviations, providing a point-by-point estimate of positional uncertainty. |
| | `20251013_144508_NN.vtu` | **Augmented Eulerian flow field.** Three-dimensional Eulerian velocity field reconstructed from the experimental Lagrangian time series at 500 RPM and mapped onto the internal tank mesh. Contains spatially resolved experimental flow quantities for visualization, quantitative analysis, CFD validation, and physics-based AI applications. |

| Result | Description |
|---|---|
| **Mixing index** | Quantitative characterization of mixing based on the spatial exploration of the tracer trajectory within the vessel. |
| **Velocity distributions** | Statistical distributions of the measured/reconstructed tracer velocities, providing information on the range and frequency of velocities encountered throughout the vessel. |
| **Position distributions** | Spatial distributions of tracer occurrence, showing how frequently different regions of the vessel are visited during the experiment. |
| **Pumping rates** | Flow-rate metrics calculated by integrating the reconstructed velocity field across selected surfaces, providing estimates of impeller pumping and circulation. |
| **Velocity profiles** | Extracted velocity components or velocity magnitude along selected spatial locations, enabling comparison of the flow structure across the vessel and between operating conditions. |
| **Wall velocity distributions** | Distribution of velocities in the near-wall region, providing a quantitative characterization of fluid motion adjacent to the vessel wall. |
