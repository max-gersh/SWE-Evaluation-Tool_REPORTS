# Spatial Estimates of SWE for the Rio Grande Basin Using the SWE Evaluation Tool (SWEET)

This repository provides workflows, documentation, and resources for generating spatial estimates of Snow Water Equivalent (SWE) across the Rio Grande Basin using the SWE Evaluation Tool (SWEET). The project enables users to compare and evaluate multiple SWE products to support hydrologic assessments, water supply forecasting, snow monitoring, and research applications.

## Introduction
The Rio Grande (RG) is a snowmelt-driven river system with up to 75% of its water originating from seasonal snowpack in the mountains of Colorado and northern New Mexico (Moeser et al., 2021). Snowpack acts as a natural reservoir in the RG Basin, gradually releasing meltwater during the spring and early summer months, sustaining streamflow and providing vital water supply for downstream users. However, regional decreases in snowpack volume and earlier snowmelt timing, especially throughout the western U.S. and New Mexico, can lead to reduced water availability (Mote et al., 2005; EPA, 2016b; Mote et al., 2018; Hale et al., 2023).

Long-term changes in snowpack patterns and timing can serve as an indicator of climate change, while understanding short-term changes is critical for monitoring seasonal variability and forecasting seasonal water supply. Monitoring snowpack provides valuable data on shifts in precipitation patterns and temperatures, helping scientists and decision-makers better understand and manage climate-related challenges.

Snow water equivalent (SWE) is the estimate of the depth of liquid water contained in the snowpack. SWE is the standard metric in estimating the volume of meltwater in the snowpack, which plays a critical role in the seasonal snow water supply in the RG Basin. SWE is measured at in-situ Snow Telemetry (SNOTEL) sites throughout the RG Basin and the greater Western U.S. However, the spatial distribution of SWE is complex and often difficult to estimate outside of the in-situ SNOTEL measurements. While SNOTEL provides important point-based measurements, it has been suggested that these data may not be representative of the surrounding snow-covered area (Meromy et al., 2013). Whereas regional tendencies of spatial distribution are consistent, local snowpack volumes are more variable, all of which influences the magnitude and timing of snowmelt-driven runoff.

## SWE Evaluation Tool (SWEET)
The RG Basin, and more broadly the Western U.S., is experiencing a prolonged and severe drought (EPA, 2016a), exacerbated by a warming climate that increases evapotranspiration, reduces overall snowpack quantity, and reduces the seasonal duration of snowpack. The application of the SWE Evaluation Tool (SWEET) will supply scientists and decision-makers with an improved insight into the spatial distribution of SWE by providing real-time spatial SWE estimates for the RG Basin, its subbasins, and elevation bands within the basin.

Because no spaceborne sensor can directly measure SWE, spatial distribution of SWE must be estimated from remotely sensed observations coupled with modeling approaches. However, gridded SWE products are known to have accuracy issues across both mountainous and non-mountainous regions (Mudryk et al., 2025), resulting in a range of spatial SWE estimates for any given location. For this reason, NM OSE and INSTAAR are developing a tool to integrate various, suitable data products to build SWEET based on an ensemble of spatially estimated SWE. By taking an ensemble approach, the goal for SWEET is to provide spatial SWE estimations for the RG Basin that are, on average, equally or more accurate than any individual model (Thompson, 1977; Arsenault et al., 2015). In addition, the use of a single estimate calculated from an ensemble can reduce confusion for water managers about which product may be performing best, providing a path towards consistency throughout users, and is useful in identifying product outliers.

In the development of SWEET, building from previous research and our expertise, we have selected output from available models. Spatial resolution, temporal resolution, coverage, and data lag are model-dependent. These factors serve as key criteria in determining which models are selected, as they influence the model’s suitability for specific application in the project’s ensemble approach. The following models are included in the ensemble approach for WY2026 and are subject to change in the future.

### SNODAS SWE
The SNOw Data Assimilation System (SNODAS) represents a modeling and data assimilation system developed by the National Operational Hydrologic Remote Sensing Center (NOHRSC). SNODAS generates spatial estimates of SWE, snow cover, and snow depth through a combination of remotely sensed snow data and in-situ measurements of SWE from SNOTEL at a 1-km spatial resolution and 24-hour temporal resolution.

The national SNODAS dataset is available through the [SNODAS Data Products at National Snow and Ice Data Center (NSIDC), Version 1](https://nsidc.org/data/g02158/versions/1) (NOHRSC, 2004). SNODAS data can be viewed at the [NOHRSC Interactive Snow Information page](https://www.nohrsc.noaa.gov/interactive/html/map.html). Gridded observed snowfall images, seasonal totals, and data downloads in several formats can be found on the [National Gridded Snowfall Analysis page](https://www.nohrsc.noaa.gov/snowfall_v2/).

Refer to the [SNODAS User Guide](https://nsidc.org/sites/default/files/g02158-v001-userguide_2_1.pdf) and the [NSIDC Special Report 11](https://nsidc.org/sites/default/files/nsidc_special_report_11.pdf) (Barrett, 2003) for more information.

### UA/SWANN SWE
*Content describing UA/SWANN SWE workflow, model basis, resolution, and recommended usage will go here.*

### CU SWE
*Content describing CU SWE dataset characteristics, derivation, and integration steps will go here.*

## Acknowledgements
The work completed and presented in this report is funded by NASA Western Water Actions Office (WWAO), subcontract no. 1712706, as part of the Rio Grande River Basin Needs Assessment Report (WWAO and DBS&A, 2022). The development of SWEET would not have been possible without the efforts from our partner at INSTAAR, University of Colorado Boulder.

## References
Arsenault, R., Gatien, P., Renaud, B., Brissette, F., & Martel, J. L. (2015). A comparative analysis of 9 multi-model averaging approaches in hydrological continuous streamflow simulation. Journal of Hydrology, 529, 754-767.

Barrett, Andrew. (2003). National Operational Hydrologic Remote Sensing Center Snow Data Assimilation System (SNODAS) Products at NSIDC. NSIDC Special Report 11. Boulder, CO USA: National Snow and Ice Data Center. 19 pp.

Environmental Protection Agency [EPA]. (2016a). Climate Change Indicators: Drought. Web update: June 2024. Available at: https://www.epa.gov/climate-indicators/climate-change-indicators-drought. Accessed: March 31, 2025.

Environmental Protection Agency [EPA]. (2016b) Climate Change Indicators: Snowpack. Web update: June 2024. Available at: https://www.epa.gov/climate-indicators/climate-change-indicators-snowpack. Accessed: March 31, 2025.

Hale, K.E., Jennings, K.S., Musselman, K.N., Livneh, B., Molotch, N.P. (2023). Recent decreases in snow water storage in western North America. Communications Earth & Environment, 4(1), p. 170. Available at: https://doi.org/10.1038/s43247-023-00751-3.

Meromy, L., Molotch, N.P., Link, T.E., Fassnacht, S.R., & Rice, R. (2013). Subgrid variability of snow water equivalent at operational snow stations in the western USA. Hydrological Processes, 27, 2383-2400, doi: 10.1002/hyp.9355.

Moeser, C.D., Chavarria, S.B., and Wootten, A.M. (2021). Streamflow response to potential changes in climate in the Upper Rio Grande Basin: U.S. Geological Survey Scientific Investigations Report 2021–5138, 41 p., https://doi.org/10.3133/sir20215138.

Mote, P. W., Hamlet, A. F., Clark, M. P., & Lettenmaier, D. P. (2005). Declining mountain snowpack in western North America. Bulletin of the American Meteorological Society, 86(1), 39–50. https://doi.org/10.1175/BAMS-86-1-39.

Mote, P. W., Li, S., Lettenmaier, D. P., Xiao, M., & Engel, R. (2018). Dramatic declines in snowpack in the western US. Climate and Atmospheric Science, 1, 2. https://doi.org/10.1038/s41612-018-0012-1.

Mudryk, L., Mortimer, C., Derksen, C., Elias Chereque, A., Kushner, P. (2025). Benchmarking of snow water equivalent (SWE) products based on outcomes of the SnowPEx+ Intercomparison Project. The Cryosphere, 19(1), pp. 201–218. Available at: https://doi.org/10.5194/tc-19-201-2025.

NASA Wester Water Applications Office [WWAO] and Daniel B. Stephens & Associates, Inc. [DBS&A]. (2022). Rio Grande River Basin Needs Assessment Report. NASA WWAO Assessment Report. Available at: https://wwao.jpl.nasa.gov/documents/138/Water-Needs-Rio-Grande-Report-2022.pdf.

National Operational Hydrologic Remote Sensing Center [NOHRSC]. (2004). Snow Data Assimilation System (SNODAS) Data Products at NSIDC, Version 1. SWE Dataset. Boulder, Colorado USA. NSIDC: National Snow and Ice Data Center. https://doi.org/10.7265/N5TB14TC. Accessed: April 1, 2025, and as needed.

Thompson, P.D. (1977). How to improve accuracy by combining independent forecasts. Monthly Weather Review, 105(2), pp.228-229.
