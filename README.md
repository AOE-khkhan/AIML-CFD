# AIML-CFD
CMU 24-787 Artificial Intelligence and Machine Learning Project: A Machine Learning Framework for Predicting Errors in the Numerical Solutions of Navier-Stokes Equations
### Turbulence modeling is widely used for solving real world problems with Computational Fluid Dynamics (CFD). In addition to the accuracy of the results, it is also important to consider the computational expense. Large Eddy Simulation (LES) has gain a lot of popularity due to its high accuracy, but still it takes too many computational resources for a simple engineering problem, such as flow around cylinder. Reynolds-averaged Navier–Stokes Equations (RANS) is widely used for turbulence modeling in the industry. Inviscid flow is the easiest and fastest to implement, but the results may not be as reliable due to the lack of viscosity in the assumption. In this project, multiple machine learning models were implemented, which would act as surrogate to the inexpensive numerical schemes, to correct the CFD results and achieve the same accuracy as provided by more expensive CFD methods such as LES. In the first part of this work, the flow around airfoil is simulated with inviscid and RANS models for multiple airfoils, angle of attacks and velocities. The errors between inviscid and RANS simulations are trained using neural network techniques like MLP and CDNN. For the second part, the flow around a cylinder is modeled with RANS and LES models. The errors between LES and RANS are trained with MLP and Random forest regressor coupled with k-fold cross-validation considering LES as ground truth. The highest accuracy from different machine learning methods is 98%.
