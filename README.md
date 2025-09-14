# The Air We Breathe 🌎

A comprehensive Streamlit web application that visualizes global Air Quality Index (AQI) data through interactive maps and charts, providing insights into air pollution levels across cities worldwide.

## 🌟 Overview

**The Air We Breathe** is a data visualization dashboard that transforms complex air quality data into accessible, interactive visualizations. The application enables users to explore AQI values for different pollutants across multiple cities globally, making environmental data comprehensible and actionable.

## 🚀 Features

- **Interactive Global Maps**: Explore AQI data with geospatial plotting using Plotly and Folium
- **Multi-Pollutant Analysis**: Visualize different pollutant levels including PM2.5, PM10, CO, NO2, SO2, and O3
- **City-wise Comparisons**: Compare air quality metrics across different cities worldwide
- **Real-time Data Processing**: Clean and process air quality data for accurate visualization
- **Responsive Dashboard**: User-friendly interface optimized for various screen sizes
- **Environmental Insights**: Interpret environmental metrics with clear visual representations

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Data Visualization**: 
  - Plotly (interactive charts)
  - Folium (geospatial mapping)
- **Data Processing**: Pandas
- **Language**: Python 3.x

## 📁 Project Structure

```
air-we-breathe/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── data/
│   └── sample.csv        # Sample air quality dataset
├── README.md             # Project documentation
└── assets/               # Static assets (if any)
```

## 🔧 Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/ShruAgarwal/air-we-breathe.git
   cd air-we-breathe
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

4. **Access the app**

### Alternative: Virtual Environment Setup

```bash
# Create virtual environment
python -m venv air_quality_env

# Activate virtual environment
# On Windows:
air_quality_env\Scripts\activate
# On macOS/Linux:
source air_quality_env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

## 📊 Data Sources & Format

The application processes CSV data containing air quality measurements with the following structure:
- City names and geographical coordinates
- AQI values for different pollutants
- Timestamp information
- Pollution level categories

### Expected CSV Format
```csv
City,Country,Latitude,Longitude,PM2.5,PM10,CO,NO2,SO2,O3,AQI
New York,USA,40.7128,-74.0060,12.5,18.3,0.4,21.2,3.1,45.2,52
London,UK,51.5074,-0.1278,15.8,22.1,0.6,28.5,4.2,38.7,58
...
```

## 🎯 Use Cases

- **Environmental Research**: Analyze air pollution patterns across different regions
- **Policy Making**: Support environmental policy decisions with data-driven insights
- **Public Health**: Understand air quality impacts on community health
- **Educational Purpose**: Learn about data visualization and environmental science
- **Urban Planning**: Assess air quality for city development projects

## 🌐 Live Demo

Experience the application live at: [https://air-we-breathe.streamlit.app/](https://air-we-breathe.streamlit.app/)

## 📈 Key Visualizations

1. **Global AQI Heatmap**: Interactive world map showing AQI levels by color coding
2. **Pollutant Comparison Charts**: Bar charts and line graphs comparing different pollutants
3. **City Rankings**: Sorted lists of cities by air quality metrics
4. **Temporal Analysis**: Time-series visualizations (if temporal data available)
5. **Statistical Summaries**: Key statistics and insights about global air quality

## 🔍 Data Analysis Features

- **Data Cleaning**: Automated preprocessing of air quality data
- **Outlier Detection**: Identification and handling of anomalous readings
- **Missing Value Treatment**: Intelligent handling of incomplete data
- **Statistical Analysis**: Descriptive statistics and trend analysis
- **Correlation Analysis**: Relationships between different pollutants

### Theme Configuration
- Modern, clean interface design
- Color-coded air quality indicators
- Responsive layout for mobile and desktop
- Accessibility-focused color schemes

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

### Development Setup
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/new-feature`)
6. Create a Pull Request

## 📄 License

This project is open source. Please check the repository for specific license information.

## 👏 Acknowledgments

- **Data Sources**: Various environmental monitoring agencies
- **Streamlit Community**: For the excellent framework and community support
- **Open Source Contributors**: For the visualization libraries used

🚧 **Development Challenges**
During the creation of this project, several technical and design challenges were encountered:
**Data Quality & Processing**

- **Inconsistent Data Formats**: Handling varying air quality data structures from different global monitoring stations
- **Missing Values**: Implementing robust strategies to manage data gaps across cities and time periods
- **AQI Standardization**: Reconciling different international air quality measurement standards and calculation methods

**Visualization Complexity**

- **Multi-Library Integration**: Seamlessly combining Plotly and Folium for optimal interactive mapping performance
- **Performance Optimization**: Balancing rich interactive features with app loading speed and responsiveness
- **Accessibility Design**: Creating intuitive color schemes for pollution levels while maintaining visual accessibility standards

**Technical Implementation**

- **Streamlit Performance**: Optimizing application performance when handling large global datasets with multiple pollutants
- **Memory Management**: Efficiently managing memory usage when displaying comprehensive city data simultaneously
- **Cross-Platform Compatibility**: Ensuring consistent rendering and functionality across different devices and browsers
