# 🧮 Precision Estimator

[![GitHub](https://img.shields.io/badge/GitHub-SahSanjeev%2FPrecisionEstimator-black?logo=github)](https://github.com/SahSanjeev/PrecisionEstimator) [![Python](https://img.shields.io/badge/Python-3.7%2B-blue?logo=python)](https://www.python.org/)

A streamlined Python-based construction cost estimator tailored for **Precision Build Pros**, a Tennessee-based residential and commercial contracting company. This tool calculates accurate labor and material costs across various construction services using real-world price data from Precision Build Pros’ rate sheet.

Built by **sanjeev Sah** ([https://github.com/SahSanjeev](https://github.com/SahSanjeev)) to improve quoting speed, accuracy, and professionalism.

---

## 📋 Table of Contents

- [Features](#features)  
- [Getting Started](#getting-started)  
- [Usage](#usage)  
- [Project Structure](#project-structure)  
- [Roadmap](#roadmap)  
- [About Precision Build Pros](#about-precision-build-pros)  
- [Contributing](#contributing)  
- [License](#license)  
- [Contact](#contact)  

---

## Features

- Estimate pricing for multiple construction services including:  
  - Flooring (LVP, LVT, laminate, hardwood)  
  - Tile (installation, backsplash, removal)  
  - Drywall (replacement & new construction)  
  - Trim (baseboards, crown molding, window & door trim)  
  - Paint & stain (walls, ceilings, trim, wood)  
  - Framing (interior)  
- Accepts input by square footage, linear footage, or per sheet  
- Provides fast cost breakdown using Precision Build Pros’ actual rates  
- Easy to update and customize services and pricing  
- Command-line interface (CLI) for quick interaction  
- Planned graphical user interface (GUI) for easier use  
- Modular code design for future expansions

---

## Getting Started

### Prerequisites

- Python 3.7 or higher installed on your machine  
- `pip` package manager

### Installation

1. Clone the repository

```bash
git clone https://github.com/SahSanjeev/PrecisionEstimator.git
cd PrecisionEstimator
```

2. Install required dependencies

```bash
pip install -r requirements.txt
```

### Running the Estimator

Run the main estimator script:

```bash
python pricingestimator.py
```

### Usage

Upon running, you will be prompted to:

- Select a service type (e.g., Flooring, Drywall)
- Input the measurement units (square footage, linear footage, sheets)
- Enter the quantity (e.g., 500 sqft)

The estimator will calculate and output an estimated price range based on the Precision Build Pros rate sheet.

Example

> Choose a Service: Flooring Install - LVP  
> Enter Square Footage: 500  
> Estimated Total: $2,000 - $3,500  

Project Structure

precision-estimator/
├── README.md                 # Project documentation
├── LICENSE                   # MIT License
├── requirements.txt          # Python dependencies
├── pricingestimator.py       # Main entry point script
├── estimator/                # Core estimator modules
│   ├── __init__.py
│   ├── core.py               # Calculation logic
│   ├── services.py           # Service definitions and pricing data
│   └── utils.py              # Helper functions
├── data/
│   └── price_sheet.csv       # Editable price sheet data
├── outputs/
│   └── sample_estimate.pdf   # Sample exported estimate (planned)
└── tests/
    └── test_core.py          # Unit tests

Roadmap

    Add support for regional pricing adjustments and taxes

    Integrate material tracking and inventory management

    Create a cloud-sync or multi-user version

    Develop a web-based interface for remote access

About Precision Build Pros

Precision Build Pros LLC is a licensed and insured contractor located in Cottontown, TN, serving Nashville and surrounding areas. With over 10 years of combined industry experience, Precision Build Pros specializes in remodeling, maintenance, handyman services, and property management.

This estimator tool was developed internally by Giampiero Zampolli to improve estimating accuracy and professionalism for client proposals.
Contributing

Contributions are welcome! Please follow these steps:

    Fork the repository

    Create a feature branch (git checkout -b feature-name)

    Commit your changes (git commit -m 'Add feature')

    Push to the branch (git push origin feature-name)

    Open a Pull Request

Please ensure code is well-documented and tested before submitting.
License

This project is licensed under the MIT License. See the LICENSE file for details.
Contact

Author: Sanjeev Sah
GitHub: https://github.com/SahSanjeev
Email: sanjeev.s.sah@gmail.com

Thank you for checking out Precision Estimator! Feel free to open issues or reach out with questions or suggestions.
