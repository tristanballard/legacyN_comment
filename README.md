# legacyN_comment
R code and files necessary to recreate the figures from our Technical Comment (Science 2018). Contact Tristan Ballard (tballard@stanford.edu) with any questions.

File descriptions:

comment_code.Rmd contains the code to recreate the figures from our Technical Comment using the free R computing language. Code and figures can also be viewed without installing R in the files ‘comment_code.pdf’ and ‘comment_code.html’.

VM_predicted.csv (not included) contains 1800-2015 predicted loading fluxes [kilotons] from Van Meter et al. (2018). Data is available from those authors upon request.

n_surplus.csv (not included) contains 1866-2014 cropland N surplus values [kg/ha of cropland] as estimated by Van Meter et al. (2017), corresponding to the values in Figure 4A of the 2017 paper, as well as the fraction of the Mississippi River Basin covered in cropland, corresponding to Figure 3A of the same paper. Data is available from those authors upon request.

pigment_60_95.csv contains 1960-1995 chloropigment measurements [ug/g]. These were estimated from Figure 1B of Van Meter et al (2018) using a free plot analysis/extraction tool (https://automeris.io/WebPlotDigitizer/). 

precipitation.df.RDS contains annual 1900-2015 basin-wide precipitation [mm] data in R preferred format estimated from the freely available PRISM dataset. Code for extracting this from the raw PRISM data is a bit tedious, extracting precipitation data for each HUC8 watershed within the US and then summing over HUC8 watersheds within the Mississippi River Basin, accounting for differences in sizes of HUC8s. This takes ~15min to run on a standard laptop; contact tballard@stanford.edu if you would like this code as well.

References:
K. J. Van Meter, P. Van Cappellen, N. B. Basu, Legacy nitrogen may prevent achievement of water quality goals in the Gulf of Mexico. Science (80). 360, 427–430 (2018).
K. J. Van Meter, N. B. Basu, P. Van Cappellen, Two centuries of nitrogen dynamics: Legacy sources and sinks in the Mississippi and Susquehanna River Basins. Global Biogeochem. Cycles. 31, 2–23 (2017).
