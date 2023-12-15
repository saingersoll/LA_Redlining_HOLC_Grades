# LA Redlining and HOLC Grade Exploration

Present-day environmental justice may reflect legacies of injustice in the past. The United States has a long history of racial segregation which is still visible. During the 1930's the Home Owners' Loan Corporation (HOLC), as part of the New Deal, rated neighborhoods based on their perceived safety for real estate investment. Their ranking system, (A (green), B (blue), C (yellow), D (red)) was then used to block access to loans for home ownership. Colloquially known as "redlining", this practice has had widely-documented consequences not only for community wealth, but also health[^1]. Redlined neighborhoods have less greenery[^2] and are hotter than other neighborhoods[^3]. Redlines and greenspace: the relationship between historical redlining and 2010 greenspace across the United States[^4].

[^1]: Gee, G. C. (2008). A multilevel analysis of the relationship between institutional and individual racial discrimination and health status. American journal of public health, 98(Supplement_1), S48-S56.
[^2]: [Nardone, A., Rudolph, K. E., Morello-Frosch, R., & Casey, J. A. (2021).  Environmental health perspectives, 129(1), 017006.
[^4] Hoffman, J. S., Shandas, V., & Pendleton, N. (2020). The effects of historical housing policies on resident exposure to intra-urban heat: a study of 108 US urban areas. Climate, 8(1), 12. 

Check out coverage by the [New York Times](https://www.nytimes.com/interactive/2020/08/24/climate/racism-redlining-cities-global-warming.html).

A recent study found that redlining has not only affected the environments communities are exposed to, it has also shaped our observations of biodiversity.^[Ellis-Soto, D., Chapman, M., & Locke, D. H. (2023). Historical redlining is associated with increasing geographical disparities in bird biodiversity sampling in the United States. Nature Human Behaviour, 1-9.] Community or citizen science, whereby individuals share observations of species, is generating an enormous volume of data. Ellis-Soto and co-authors found that redlined neighborhoods remain the most undersampled areas across 195 US cities. This gap is highly concerning, because conservation decisions are made based on these data.

Check out coverage by [EOS](https://eos.org/articles/bird-biodiversity-reports-reflect-cities-redlined-past?utm_source=EosBuzz&mkt_tok=OTg3LUlHVC01NzIAAAGOx3ckQPpeDY3QyFKdUnBSYqILj3qLrgb_Q2lasphwcF90xEzMgjZFUo3NHsw3caXDcZe6I8D8qdVsSRr3wzhb6LKAQRgNo8ffhjieEbDwMw).

### Data
#### EJScreen
We will be working with data from the United States Environmental Protection Agency's EJScreen: Environmental Justice Screening and Mapping Tool.

According to the [US EPA website](https://www.epa.gov/ejscreen/purposes-and-uses-ejscreen)[^5]:

>This screening tool and data may be of interest to community residents or other stakeholders as they search for environmental or demographic information. It can also support a wide range of research and policy goals. The public has used EJScreen in many different locations and in many different ways.
>
>EPA is sharing EJScreen with the public:  
> - to be more transparent about how we consider environmental justice in our work,  
> - to assist our stakeholders in making informed decisions about pursuing environmental justice and,   
> - to create a common starting point between the agency and the public when looking at issues related to environmental justice.

[^5]: EJScreen: Environmental Justice Screening and Mapping Tool | US EPA, <www.epa.gov/ejscreen>. 

EJScreen provides on environmental and demographic information for the US at the Census [tract](https://en.wikipedia.org/wiki/Census_tract) and [block group](https://en.wikipedia.org/wiki/Census_block_group) levels. You will be working with block group data that has been downloaded from the [EPA site](https://www.epa.gov/ejscreen/download-ejscreen-data). To understand the associated data columns, you will need to explore the Technical Documentation and column description spreadsheet available in the data folder. I also encourage you to explore the [limitations and caveats](https://www.epa.gov/ejscreen/limitations-and-caveats-using-ejscreen) of the data.

#### Mapping Inequality
A team of researchers, led by the [Digital Scholarship Lab](https://dsl.richmond.edu/) at the University of Richmond have digitized maps and information from the HOLC as part of the [Mapping Inequality](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58) project[^6].

[^6]: “Mapping Inequality.” Digital Scholarship Lab, <dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58>. 

We will be working with maps of HOLC grade designations for Los Angeles. Information on the data can be found [here](https://dsl.richmond.edu/panorama/redlining/#loc=5/39.1/-94.58&text=downloads).[^7].

[^7]: Robert K. Nelson, LaDale Winling, Richard Marciano, Nathan Connolly, et al., “Mapping Inequality,” American Panorama, ed. Robert K. Nelson and Edward L. Ayers, accessed October 17, 2023, <https://dsl.richmond.edu/panorama/redlining/> 

#### Biodiversity observations
The [Global Biodiversity Information Facility](gbif.org) is the largest aggregator of biodiversity observations in the world[^8]. Observations typically include a location and date that a species was observed. We will be working observations of birds from 2021 onward.

[^8]: GBIF, <www.gbif.org/>. 

**Note:** the data associated with this project is too large to include in the GitHub repo. Instead, download data from [here](https://drive.google.com/file/d/1lcazRbNSmP8Vj9sH1AIJcO4D1d_ulJij/view?usp=share_link). Unzip the folder and all the contents and store in your directory as follows. Don't include data when you push to GitHub!

```         
LA_Redlining_HOLC_Grades
│   README.md
│   Rmd/Proj files    
│
└───data
    │   column descriptions: EJSCREEN_2023_BG_Columns.xlsx
    │   metadata explation: ejscreen-tech-doc-version-2-2.pdf
    │   spatial data: EJSCREEN_2023_BG_StatePct_with_AS_CNMI_GU_VI.gdb
    |   biodiversity data: gbif-birds-LA/gbif-birds-LA.shp
```
