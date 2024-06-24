# Physical Layer Parameters Collection from Firecells Testbed 5G Labkit 40

## Overview

his repository contains scripts and tools for collecting physical layer parameters (RSSI, RSRP, RSRQ, and SINR) from the Firecells testbed 5G Labkit 40. The User Equipment (UE) used in this setup is the Teltonika RUTX50 router. The distance between the gNB (gNodeB) and the UE is fixed at 1 meter, with no mobility considered in this test setup.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Setup and Installation](#setupandinstallation)
- [Usage](#usage)
- [Data Collection](#datacollection)
- [Graphs and Visulaization](#graphs)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The aim of this project is to provide a simple and effective way to monitor and log key physical layer parameters in a controlled 5G test environment. The scripts in this repository connect to the Teltonika RUTX50 router via SSH to retrieve and log parameters such as RSSI, RSRP, RSRQ, and SINR.

## Requirements

List the software and packages required to run the code in this repository. For example:

- Python 3.6+
- Teltonika RUTX50 Router
- Firecells 5G Labkit 40
- Matplotlib
- pyQt5

## Installation

Instructions for setting up the environment and installing the required packages.

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/5G-Physical-Layer-Parameters.git
cd 5G-Physical-Layer-Parameters
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

To run the data collection and visualization tool, execute the following command, This will start the graphical user interface (GUI) for the application. The GUI allows you to start and stop the data collection process and visualize the collected data in real-time.

   ```sh
   python3 25062024gpsgsmstates.py
   ```
        
# Data Collection

The script 25062024gpsgsmstates.py initiates an SSH connection to the RUTX50 router and sends commands to retrieve physical layer parameters. The collected data is stored in a CSV file with the following columns:

- TIME_STAMP
- LATITUDE
- LONGITUDE
- ACCURACY
- TX
- RX
- RSSI
- RSRP
- SINR
- RSRQ

# CSV Filename

The CSV file is named using the format PHY_TEST_YYYY-MM-DD_HH-MM-SS.csv and is saved in the current directory.

# Graphs and Visualization

The GUI application provides real-time plots of the following parameters:

- RSSI, RSRP, RSRQ on one subplot
- SINR on a separate subplot

These plots are updated in real-time as data is collected from the router.

## Contributing

We welcome contributions from the community. To contribute:

- Fork the repository.
- Create a new branch with a descriptive name.
- Make your changes and test them thoroughly.
- Submit a pull request with a detailed description of your changes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.


## Contact

For any questions or issues, please open an issue in this repository or contact the project maintainer at muhammadwaseem.akhtar@miun.se

