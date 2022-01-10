# 2022_PT_Election

This project is to do text analytics on the political programs/manifests of the main Portuguese parties in the 2022 general election.

Project has 4 main parts:
 - Clean-up
    - take out pontuation and general clean-up of the PDF/HTML with the programs/manifests
    - done through a Macro in Word (a file at a time)
    - than to be saved as individual TXT
 - pre-processing 
    - Run through the Cleaned-up TXT and count words (and also groups of 2 and 3 words)
      - take out generic words 
      - apply synonym substituition
    - Sub-select only most used words (to feed to next step)
    - Run can start mid this file reusing the "Processed CH+BE+PCP+Livre+PSD+PS+IL" file (unless you want to wait hours on the initial processing)
 - Clustering and MDS
      - Check proximity between Parties
      - MDS done from 1 to 4 dimensions
 - Multilinear Regression
      - Check which words drive the dimensions from MDS
