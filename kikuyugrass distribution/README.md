# Kikuyugrass species distribution model

This project creates a species distribution model for kikuyugrass (*Cenchrus clandestinus*) in California using iNaturalist observations and [CHELSA](https://chelsa-climate.org/) climate data. The model uses Maxent to predict suitable habitat based on bioclimatic variables.

## Notebooks

1. `1_query_inaturalist.md`: Query iNaturalist API to fetch observations of kikuyugrass in California, including location data and images.

2. `2_label_images.md`: Widget for manually reviewing and labeling iNaturalist images to validate species id, creating a clean dataset of confirmed kikuyugrass occurrences.

3. `3_generate_background_points.md`: Generate background (pseudo-absence) points for model training.

4. `4_prep_climate_data.md`: Download CHELSA climate data and extract climate data for point locations.

5. `5_train_maxent_model.md`: Train MaxEnt species distribution model, geographic cross-validation, and figures.

6. `6_generate_map.md`: Create final map showing the probability of kikuyugrass occurrence across California.