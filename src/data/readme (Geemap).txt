
First of all, it is necessary to install and import all the libraries found in the "Package installation and initial configuration" section, (unzip "!pip install geemap", 
if it is not installed on your computer). To do this, simply run the program lines

Next, it is necessary to register in "Google Earth Engine" with a valid Google account. To do this, go to its home page and select the button located on the top right bar "Get Started". Once this is done, select the "Register a 
Noncommercial or Commercial Cloud project" option along with the "Unpaid usage" option (select the academic project). Once selected, create the desired project along with an ID (you can put ee-"email_address", without at). 
Then select the option "Continue to Summary" and confirm your project and confirm your project.

Once the project has been created, returning to the program, we will proceed to execute section "Creation of the Environment Map"  when executing the command "Map = geemap.Map()", you will be asked, on the bottom, for an access
code to be able to use this tool. To obtain it, click on the link that appears on the screen, which is in the form " https://code.earthengine.google.com/client-auth?scopes=https%3A//www.googleapis.com/auth/earthengine%20https%3A//www.googleapis.com/auth/devstorage.full_control&request_id=ixRamrf9hpSl4ep2VsF6eedjddnYNcXJRN_MTuxKbi4&tc=YYkxdJqyS_UFpT8zJbaWkKcgqfO2HH5Fbs9M0R4UgpA&cc=cABRbrNVmV6uEsERNuMn5RS7T0of6QIlyrDkzxKr_Hc"
(it does not necessarily have to be the same). Once you click on this link, you will be asked to log in with google and create/choose a work project (you must use the e-mail and project ID used in Google Earth Engine).
Then select the option "Generate Token". Once clicked, select the Google account you wish to work with. You will then get an alert that "Google has not verified this application", however, select the "Continue" option and in the next 
window, select all selectable objects. Once you have done this, you will have the authorization code, which is located at the bottom of the notification. Once copied, paste it into the corresponding space in the program and press enter. 

Once you have done this, an interactive map should appear with the region of interest boxed in red. If you wish to change the analysis point, change the geographical coordinates of "point" within the "Creation of the Environment Map" 
section.

Now, you can proceed to run the supervised and unsupervised classification algorithm.

Supervised Classification:
Remember that the supervised one can only be run for points within the USA. 
Initializes the section "Training + Classification" to obtain a map with the image of interest marked and all categories sorted according to the legend and predefined labels.
according to the legend and the predefined labels. The following sections ("Training Data" and "Validation Data") can be run to check the accuracy of the classification performed.
If you want to obtain the percentage of the "region", you must run the "Ratios" section.

Unsupervised Classification:
This section is independent of the previous one (it can be executed without having executed the supervised classification, although it is necessary to have processed the "Creation of the Environment Map" section in order to have a 
working point). Run the first section to determine the training data. If you want to visualize the number of optimal clusters, run the "Determinate Cluster Number" section.
Finally, run the "Classification" section, adjusting the desired number of clusters in "n_clusters" to obtain the results of the unsupervised classification.
