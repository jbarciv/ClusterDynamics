# Urban Areas Exploration with Geemap

## Introduction
This project involves the application of supervised and unsupervised classification algorithms on satellite images using Google Earth Engine with Geemap.

## Installation
To get started, install the required Python packages. If `geemap` is not installed, unzip it using the following command:
```
!pip install geemap
```

## Google Earth Engine Registration
1. Register on [Google Earth Engine](https://earthengine.google.com/).
2. Create a new project with an ID (e.g., `ee-email_address`).
3. Select "Register a Noncommercial or Commercial Cloud project" and choose "Unpaid usage."
4. Execute the code under "Creation of the Environment Map" to generate an access code.

## Environment Map Setup
1. Execute the command `Map = geemap.Map()` and provide the access code when prompted.
2. Customize the geographical coordinates in the "Creation of the Environment Map" section for the analysis point.

## Supervised Classification
### Initial Steps
1. Navigate to the "Training + Classification" section.
2. Run the code to obtain a map with marked areas based on predefined labels.

### Accuracy Verification
1. Execute the "Training Data" and "Validation Data" sections to assess classification accuracy.
2. Run the "Ratios" section to obtain the percentage of the region.

## Unsupervised Classification
1. Run the "Determinate Cluster Number" section to visualize the optimal number of clusters.
2. Execute the "Classification" section, adjusting `n_clusters` for the desired cluster count.

Feel free to explore and analyze the results obtained from both supervised and unsupervised classification algorithms.

## License
This project is licensed under the [MIT License](LICENSE).

## References

Wu, Q., (2020). *geemap: A Python package for interactive mapping with Google Earth Engine*. The Journal of Open Source Software, 5(51), 2305. [https://doi.org/10.21105/joss.02305](https://doi.org/10.21105/joss.02305)

