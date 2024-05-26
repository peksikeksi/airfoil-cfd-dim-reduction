# Airfoil CFD Data Dimensionality Reduction
## Description
This project focuses on performing Singular Value Decomposition (SVD) and Proper Orthogonal Decomposition (POD) on computational fluid dynamics (CFD) data of steady airfoil flow fields. The goal is to achieve dimensionality reduction to simplify the analysis and visualization of complex flow patterns around airfoils.

## Introduction
Dimensionality reduction techniques like SVD and POD are powerful tools used to simplify complex datasets. In this project, we apply these techniques to CFD data of airfoil flow fields to reduce the complexity and enhance the understanding of flow characteristics.

## Singular Value Decomposition (SVD)
What is SVD?
Singular Value Decomposition (SVD) is a mathematical technique used in linear algebra to decompose a matrix into three simpler matrices. It expresses the original matrix as the product of an orthogonal matrix, a diagonal matrix, and the transpose of another orthogonal matrix.

![image](https://github.com/peksikeksi/airfoil-cfd-dim-reduction/assets/81853083/4f21e79a-bdf7-42e6-9feb-41a14b1fd0ed)

Visualization of the matrix multiplications in singular value decomposition [1]

SVD is widely used for reducing the dimensionality of data, extracting significant features, enhancing computational efficiency, noise reduction and data compression.

## Proper Orthogonal Decomposition (POD)

Proper Orthogonal Decomposition (POD) is a technique used to identify patterns in data by finding orthogonal modes that capture the most energy or variance in the system. It is similar to Principal Component Analysis (PCA) but specifically applied to fluid dynamics and other physical systems. [6]

![image](https://github.com/peksikeksi/airfoil-cfd-dim-reduction/assets/81853083/f9ed3b92-1521-4082-8029-8bb8f339223d)

POD snapshots [7]

POD is used for extracting dominant features from complex flow fields, reducing the number of variables needed to describe the system, enhancing the understanding of underlying physical phenomena and developing reduced-order models for simulations.


## Airfoil Types
Dataset was taken from kaggle [9]. It represents Computational Fulid Dynamics (CFD) simulation results for six different airfoil shapes. Three of which are cambered (NACA 2412, NACA 2415, and NACA 4412) and three symmetric (NACA 0012, NACA 0015 and NACA 0021). The dataset organized into columns for velocity components (U:0, U:1, U:2), pressure coefficient values and coordinates of points on the airfoil.

### Cambered Airfoils
A cambered airfoil is designed with a curved shape where the upper and lower surfaces are not symmetrical. The curvature allows for more lift at lower angles of attack compared to symmetric airfoils. Cambered airfoils are commonly used in aircraft wings to improve aerodynamic efficiency.

### Symmetric Airfoils
A symmetric airfoil has identical upper and lower surfaces, resulting in no camber. These airfoils do not generate lift at zero angle of attack but can be effective for applications where lift is not required at all times, such as in certain control surfaces or rotor blades.

### Differences Between Cambered and Symmetric Airfoils:

**Lift Characteristics:** Cambered airfoils generate lift at zero angle of attack, while symmetric airfoils do not.

**Stability:** Symmetric airfoils are typically more stable in inverted flight and are often used in aerobatic aircraft.

**Application:** Cambered airfoils are used in fixed-wing aircraft wings for efficient lift, whereas symmetric airfoils are used in applications requiring equal performance in both directions.

## Usage
To use this project, clone the repository and follow the instructions in the provided Jupyter notebooks for performing SVD and POD on the given CFD airfoil data.

## Acknowledgments
__FlowFieldVisualizer Class__ was based on __FieldVisualizer__ and __FlowFieldStreamlines__ classes created by original authors [10]. The original code is licensed under the Apache 2.0 license.

## License
This project is licensed under the MIT License.

## References and Cool Links

[1] [Image Link](https://en.wikipedia.org/wiki/File:Singular_value_decomposition_visualisation.svg)

[2] [Singular Value Decomposition (SVD) - GeeksforGeeks](https://www.geeksforgeeks.org/singular-value-decomposition-svd/)

[3] [Singular value decomposition - Wikipedia](https://en.wikipedia.org/wiki/Singular_value_decomposition)

[4] [Singular Value Decomposition (SVD): Mathematical Overview](https://www.youtube.com/watch?v=nbBvuuNVfco)

[5] [Singular Value Decomposition (the SVD)](https://www.youtube.com/watch?v=mBcLRGuAFUk)

[6] [Proper Orthogonal Decomposition - Wikipedia](https://en.wikipedia.org/wiki/Proper_orthogonal_decomposition)

[7] [Image Link](https://en.wikipedia.org/wiki/File:POD_snapshots.png)

[8] [Principal Component Analysis (PCA)](https://www.youtube.com/watch?v=fkf4IBRSeEc)

[9] [Airfoil CFD Data for 6 airfoils](https://www.kaggle.com/datasets/udvasbasak/ae646-gp1-data/data)

[10] [Grp-Pr-1_Arka,Lavanya,Udvas](https://www.kaggle.com/code/udvasbasak/grp-pr-1-arka-lavanya-udvas)


