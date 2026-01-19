# MATLAB Graph Digitizer – Picture to Excel

This repository provides a MATLAB-based interactive tool to extract numerical data from published graph images and export them to Excel format. The program is designed for engineering applications such as force–deflection, moment–curvature, or load–displacement curves when raw experimental data are not available. The software does not reproduce, redistribute, or modify copyrighted figures; it only assists in extracting approximate numerical values visible in the original image. Users are responsible for properly citing the original source of any digitized figure.

# Features

The script loads a graph image, allows interactive calibration of the x- and y-axes using known reference values, automatically detects one or multiple curves based on color and intensity, distinguishes curves without relying on axis titles, resamples each curve into a user-defined number of equally spaced points (default 100), overlays the detected curves on the original image for visual verification, and exports the digitized data to an Excel file with one sheet per curve.

# Requirements

MATLAB with the Image Processing Toolbox is required. The code has been tested with standard RGB images such as PNG and JPG files commonly used in journal papers.

# Usage

Run the MATLAB script and select the image file of the graph when prompted. Click two known points on the x-axis and enter their corresponding numerical values, then repeat the process for the y-axis. The program will automatically identify the curves, display them over the original image for checking, and generate an Excel file containing the x–y data for each curve.

# Output

The output is an Excel file where each curve is stored in a separate sheet named Curve_1, Curve_2, etc. Each sheet contains two columns corresponding to the x and y coordinates of the digitized curve.

# Limitations

Curve separation relies primarily on color and contrast; figures with very similar curve colors or heavy overlap may require minor preprocessing or manual refinement. The accuracy of the extracted data depends on the resolution of the input image and the precision of the axis calibration points selected by the user.

# License

This project is released under the MIT License to encourage reuse and modification for academic and research purposes.

# Citation

If this tool is used in academic work, please cite the repository and clearly acknowledge the original source of the digitized figure, in accordance with the journal’s ethical guidelines.
