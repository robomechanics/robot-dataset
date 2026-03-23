# robot-dataset
Robot Scaling Literature Review Dataset Data and figures accompanying the paper: Allometric Scaling Laws for Bipedal Robots. This repository contains morphological data (body length, leg length, mass) for different robot systems spanning locomotion types, used to derive empirical scaling laws via power-law regression.

---

## Repository Contents

| File | Description |
|------|-------------|
| `robot_scaling_dataset.csv` | Robot dataset with morphological measurements and reference URLs |
| `fit_summary_powerlaw.txt` | Power-law fit results (coefficient A, exponent b, R², n) for all relationships |
| `litrev_mass_length.png` | Figure: Mass and leg scaling plots (static image) |
| `litrev_mass_length.svg` | Figure: Mass and leg scaling plots (vector, editable) |
| `litrev_mass_length.html` | Figure: Mass and leg scaling plots (interactive) |

---

## Dataset (`robot_litrev.csv`)
<!--
### Columns

| Column | Units | Description |
|--------|-------|-------------|
| `robot_name` | — | Robot name |
| `reference` | — | Primary reference/source URL |
| `type` | — | Locomotion type: `biped`, `quadruped`, `hexapod` |
| `year` | year | Year of publication or commercial release |
| `cost_dollars` | USD | Approximate retail/reported cost |
| `total_length_inm` | m | Total body length |
| `leg_length_inm` | m | Leg length |
| `min_mass_inkg` | kg | Minimum reported mass |
| `max_mass_inkg` | kg | Maximum reported mass |
| `average_mass_inkg` | kg | Average or reported mass used in analysis |
| `normal_speed_inmps` | m/s | Normal operational speed |
| `walking_speed_inmps` | m/s | Walking speed |
| `running_speed_inmps` | m/s | Running/maximum speed |
| `DOF` | — | Degrees of freedom |
| `payload_inkg` | kg | Rated payload capacity |
| `actuator_mass_inkg` | kg | Total actuator mass |
| `accuator_count` | — | Number of actuators |
| `highest_stall_torqueorforce_on_actuators_inNm` | Nm | Maximum stall torque of primary actuator |
| `actuator_name` | — | Actuator model/name |
| `acutation_type` | — | Actuation technology (e.g., motors, hydraulics) |
| `reported_COT` | — | Cost of Transport |
| `battery_life_hours` | hours | Rated battery life |
| `battery_wt_inkg` | kg | Battery mass |

### Robot Types

- **Full Biped**: humanoid robots with full upper body (n = 17)
- **Lower Biped**: bipedal locomotion-only platforms (n = 10)
- **Quadruped**: four-legged robots (n = 14)
- **Hexapod**: six-legged and insect-scale robots (n = 6)



---

## Scaling Laws (`fit_summary_powerlaw.txt`)

All relationships follow the form **y = A · x^b**, fit by ordinary least squares in log–log space.

Key results (global fits across all 47 legged robots):

| Relationship | A | b | R² |
|---|---|---|---|
| Mass vs Body Length | 23.76 | 2.34 | 0.90 |
| Mass vs Leg Length | 68.20 | 2.12 | 0.87 |
| Leg vs Body Length | 1.48 | 0.86 | 0.87 |

Per-type fits are also provided for Full Biped, Lower Biped, Hexapod, and Quadruped categories.

---

## Notes

- Data were collected and verified from manufacturer specifications, datasheets, and peer-reviewed publications.
- Some robots were included in the CSV file, but excluded from powerfitting due to missing data
