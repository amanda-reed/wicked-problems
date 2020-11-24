# Accessibility 1

<img src="ddm_pop20.png" width="450" height="450" />  <img src="bel_adm3_ppp.png" width="450" height="525" /> 

After importing adm3 data for Belgium from GADM, I cropped and masked the raster to include data for solely Dendermonde, a subdivision of Oost-Vlaanderen with a population of approximately 200,000. The first plot shows a simple density plot of the region while the second plot uses the spatial probability distribution to create a point pattern of the region. 
<img src="ddm_density3.png" width="600" height="700" />
After establishing the bandwidth, I created a density plot based on that value and added contour lines to show the boundaries of the more populated areas of Dendermonde. 

<img src="pop_polys.png" width="600" height="600" /> 

Based on the contour lines, I isolated the inside and outside polygons. I then brought the two sets of polygons together and filtered the largest polygon. On a simple density plot, the polygons outline the most urban areas of the region.

![](ddm_dens_dots.png)

Using the urban area polygons, I identified the central points of each area and plotted points based on the overall population size and density of the area. 
