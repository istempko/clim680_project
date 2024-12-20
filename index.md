# **Examining the Link between the Western Hemisphere Warm Pool Index and Extreme Heat in the Great Plains Region of the US through the Great Plains Low Level Jet**
By Ivy Stempkovski

## **Introduction**
The Western Hemisphere Warm Pool (WHWP), defined by sea surface temperatures (SST) greater than or equal to 28.5°C, is made up of the Atlantic Warm Pool (AWP) and the eastern North Pacific Warm Pool. The AWP is a large body of water in the North Atlantic spanning the Gulf of Mexico, Caribbean Sea, and western tropical North Atlantic [Povea Perez, Y., 2020]. The WHWP index, and thus the modulation of the AWP, can be linked to regional weather variation through the air-sea interface. In fact, the relationship between the WHWP and regional weather variation could introduce a potential predictor for extreme heat by elucidating the catalyst processes for atmospheric blocking events. 

Studies have shown that AWP variability influences atmospheric circulation patterns that promote heat wave occurrence over the Great Plains region of the US [Lopez, H., et al, 2022]. Notably during a positive WHWP index year, the anomalously warm AWP shifts the Intertropical Convergence Zone (ITCZ) northward, as the ITCZ follows the location of greatest insolation and surface warming [Green, B., et al, 2017]. Warm rising air over the ITCZ lowers ocean surface air pressure and creates a pressure gradient. The resulting pressure gradient force generates anomalous surface winds flowing southeasterly, in the direction of decreasing pressure. The anomalous southeasterlies strengthen the southeasterly Trade Winds while weakening the northeasterly Trade Winds. Additionally, an anomalously warm AWP reduces the magnitude of sea breezes since the differential land-ocean temperature has been reduced. Both of the described ocean-atmosphere interactions contribute to changes in the Great Plains Low Level Jet (GPLLJ). 

Heat waves in the Great Plains can be traced back to the AWP by means of the GPLLJ. The GPLLJ carries warm, moist air from the Gulf of Mexico to the Great Plains and is responsible for about one-third of the total moisture transport to that region [Lopez, H., et al, 2022]. An anomalously warm AWP enhances atmospheric convection over the Caribbean and reduces moisture transport to the Great Plains. Such warm advection can result in a pair of Gill-type upper-level anticyclones that may produce anticyclonic blocking, or a blocking high [Lopez, H., et al, 2022]. A blocking high is a large, stationary high pressure system that prevents other systems from moving into the region. As the high pressure system persists, surface temperatures increase. Reduced moisture transport to the Great Plains exacerbates the “heat dome” effect of the blocking high.The following analysis will examine the influence of AWP interannual variability on heat waves over the US Great Planes.

## **Data**
For the WHWP Index, I sourced my data from the National Oceanic and Atmospheric Administration (NOAA) Physical Sciences Laboratory. The index was created using HadISST and NOAA OI SST datasets and describes the monthly anomaly of the ocean surface area warmer than 28.5°C in the Atlantic and eastern North Pacific. The climatology used to calculate the monthly anomaly is from 1971-2000. In my analysis, I grouped the data by year instead of by month. The positive values indicate a SST above 28.5°C and the negative values indicate a SST below 28.5°C. The phases were defined as follows:

- WHWP Positive Phase: years when the WHWP index is greater than or equal to 0.67

    - Associated with an anomalously warm AWP

- WHWP Negative: years when the WHWP index is less than or equal to -0.67

- WHWP Neutral: years when the WHWP index is between -0.67 and 0.67

- where 0.67 is the mean WHWP index value from 1948-2024

For extreme heat over the Great Plains region, I sourced my data from the Copernicus fifth generation European Centre for Medium-Range Weather Forecasts (ECMWF) atmospheric reanalysis of the global climate (ERA-5). Using ERA-5 data for Maximum Monthly Temperature (2m surface air temperature in Kelvin), I calculated anomalies, witht the anomalously high maximum temperatures representing extreme heat. I also grouped this data by year instead of by month.

**Citation and Links**

Wang, C., and D.B. Enfield, 2001: The tropical Western Hemisphere warm pool, Geophys. Res. Lett., 28, 1635-1638. [AOML](http://www.aoml.noaa.gov/) and [PSL](https://psl.noaa.gov/).

[NOAA Climate Indices](https://psl.noaa.gov/data/climateindices/list/)

[WHWP Data](https://psl.noaa.gov/data/correlation/whwp.data)

Muñoz Sabater, J. (2019) - ERA5-Land monthly averaged data from 1950 to present. Copernicus Climate Change Service (C3S) Climate Data Store (CDS). DOI: 10.24381/cds.68d2bb30 (Accessed on 02-DEC-2024).

[Copernicus ERA-5 Download Page](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-land-monthly-means?tab=overview)

## **Results and Analysis**

The code showing how the following figures were created can be found here [clim680proj_WHWP.ipynb](https://github.com/istempko/clim680_project/blob/main/clim680proj_WHWP.ipynb).
The environment used can be found here [climate.yaml](https://github.com/istempko/clim680_project/blob/main/climate.yaml).
All the figures can also be found in a separate folder here [figures](https://github.com/istempko/clim680_project/tree/main/figures).

**Figure 1**

![](/figures/clim680_figure1.png)

Figure 1: The WHWP index plotted over time shows that the WHWP index is trending positive.

**Figure 2**

![](/figures/clim680_figure2.png)

**Figure 3**

![](/figures/clim680_fig3.png)

Figures 2 and 3: Scatter plot and line graph showing the Phases of the WHWP over time. As shown by the line of best fit, on average, the temperature of the WHWP has increased over time. 

**Figure 4**

![](/figures/clim680_fig4.png)

Figure 4: Maximum Temperatures in the Great Planes during WHWP Positive, Neutral, and Negative. Each plot shows anomalously high maximum temperatures in the Great Plains, so to further investigate, I plotted the composite maximum temperature differences.

**Figure 5**

![](/figures/clim680_fig5.png)

Figure 5: Plots of the Composite differences clearly show anomalously high maximum temperatures in the Great Plains during WHWP postive phases, as expected.

**Figure 6**

![](/figures/clim680_fig6.png)

**Figure 7**

![](/figures/clim680_fig7.png)

Figures 6 and 7: Testing for significance shows that much of the anomalously high maximum temperatures in the Great Planes are statistically significant with a 95% confidence level. 

**Figure 8**

![](/figures/clim680_fig8.png)

Figure 8: The fluctuations tend to allign, during Positive WHWP Phase there are usally also high Maximum Temperature Anomalies.

**Figure 9**

![](/figures/clim680_fig9.png)

Figure 9: Upon calculating a correlation coefficient then getting the correlation over a domain, there does not appear to be a correlation between Maximum Temperature Anomalies and WHWP index. 

## **Summary**
Initially, I analyzed the link between the Tropical Northern Atlantic (TNA) index and maximum temperature, which showed non-statistically significant extreme heat in the Great Plains. The lack of statistical significance can be explained by the bounds of the TNA not including the Caribbean Sea nor Gulf of Mexico—the most significant regions of latent heat flux into the GPLLJ. Thus, the WHWP index is a much better indicator for extreme heat in the GPLLJ. Analyzing the link between the WHWP index and maximum temperature did indeed show a connection with an anomalously warm AWP and extreme heat in the great plains. The results were statistically significant, but not correlated. The lack of correlation can be explained by the  nonlinear relationship of the WHWP index with maximum temperature, meaning there is not a constant rate of change between them. Since there are so many variables that impact weather, the relationship is unlikely to be linear. To further investigate the link between the WHWP index and extreme heat in the Great Plains, simulations of the GPLLJ could be run to model the behavior of the jet during phases of the WHWP index. 

## **References**
Green, B., Marshall, J., and Donohoe, A. (2017). Twentieth century correlations between extratropical SST variability and ITCZ shifts. Geophys. Res. Lett., 44, 9039–9047, https://doi.org/10.1002/2017GL075044.

Lopez, H., Kim, D., West, R., and Kirtman, B. (2022). Modulation of North American heat waves by the tropical Atlantic warm pool. Journal of Geophysical Research: Atmospheres, 127, e2022JD037705, https://doi.org/10.1029/2022JD037705.

Povea Perez, Y.: Atlantic Warm Pool: climate variability, thermal ocean-atmosphere interactions and remote response to ENSO and NAO., EGU General Assembly 2020, Online, 4–8 May 2020, EGU2020-4893, https://doi.org/10.5194/egusphere-egu2020-4893, 2020.
