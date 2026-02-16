
<p align="left">
  <img src="icon.png" width="180">
</p>

A Mass Spectrometry-Based Single-Cell Metabolomics Data Processing Platform.
Welcome to the development folder for the CellMate application and source code. Here you will find source code, a precompiled version of the app, and documentation.

## License
CellMate
Copyright (C) 2026 Felix Friedrich

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.

## What is CellMate
CellMate is an application written in MATLAB for processing mass spectrometry-based direct infusion data, adapted for singe-cell metabolomics. The application can be run for targeted or untargeted data analysis. It currently supports both Thermo Fisher's .raw file format and the universal .mzML file format.

CellMate was made to handle complex direct-infusion data with repetitive events/injections, with key features of:

Semi-automated detection single-cell event window
Fast data processing in both targeted and untargeted modes
Statistical background filter options
Quantitative capabilities when using IS 
Novel deep-learning-based identification of endogenous species - an effective background removal tool
Interactive and dynamic graphical user interface

## Requirements
### Standalone Version 
The compiled version of CellMate does not require a MATLAB license. The compiled version (`CellMate.exe`) requires the MATLAB Runtime (R2023b), as this version is where the app source code was compiled. The CellMate.exe file needs to be installed and can be used directly. Upon starting the app, two .DLL files are required for Thermofishers .RAW import function. These .DLL files are in the same folder as the compiled version. For using the pre-trained deep-learning model for species classification, a .mat file needs to be loaded in the DL tab (tab 4). A potential future feature is the ability to transfer-learn a model ad hoc (on new data) to adjust to different experimental settings.

Download the MATLAB Runtime here:
https://www.mathworks.com/products/compiler/matlab-runtime.html

### Running from the App Designer application in MATLAB 2023b
The application is developed with MATLAB 2023b, including the Deep Learning Toolbox. Please install this version and the add-on before running the source code in the licensed MATLAB environment. There may be conflicts when running the code with other versions of MATLAB. After downloading the source code of the application, you can run and modify the code in the MATLAB App Designer application.

## Cite
Please cite any use of this software as: Friedrich, F.; Marques, C.; Lanekoff, I. CellMate─A Deep Learning-Assisted Single-Cell Data Processing Platform. Anal. Chem. 2026. https://doi.org/10.1021/acs.analchem.5c07205.

## Reporting problems
Although we are not supporting the software, please file any eventual issues under the issues tab on this GitHub. While the layout of the source code and implementation of the App designer app may appear unfamiliar, an LLM of your choice can easily help to modify and implement features.

Please provide a short description of the problem and try to replicate it yourself before you report it: 
In the report, provide the version of MATLAB and a copy of the error message
