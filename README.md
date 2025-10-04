#Sample codes for using 'MeTMEC' tool to estimate the cell composition by using the methylation array profile. #install the 'MeTMEC' package from the GitHub

library(devtools)

devtools::install_github("hyu020/MeTMEC")

#Calculate the cell composition 

library(MeTMEC) #loading the package

mycells <- calMeTIL(data.array) #data.array is the beta value matrix of your bulk sample methylation array profiles; calculating the proportions of your cells of interest

mycells #output of the proportions of your cells of interest
