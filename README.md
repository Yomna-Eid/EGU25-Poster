EGU25 Poster titled “When is a finer spatial resolution justified in remote sensing analysis?” {https://meetingorganizer.copernicus.org/EGU25/EGU25-19140.html}

**I.	Content**

**A.	Sections\**

  1. Introduction

  2. Research Questions\
     RQ1.   How do estimates of Impervious fraction change when the classified image is gradually down-sampled from a 20-m resolution to 10-km resolution? \
     RQ2.  How do estimates of Forest fraction change when the classified image is gradually down-sampled from a 30-m resolution to 12-km resolution? \
     RQ3.	How does the standard error of this fraction vary with down-sampling when using systematic non-random sampling (using Ripley's 1981)?\
     RQ4.	When does lowering the resolution stop being acceptable?\
     RQ5.   How does the Monte Carlo Integration (random stochastic) method compare to Gauss-Quadrature (systematic deterministic) method when computing complex covariance functions for evaluating the standard error using Ripley's 1981?
       
  3. Datasets\
     a.	High Resolution Layer Maps of Imperviousness for Germany (North-Rhine Westphalia)\
     b. PRODES Deforestation Maps for Cerrado Biome of Brazil
  
  4. Methodology
  
  5. Results
  
  6. Discussion and Conclusion

  7. References (if necessary) 

**B.	Open Source Code\**

  1.	Preparation of the datasets
  
    a.	Imperviousness maps
    
      i.	Subset to North-Rhine Westphalia, Germany\
      ii.	Binary classification based on literature threshold of 30%\
      iii.	Change 2018 map to start from 20m resolution, like other maps from 2006, 2009, 2012, 2015\
      iv.	Downsample from 20m resolution to 10km in steps\
      v.	Save maps and their downsampled by-products
    
    b.	PRODES Deforestation maps
    
      i.	Dataset availability from 2002-2024 uneven, so skip a year to maintain temporal frequency of even years (2002, 2004, 2006, 2008, 2010, 2012, 2014, 2016, 2018, 2020, 2022, 2024)\
      ii.	Clean dataset from unnecessary variables\
      iii.	Subset the study area\
      iv.	Select polygons in the required study area\
      **1.2.1.2.5.	Rasterize the vector dataset to produce the binary map (necessary for pixel-wise operation of down-sampling)**
      v.	Downsample from 30m resolution to 10km (same schema as Dataset 1)\
      vi.	Save maps and their downsampled by-products
      
    c.	Statistical Part using Ripley’s equation
    
    i.	Stochastic: Monte-Carlo integration of equation of standard error variances\
    ii.	Deterministic: Gauss-Quadrature integration of standard error variances


**C.	Figures\**

  1.	Plots of the statistical error bars to present the deterioration\
    a.	Once using the Monte Carlo method\
    b.	Then using the Guass-Quadrature method
  
  2.	Flowchart of methodology
  
  3.	 Maps of the datasets 1&2 over the study area
  
  4.	Logos of the project, ifgi, uni, egu, QR-Code of Github repo, QR-Code of voting for student competition

**B.	Template**\

  1.	Posterdown package (Betterland) in R {https://github.com/brentthorne/posterdown/wiki/posterdown_betterland}
