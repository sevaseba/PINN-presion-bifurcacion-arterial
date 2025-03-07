# Physics-Informed Neural Network Model for Predicting Pulmonary Arterial Pressure

Repository containing the code for the full paper presented at the _Medical Imaging with Deep Learning_ [MIDL](https://2025.midl.io/) conference, which will take place in 9—11 July 2025

## Abstract
Pulmonary arterial pressure is a key parameter for diagnosing cardiovascular and pulmonary diseases. Its measurement through right heart catheterization is considered the gold standard, and it is an invasive procedure that entails significant risks for patients. This has motivated the development of non-invasive techniques based on patient-specific imaging, such as Physics-Informed Neural Networks (PINNs), which integrate clinical measurements with physical models, such as the 1D reduced Navier-Stokes model, enabling biologically plausible predictions with limited data. This work implements a PINN model that uses velocity and area measurements in the main bifurcation of the pulmonary artery, comprising the main artery and its secondary branches, to predict pressure, velocity, and area variations throughout the bifurcation. The model training includes penalties to satisfy the laws of flow and momentum conservation. The results show that using 4D Flow MRI images from a healthy patient as clinical data, the pressure estimates provided by the model are consistent with the expected ranges reported in the literature, reaching a mean arterial pressure of 21.5 mmHg. This model presents an innovative approach that avoids invasive methods, being the first study to apply PINNs to estimate pulmonary arterial pressure in bifurcations. In future work, we aim to validate the model in larger populations and confirmed pulmonary hypertension cases diagnosed through catheterization.

## Main folders and files:
- La carpeta "Validación Kissas" contiene el código correspondiente a la validación propuesta en https://arxiv.org/abs/1905.04817. 
- La carpeta "exp. datos clínicos" contiene la simulación hecha para datos clínicos reales. 


## Dependencies:
The code was tested in Visual Studio Code on MacBook Pro (Sonoma 14.4.1) and Python 3.11. Main used libraries:

- [numpy](https://numpy.org/) (1.23): numerical and array operations
- [matplotlib](https://matplotlib.org/) (3.8): Figures and plots
- [tensorflow](https://www.tensorflow.org/?hl=es) (2.13): Machine learning framework
- [jupyterlab](https://jupyter.org/) (4.2): development using notebooks


This repository includes the file `PINN-blood-pressure.yml`, which is the updated conda enviroment used in this proyect.