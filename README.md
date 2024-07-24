Malaria is a fatal disease caused by parasite and is transmitted to humans and other animals through the bites of infected mosquitoes. People who are affected by malaria would typically experience high fever and chills. According to CDC, an estimated 229 million incidences of malaria were recorded in 2019 and 409,000 people died, where Africa accounted for most of the cases. In this project, I created 5 interactive visualization on malaria.
The data used for for this simple analysis is found in the tidytuesday open source project that contains a variety of dataset and tools. For the purpose of this project, I used the 2 of the 3 Malaria dataset,which is summarized below:
malaria_deaths.csv — Malaria deaths by country for all ages across the world and time
malaria _inc.csv — Malaria incidence by country for all ages across the world and time
For visualization, I used the ggplot2 package. The ggplot provides a wide range of really flexible interactive graphing tools, which could be used to meet very complex visualization objectives.

Visualization
1. To visualize the percentage change in incidence from a sample of 6 countries during the years captured (2000 - 2015). To achive this I plotted a goem_line graph of incidence against years scaling y axis to percentage format
2. To visualize the percentage change in incidence during the years captured of every individual country in the data set, I made use of the geom_point graph plotting percentage change of incidence in the years by the current year.
3. To visualize a better percentage change in incidence levels, I made use of geom_bar graph to plot for the entire data set as a whole and also narowed this to Nigeria.
4. To have a better representation of malaria cases in the world overtime, I merged the malaria incidence data with maps by the country code and used the geom_polygon and facet wrap functions to visuaize malaria incidence over time.
5. Finally I visualized an animated transitining plot of malaria death cases in Africa over time since Africa had the highest death cases. To achieve this, I merged the malaria deaths data with maps using mapname and filtered this to Africa. Then made use of the geom_polygon and animate functions to produce the animated chart of malaria death cases over time in Africa.
