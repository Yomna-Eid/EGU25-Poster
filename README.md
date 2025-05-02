# When is a finer spatial resolution justified in remote sensing analysis?
### [EGU25 Poster](https://meetingorganizer.copernicus.org/EGU25/EGU25-19140.html)

**Abstract**:

Remote sensing analysis is often used to provide supporting information for evidence-informed policy-making. Typically, such analysis presents results as classification maps, such as a land cover classification used to estimate deforestation areas in a region. For such analyses, where aggregated areal values of specific classes are the primary targets, a critical question arises: do the results significantly degrade when lower spatial resolution Earth Observation (EO) products are used instead of higher-resolution ones?

EO products like Dynamic World land use and land cover maps, produced at a high temporal and spatial resolution (5 days and 10m, respectively), are built on the widely held belief that higher resolutions inherently yield better results. However, with the exponential growth in data volumes and the computational demands of high-resolution workflows, it becomes increasingly important to determine where these resource-intensive approaches provide meaningful advantages — and where they do not — to balance computational efficiency with the need for accuracy in remote sensing workflows.

To address this question, we examine two case studies: deforestation in the Cerrado Biome of Brazil, and the imperviousness of sealed surfaces in Germany. Classification maps from each study are systematically downsampled from their native resolutions in steps up to 10 km spatial resolution. Using Ripley’s Equation1, numerically approximated with a Gaussian-Quadrature approach, we compute standard errors to assess the impact of spatial resolution on classification accuracy.

We report our findings on how the aggregated target values derived from lower-resolution data compare to those from higher-resolution inputs. We also try to identify the resolution thresholds beyond which the quality of the final product loses acceptable representation of the phenomena in the selected use cases.

_1 See Eq. 3.4, page 23 in Ripley, B.D. (1981), “Spatial Sampling” in Spatial Statistics._

**How to cite:** Eid, Y. and Pebesma, E.: When is a finer spatial resolution justified in remote sensing analysis?, EGU General Assembly 2025, Vienna, Austria, 27 Apr–2 May 2025, EGU25-19140, https://doi.org/10.5194/egusphere-egu25-19140, 2025.
