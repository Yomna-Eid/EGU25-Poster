EGU25 Poster titled “When is a finer spatial resolution justified in remote sensing analysis?”

1.	Content

1.1.	Sections\
  1.1.1.	 Introduction\
    1.1.1.1.	
    
  1.1.2.	Research Objectives\
    1.1.2.1.	How do estimates of Forest fraction change when the classified image is gradually down-sampled from a 10-m resolution to 10-km resolution? \
    1.1.2.2.	How does the standard error of this fraction vary with down-sampling when using systematic non-random sampling? [1] \
    1.1.2.3.	When does lowering the resolution stop being acceptable? \
  
  1.1.3.	Datasets\
    1.1.3.1.	
  
  1.1.4.	Methodology\
    1.1.4.1.	
  
  1.1.5.	Results
  
  1.1.6.	Discussion and Conclusion\

  1.1.7.	References (if necessary) \

1.2.	Open Source Code \
  1.2.1.	Preparation of the datasets\
    1.2.1.1.	Imperviousness maps\
      1.2.1.1.1.	Subset to North-Rhine Westphalia, Germany\
      1.2.1.1.2.	Binary classification based on literature threshold of 30%\
      1.2.1.1.3.	Change 2018 map to start from 20m resolution, like other maps from 2006, 2009, 2012, 2015\
      1.2.1.1.4.	Downsample from 20m resolution to 10km in steps\
      1.2.1.1.5.	Save maps and their downsampled by-products\
    1.2.1.2.	PRODES Deforestation maps\
      1.2.1.2.1.	Dataset availability from 2002-2024 uneven, so skip a year to maintain temporal frequency of even years (2002, 2004, 2006, 2008, 2010, 2012, 2014, 2016, 2018, 2020, 2022, 2024)\
      1.2.1.2.2.	Clean dataset from unnecessary variables\
      1.2.1.2.3.	Subset the study area\
      1.2.1.2.4.	Select polygons in the required study area\
      1.2.1.2.5.	Rasterize the vector dataset to produce the binary map (necessary for pixel-wise operation of down-sampling)\
      1.2.1.2.6.	Downsample from 30m resolution to 10km (same schema as Dataset 1)\
      1.2.1.2.7.	Save maps and their downsampled by-products\
  
  1.2.2.	Statistical Part using Ripley’s equation\
    1.2.2.1.	Stochastic: Monte-Carlo integration of equation of standard error variances\
    1.2.2.2.	Deterministic: Gauss-Quadrature integration of standard error variances\

1.3.	Figures\
  1.3.1.	Plots of the statistical error bars to present the deterioration\
    1.3.1.1.	Once using the Monte Carlo method\
    1.3.1.2.	Then using the Guass-Quadrature method\
  1.3.2.	Flowchart of methodology\
  1.3.3.	 Maps of the datasets 1&2 over the study area\
  1.3.4.	Logos of the project, ifgi, uni, egu, QR-Code of Github repo, QR-Code of voting for student competition\

2.	Template\
  2.1.	Posterdown package (Betterland) in R\
