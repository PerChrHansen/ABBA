# ABBA
Pairs of unmatched projection matrices, in Matrix sparse matrix format.

This repository contains mat-files with test matrices in Matlab sparse matrix format. The matrices are generated
by means of the ASTRA Tomography software package. Each mat-file contains
the following variables:
   A - a sparse matrix that represents the forward projector in X-ray CT
   B - a sprase matrix that represents the corresponding back projector (B is not equal to transpose(A))
   GPU - a logical scalar that is true, indicating that A and B were generated on a GPU
   m - the number of rows in A, and the number of columns in B
   n = the number of columns in A, and the number of rows in B
   num_angles - the number of projection angles in the X-ray CT measurement setup
   num_detectors - the number of detectors in the X-ray CT measurement setup
   num_pixels - the square image to be reconstructed is num_pixels x num_pixels
