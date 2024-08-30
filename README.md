
# CoolMetrix

![alt text](image.png)

CoolMetrix is a project that utilizes satellite data to measure urban heat, vegetation, and air quality. The project aims to identify how much hotter cities are compared to their surroundings. This information is essential for guiding efforts to make cities greener and cooler, ultimately supporting more sustainable urban planning.

## Overview

Urban Heat Islands (UHIs) refer to the phenomenon where urban areas experience higher temperatures than their rural surroundings. This is primarily due to human activities, reduced vegetation, and increased infrastructure like roads and buildings that retain heat. CoolMetrix provides insights into the UHI effect by analyzing satellite data, enabling the identification of heat hotspots within cities and suggesting mitigation strategies.

## Features

- **Urban Heat Measurement**: Uses satellite data to calculate temperature differences between urban and surrounding areas.
- **Vegetation Analysis**: Assesses vegetation cover through NDVI (Normalized Difference Vegetation Index) and EVI (Enhanced Vegetation Index).
- **Air Quality Monitoring**: Evaluates air quality using NO2 levels from satellite data.
- **Cooling Action Suggestions**: Based on the analysis, CoolMetrix suggests actions to mitigate the UHI effect, such as increasing green spaces or using reflective materials.

## Installation

To run this project locally, follow the steps below:

1. Clone the repository:

   ```bash
   git clone https://github.com/tensortrove/CoolMetrix.git
   cd coolmetrix
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```



## Usage

1. **Data Preparation**: Ensure that all required data is downloaded and placed in the correct directories.

2. **Run the Notebook**: Open the Jupyter notebook `UHI.ipynb` from the `notebooks/` directory and run all cells sequentially to process the data and generate results.

3. **View Results**: The notebook will output key metrics, visualizations, and suggested cooling actions for different regions.

4. **Export Results**: The results, including cooling action suggestions, can be exported as a CSV file for further analysis or reporting.

## Project Structure

```bash
CoolMetrix/
│
├── data/                     # Directory containing input data files
│   ├── chennai_regions_cooling_actions.csv
│   ├── chennai_regions_uhi_data.csv
│   ├── regions_chennai.csv
│   └── uhi_vs_features_16_day_intervals.csv
│
├── notebooks/                # Directory containing Jupyter notebooks
│   └── UHI.ipynb
│
├── plots/                    # Directory containing output plots and maps
│   ├── correlation_matrix.png
│   ├── feature_distributions.png
│   ├── hot_spots_map.html
│   └── predicted_future_uhi.png
│
├── presentation/             # Directory containing the project presentation
│   └── presentation.pptx
│
├── CODE_OF_CONDUCT.md        # Code of Conduct for contributors
├── LICENSE                   # Project license
└── README.md                 # Project documentation
```

## Data Sources

- **Satellite Data**: The project utilizes data from Google Earth to analyze temperature, vegetation, and air quality.
- **Chennai City Data**: Specific regions within Chennai, India, were analyzed to demonstrate the capabilities of CoolMetrix.

## Cooling Action Suggestions

Based on the analysis, the following actions are recommended for mitigating the UHI effect:

- **Increase Green Spaces**: Introduce more trees, green roofs, and green walls in regions with low NDVI.
- **Use Reflective Materials**: Implement reflective pavements and building materials in areas with high albedo.
- **Introduce Water Bodies**: Consider expanding or introducing water bodies in densely populated areas to cool the surroundings.
- **Pollution Control**: Implement measures to reduce NO2 levels in areas with poor air quality.

## Contributing

We welcome contributions to enhance the capabilities of CoolMetrix. If you would like to contribute, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

We would like to thank **Google Earth Engine** for providing the data and tools used in this project.

## Authors

- [@ankitdey-marsh](https://www.github.com/ankitdey-marsh)
- [@Terminal127](https://www.github.com/Terminal127)
- [@debjit-mandal](https://www.github.com/debjit-mandal)
- [@nilotpal-basu](https://www.github.com/nilotpal-basu)