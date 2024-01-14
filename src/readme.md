# Urban Areas Exploration with Geemap

## Introduction
This project involves the application of supervised and unsupervised classification algorithms on satellite images using Google Earth Engine with Geemap.

## Installation
To get started, install and import all the libraries found in the "Package installation and initial configuration" section. If `geemap` is not installed, unzip it using the following command:
```
!pip install geemap
```

## Google Earth Engine Registration
1. Register on [Google Earth Engine](https://earthengine.google.com/).
2. Select "Register a Noncommercial or Commercial Cloud project" and choose "Unpaid usage" option (select the academic project).
3. Create a new project with an ID (e.g., `ee-email_address`).
4. Then select the option "Continue to Summary" and confirm your project and confirm your project.

## Environment Map Setup
1. Once the project has been created, returning to the program, we will proceed to execute section "Creation of the Environment Map"  when executing the command `Map = geemap.Map()`, you will be asked, on the bottom, for an access
code to be able to use this tool.

2. To obtain it, click on the link that appears on the screen, which is in the form
```
https://code.earthengine.google.com/client-auth?scopes=https%3A//www.googleapis.com/auth/earthengine%20https%3A//www.googleapis.com/auth/devstorage.full_control&request_id=ixRamrf9hpSl4ep2VsF6eedjddnYNcXJRN_MTuxKbi4&tc=YYkxdJqyS_UFpT8zJbaWkKcgqfO2HH5Fbs9M0R4UgpA&cc=cABRbrNVmV6uEsERNuMn5RS7T0of6QIlyrDkzxKr_Hc
``` 
(it does not necessarily have to be the same).

3. Once you click on this link, you will be asked to log in with google and create/choose a work project (you must use the e-mail and project ID used in Google Earth Engine).

4. Then select the option "Generate Token". Once clicked, select the Google account you wish to work with. You will then get an alert that "Google has not verified this application", however, select the "Continue" option and in the next 
window, select all selectable objects.

5. Once you have done this, you will have the authorization code, which is located at the bottom of the notification. Once copied, paste it into the corresponding space in the program and press enter. 

## Supervised Classification
### Initial Steps
Remember that the supervised one can only be run for points within the USA. 

1. Initialize the section `Training + Classification` to obtain a map with the image of interest marked and all categories sorted according to the legend and predefined labels.

### Accuracy Verification

2. The following sections (`Training Data` and `Validation Data`) can be run to check the accuracy of the classification performed.

3. If you want to obtain the percentage of the `region`, you must run the `Ratios` section.

## Unsupervised Classification
This section is independent of the previous one (it can be executed without having executed the supervised classification, although it is necessary to have processed the `Creation of the Environment Map` section in order to have a 
working point).

1. Run the first section to determine the training data. If you want to visualize the number of optimal clusters, run the `Determinate Cluster Number` section.
2. Finally, run the `Classification` section, adjusting the desired number of clusters in `n_clusters` to obtain the results of the unsupervised classification.


## License
This project is licensed under the [MIT License](../LICENSE).

## References

Wu, Q., (2020). *geemap: A Python package for interactive mapping with Google Earth Engine*. The Journal of Open Source Software, 5(51), 2305. [https://doi.org/10.21105/joss.02305](https://doi.org/10.21105/joss.02305)

