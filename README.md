![image](https://user-images.githubusercontent.com/40338105/159864615-d5fe6877-e630-4d55-8a03-1325ec925642.png)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e-j7Yw3rTu8PTON-XK4d7FBYb8Z-0Yyd?usp=sharing)

The objective of this project is to provide seamless online access to all PHREEQC features through an instantly operational interface. No downloads or installations are necessary.

Phreeqc Web is comprised of a Python script that leverages IPhreeqc, specifically designed for effortless execution within a Jupiter notebook hosted on Google Colab. This setup ensures that users can harness the full spectrum of capabilities offered by the desktop graphical user interface without any additional setup requirements.

The implementation has been possibile through the Python package "phreeqpy" (https://www.phreeqpy.com/).

# Getting started 

Phreeqc Web is run in a Jupiter notebook which can be accessed in Google Colab and run here &#8594; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e-j7Yw3rTu8PTON-XK4d7FBYb8Z-0Yyd?usp=sharing)

The notebook contains 5 examples:

1) Visualization of the outputs of a simple reaction
2) Automatic replacement of inputs 
3) Breakthrough plots (example 11 of Phreeqc's manual)
4) Spatial profile plots (uphill diffusion example)
5) Electrokinetic transport 

Each example is independent and provides a starting point to develop more complex applications. 

# Do I need to compile IPhreeqc to make it work? 

No, Phreeqc Web is ready to run. Actually, the source code of Iphreeqc is taken from the USGS website (https://www.usgs.gov/software/phreeqc-version-3) and it is automatically compiled using GitHub actions (available for this repo here: https://github.com/rispr/phreeqc_web/blob/main/.github/workflows/compile_on_upload.yml). Every time a new source code is uploaded in this repository it is automatically compiled and a Linux library is generated (https://github.com/rispr/phreeqc_web/tree/main/Iphreeqc_compiled) which is ready to be used by IPhreeqc, just by changing a link in Google Colab. 

# References

* Parkhurst, D. L., & Appelo, C. A. J. (2013). Description of input and examples for PHREEQC version 3-a computer program for speciation, batch-reaction, one-dimensional transport, and inverse geochemical calculations. US geological survey techniques and methods, 6(A43), 497.
* Charlton, S. R., & Parkhurst, D. L. (2011). Modules based on the geochemical model PHREEQC for use in scripting and programming languages. Computers & Geosciences, 37(10), 1653-1663.
* Müller, M., Parkhurst, D. L., & Charlton, S. R. (2011). Programming PHREEQC calculations with C++ and Python a comparative study. EXCHANGE, 1(40), 632-636.
