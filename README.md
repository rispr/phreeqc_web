# Phreeqc Web

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e-j7Yw3rTu8PTON-XK4d7FBYb8Z-0Yyd?usp=sharing)

The purpose of this project is to make all the features of PHREEQC available online. 

Phreeqc Web consists in a Python script which executes IPhreeqc and it is designed to run out-of-the-box in the cloud, with all the capabilities of the desktop graphical user interface.

The implementation has been possibile through the Python package "phreeqpy" (https://www.phreeqpy.com/).

# Getting started 

Phreeqc Web is run in a Jupiter notebook which can be accessed in Google Colab and run here &#8594; [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e-j7Yw3rTu8PTON-XK4d7FBYb8Z-0Yyd?usp=sharing)

The notebook contains 5 examples:

1) Visualize the outputs of a simple reaction
2) Automatic replace inputs 
3) Make a breakthrough plot (example 11 of Phreeqc's manual)
4) Plot spatial profiles (uphill diffusion example)
5) Simulate electrokinetic transport 

Each example is independent and should provide a starting point to develop more complex applications. 

# Do I need to compile IPhreeqc to make it work? 

No, Phreeqc Web is ready to run. Actually, the source code of Iphreeqc is taken from the USGS website (https://www.usgs.gov/software/phreeqc-version-3) and it is automatically compiled using GitHub actions (available for this repo here: https://github.com/rispr/phreeqc_web/blob/main/.github/workflows/compile_on_upload.yml). Every time a new source code is uploaded in this repo it is automatically compiled and a Linux library is generated (https://github.com/rispr/phreeqc_web/tree/main/Iphreeqc_compiled) which is ready to be used by IPhreeqc, just by changing a link in Google Colab. 

# Feedbacks? Suggestions? Requests of new features? 
Then get in touch with Riccardo Sprocati (ricspr@protonmail.com).
