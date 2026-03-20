# gripper-hub-fea-ml-optimization
AI-assisted optimization of a soft robotic gripper hub using Fusion 360, FEA, Python, and machine learning to improve structural performance and reduce mass.

## Overview
This project focuses on optimizing a soft robotic gripper hub using CAD, finite element analysis, and machine learning.

I created 11 design iterations in Fusion 360 and evaluated each version using structural simulation. The design dataset was then analyzed in Python, and machine learning models were used to explore design-performance relationships and guide further optimization.

## Objective
To reduce hub mass while maintaining low stress, low displacement, and a high safety factor.

## Tools Used
- Fusion 360
- Python
- Pandas
- Matplotlib
- Scikit-learn

## Design Variables
- Pocket depth
- Through cut
- Rib thickness
- Cutout length
- Cutout angle

## Performance Metrics
- Mass
- Volume
- Maximum stress
- Maximum displacement
- Minimum safety factor

## Workflow
1. Created multiple CAD design iterations
2. Ran FEA simulations in Fusion 360
3. Built a dataset from simulation outputs
4. Visualized design trade-offs using Python
5. Ranked versions using a weighted engineering score
6. Trained ML models to predict structural performance
7. Used ML-guided exploration to improve the design

## Key Findings
- Through cuts weakened the structure significantly
- Moderate material removal gave the best trade-off
- V6 emerged as the best design from the initial set
- Further guided exploration led to V11, which improved on V6

## Final Best Design: V11
- Mass: 19.988 g
- Volume: 18856.361 mm^3
- Pocket depth: 6 mm
- Through cut: 0
- Rib thickness: 4.5 mm
- Cutout length: 15.5 mm
- Cutout angle: 12°
- Max stress: 1.09 MPa
- Max displacement: 0.013 mm
- Minimum safety factor: 18.342

## Engineering Conclusion
The project showed that moderate cutout extension without through cuts produced the best balance between light weight and structural integrity.

## Files
- `gripper_dataset_final.csv` : simulation dataset
- `gripper_analysis_complete.ipynb` : Python analysis and ML workflow
- `images/` : CAD views, simulation screenshots, and graphs

## Skills Demonstrated
CAD design, FEA, design optimization, Python data analysis, machine learning, engineering decision-making
