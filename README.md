# approx_Graph_Frechet_Mean

The code provided approximates the Frechet mean of a set of graphs when considering the euclidean distance between the spectra of two graphs. The theory is outlined in **Approximate Empirical Frechet mean of graphs with applications to linear regression** with an arxiv link to come.  <br />

Here we provide both the raw data and the results for the Frechet mean as two separate files. One may write their own implementation of the algorithms presented in **Approximate Empirical Frechet mean of graphs with applications to linear regression** and compare to our results. Our implementation of the algorithms are also provided.

**Raw Data** <br />
The raw data files are titled "BLANK_BLANK_Data.mat". Each of these .mat files contains the parameters used to generate the data and the sample set of adjcency matrices.

**Converged Data** <br />
The converged data serves as a way to compare and reproduce results of the paper. The files "BLANK_BLANK_Data_converged.mat" are the result of running approxEmpiricalFrechetMean.m given the raw data.

The data provided is associated with the above paper and the code can be used to generate the figures in the following way.

**Tutorial: Frechet Mean** <br />
**Step 1:** Download the matlab file titled approxEmpiricalFrechetMean.m <br />
**Step 2:** Download the data file(s) <br />
**Step 3:** Load Small_World_Data.mat into matlab (or any other raw data file) <br />
Contents - sampleAdjSet: the sample adjacency set of graphs <br />
              K, beta: parameters used to generate the set from the Small World ensemble <br />
              n: the number of nodes <br />
              N: the number of graphs in the set <br />
**Step 4:** Run approxEmpiricalFrechetMean.m  <br />
        -We suggest saving the data after this step. <br />
**Step 5:** Run displayMean.m <br />
        -This file will display the approximate Frechet mean of the set of graphs and the first graph in the observed sample set <br />
**Step 6:** Run plottingHistogram.m <br />
        -This file will display the average eigenvalues from the dataset and the eigenvalues of the approximate Empirical Frechet Mean graph. Along with the theoretical eigenvalues of the approximate Empirical Frechet mean graph. <br />

**Tutorial: Regression** <br />
**Step 1:** Download the matlab file titled approxEmpiricalFrechetRegression.m <br />
**Step 2:** Download the data file regression_data.m <br />
**Step 3:** Load the data into matlab <br />
**Step 4:** Run approxEmpiricalFrechetRegression.m <br />
-We suggest saving the data at this step <br />
**Step 5:** Run plottingRegression.m <br />
