#  Seismic Noise Filtering System

A web-based application for accessing, processing, and filtering seismic data from NASA's IRIS dataset with specialized support for Martian seismic data. This system provides an intuitive Streamlit interface to retrieve and clean seismic data, exporting filtered results in CSV format.



## Features

- ** Martian Data Specialization**: Optimized for processing Mars seismic data from InSight mission
- ** Advanced Filtering**: Multiple noise reduction algorithms using Obspy signal processing
- ** Interactive Web UI**: Streamlit-powered interface for real-time parameter configuration
- ** CSV Export**: Download filtered seismic data in standardized CSV format
- ** Real-time Visualization**: Preview raw and filtered data with interactive plots
- ** Multi-Planetary Support**: Access data from Earth, Mars, and other planetary bodies
- ** Cloud Ready**: Deployable via GitHub Pages and Streamlit sharing

##  Quick Start

### Prerequisites

- Python 3.8+
- Modern web browser
- Internet connection (for data access)

### Installation

1. **Clone the repository**
   bash
   git clone https://github.com/JohnJomi/seismic-noise-app.git
   cd seismic-noise-app
2. Install dependencies
    pip install -r requirements.txt
3.Launch the application
  bash
  streamlit run app.py
4.Access the web interface.
  Open your browser and navigate to: http://localhost:8501
 Usage


1. Data Selection

Choose time range and station network
Specify seismic channels and components
Mars Specialization: Pre-configured for InSight mission data

2. Filter Configuration

Bandpass Filter: Set frequency ranges using Obspy
Noise Reduction: Multiple Obspy-based algorithms
Detrending Options: Remove linear/quadratic trends
Decimation: Adjust sampling rates as needed

3. Processing & Export

Preview filtered waveforms in real-time
Validate data quality metrics
Download results as CSV files
Access processing metadata and station information


Project Structure

seismic-noise-app/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies (Obspy, Streamlit, etc.)
├── index.html            # Main web interface
├── main.html             # Additional HTML pages
├── tutorial.html         # Tutorial documentation
├── script.js             # Client-side JavaScript
├── style.css             # Stylesheets
├── .streamlit/           # Streamlit configuration
├── .github/workflows/
│   └── static.yml        # GitHub Pages deployment
└── output/               # Generated CSV files (if any)

Technology Stack

Backend: Python with Obspy for seismic processing
Web Framework: Streamlit for interactive UI
Data Access: NASA IRIS API integration
Visualization: Built-in Streamlit charts + custom JS
Deployment: GitHub Pages + Streamlit sharing
Specialization: Optimized for Martian seismic data analysis

 Data Sources

This system integrates with multiple data providers:

NASA IRIS: Primary seismic data source
InSight Mission: Martian seismic data specialization
Planetary Data System: Multi-planetary datasets

 Sample Output
The CSV export includes:

Timestamp data
Raw seismic waveforms
Filtered seismic data using Obspy
Processing metadata
Quality metrics
Station information (particularly Mars stations)
🛠️ Development

Adding New Filters

Implement filter using Obspy in app.py
Add Streamlit UI controls in the application
Update processing pipeline with new Obspy methods
Custom Data Sources

Extend the IRIS data fetcher to support additional planetary data providers.

Contributing

We welcome contributions! Please see our Contributing Guidelines for details.

Fork the repository
Create a feature branch
Commit your changes
Push to the branch
Open a Pull Request


Acknowledgments

NASA IRIS for providing seismic data access
InSight Mission team for Martian seismic data
Obspy development team for seismic processing library
Streamlit team for the web framework
Contributors and testers of this system

📞 Support
For support and questions:
📧 Email: john.jomi@btech.christuniversity.in or johnjomi1234@gmail.com
🐛 Issue Tracker
📚 Documentation
🔄 Version History

v1.0.0 (Current): Initial release with Mars data specialization
v0.5.0: Beta release with Streamlit integration
v0.1.0: Proof of concept with basic filtering
