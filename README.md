Shiny Climate Explorer
=========

### Analyze GHCN climatological data at individual stations  

![Shiny_ClimateExplorer dualmode](https://github.com/awentland90/Shiny_ClimateExplorer/blob/master/data/station_analysis.png)

### Explore GHCN Stations

![Shiny_ClimateExplorer dualmode](https://github.com/awentland90/Shiny_ClimateExplorer/blob/master/data/station_explorer.png)


Download & Installation
--------

### Latest Code on GitHub

You can also use the following link to access the git repository:

*   **Git Repository:**

   The git repository can be found at: <https://github.com/awentland90/Shiny_ClimateExplorer>
   
    Get it using the following command:

        $ git clone git://github.com/awentland90/Shiny_ClimateExplorer.git
        
*   **Run Locally:**

    To run on your local machine, paste the following code into the R console:
    
        install.packages(c("shiny", "leaflet", "rnoaa"), repos="http://cran.rstudio.com/")
		library(shiny)
		runGitHub("Shiny_ClimateExplorer", "awentland90")

*   **NOAA/NCDC API Key:**

	You will need an API key to utilize the ncdc function from the rnoaa library.
	You can register (free) for a key here:
	
	[NCDC API Token Request](https://www.ncdc.noaa.gov/cdo-web/token)
	 
	I personally put the key in my .bash_profile:
	
		export NOAA_KEY="API_key_here"
	
	You can find other options for using the key on the rnoaa github page here:

	[rnoaa NCDC Authentication](https://github.com/ropensci/rnoaa/tree/492cf5a4ae440e35a909c5e4721ee302166cdd47#ncdc-authentication)


Citations
--------
*   **Global Historical Climatology Network (GHCN)**

	Menne, M.J., I. Durre, B. Korzeniewski, S. McNeal, K. Thomas, X. Yin, S. Anthony, R. Ray,
	
	R.S. Vose, B.E.Gleason, and T.G. Houston, 2012
	
	Global Historical Climatology Network - Daily (GHCN-Daily), Version 3.
	
	NOAA National Climatic Data Center. http://doi.org/10.7289/V5D21VHZ

*   **rnoaa (R library)**

	Scott Chamberlain (NA). rnoaa: 'NOAA' Weather Data from R.
	
	R package version 0.6.6. <https://github.com/ropensci/rnoaa>
	
*   **Leaflet (R library)**
	
	Joe Cheng and Yihui Xie (2016). leaflet: Create Interactive Web Maps
	
	with the JavaScript 'Leaflet' Library. R package version 1.0.1.
	
	<https://CRAN.R-project.org/package=leaflet>