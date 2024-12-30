## Background
In oceanography, a front is a boundary between two ocean masses. They can be distinguished by changes in parameters like Sea Surface Height (SSH), Temperature, Salinity, etc.

Jones et. al. 2018, is a notable paper where Principal Component Analysis and Gaussian Mixture Models were used on Argo float data in order to detect fronts in the Southern Ocean. 

Our attempt is to use BGC-Argo float data, which measures biogeochemical parameters like Chlorophyll, Dissolved Oxygen, Downwelling Irradiance, etc., in order to generate similar front boundaries in the Southern Ocean. Specifically, we're currently investigating Chlorophyll-A (CHLA) for its possibility of identifying southern ocean fronts. 

## Challenge
The main challenge with this approach is the fact that there's not a lot of data available in order to perform GMM in this region (below -30 S). The profiles aren't clean at all, with lots of NaN values, which can't be reliably interpolated or filled without leading to catastrophic errors affecting our models. 
