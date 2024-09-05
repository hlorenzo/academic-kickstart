+++
title = "PLS and sparse PLS"

date = 2018-11-22T00:00:00

summary = "Introduction to PLS (Partial Least Square) and one of its sparse versions."

tags = ["French","R","PLS","Selection","Sparse","Single Cell"]

# Optional external URL for project (replaces project detail page).
# external_link = "static/html/lorenzo_double_cursus_SOURCE/main.html"

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Simulated datasets analysed with PLS under discriminant analysis"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Right"
+++

# Overview

The **PLS** tool is powerfull to tackle the curse of dimensionality, especially if the dataset suffers form high colinearities or if $n<p$. It even works when the response matrix is multivariate!

That course, given to **M2**-biostatistics students of **ISPED**, [website](http://www.isped.u-bordeaux.fr/Formation/MasterenSantePublique/M2BIOSTAT.aspx) introduces that tool and its sparse version thanks to which this is easily possible to select variables. 

# Magistral course

  - Recalls over linear regression and non-invertible cases,
  
  - **PLS1** and **PLS2** algorithms.
  
  - **sPLS** from the **Lasso** point of view.
  
  - A case study

[<i class="fa fa-file-pdf fa-2x"></i>](/pdf/CM_sPLS.pdf)

# Practical work on R

  - **sPLS-DA on simulated datasets**: A **4**-classes discrimination simulated problem to show the importance of the cross-validation process for supervized problems rather than explained variance [<i class="fab fa-r-project fab-2x"></i>](/html/TP_sPLS.html)

  - **sPLS-DA for single-cell 10X dataset**: The application of the **PLS** method to a Discriminant Analysis case for Single-cell *4* classes discrimination:
  
    - Statement [<i class="fab fa-r-project fab-2x"></i>](/html/spls_single_cell.html) [<i class="fab fa-r-project fab-2x"></i>](/R/crossValidate_splsDA.R) [<i class="fas fa-file-archive fas-2x"></i>](/csv/cellTypes_genes.zip)
    - Correction [<i class="fab fa-r-project fab-2x"></i>](/html/spls_single_cell_CORRECTION.html)
  
  - **sPLS regression**: The classical application to the sPLS regression model to the `liver.toxicity` dataset:
  
    - Statement [<i class="fab fa-r-project fab-2x"></i>](/html/sPLS_regression.html)
    - Correction [<i class="fab fa-r-project fab-2x"></i>](/html/sPLS_regression_correction.html)
  