# Go-Around Detection at LPPT based on Deep Learning Models using ADS-B and Meteorological Data

Go-arounds are a standard manoeuvre during the final approach, often initiated by pilots flying or requested by air traffic controllers to abort the landing procedures. While there are few go-arounds, they represent a safety critical manoeuvre that impact negatively airport operations and air traffic control (ATC). Humberto Delgado Airport (LPPT) is the largest airport in Portugal and one of the busiest airports in Europe, despite having only two terminals and one runway, and it has experienced a significant growth in passengers and aircraft movements. This study investigates the use of **deep learning models**, to detect go-around events in the final approach phase at LPPT using ADS-B and meteorological data. Results show that the **attention-based Long Short Term Memory (LSTM) model** achieves a promising performance, identifying **50% to 60% of go-arounds**, comparable to other state-of-the-art approaches. Meteorological features, such as **turbulence and wind related features, aircraft energy and glideslope** were particularly informative. Overall, this study contributes to a more comprehensive understanding of go-around risk at LPPT and supports the study and development of early-warning tools for air traffic control.

This repository contains the code, datasets and trained models used in this thesis.

## Dataset Summary

| ------------------ | -------------------------------------- |
| **Total flights**  | 243,522 flights                        |
| **Time period**    | June 2023 – August 2025                |
| **Go-around rate** | 0.48%                                  |
| **Airport**        | Humberto Delgado Airport (LPPT)        |

To ensure reproducibility, the complete final dataset has been made openly available on [Figshare](https://figshare.com/s/94d64be301fda5f2ea1d).

## Methodology

The following figure shows the flowchart of the methodological process.

![Image](https://github.com/user-attachments/assets/48e4c04d-ef0c-4ccc-9514-f0bee0be1fe7)

## Data Sources

- **Flight Data**
  - Software Defined Radio (SDR) setup  
  - [OpenSky Network — Historical Dataset](https://opensky-network.org/)
- **Weather Data**
  - Meteorological Aviation Routine Weather Report (METAR) collected using Python’s [get-metars](https://pypi.org/project/get-metars)
  - European Centre for Medium-Range Weather Forecasts (ECMWF) provided by [Instituto Português do Mar e da Atmosfera (IPMA)](https://www.ipma.pt/pt/index.html)
    
## Models Implemented
- LSTM
- Bi-LSTM
- GRU
- LSTM with an attention layer
- Bi-LSTM with an attention layer
- GRU with an attention layer

The following figure shows the model architecture of the LSTM with an attention layer.
![Image](https://github.com/user-attachments/assets/29cbc840-ef1a-4cef-ae31-5e8f4ff5d1ba)

<img width="1189" height="590" alt="Image" src="https://github.com/user-attachments/assets/b741d660-d3e3-48af-9f56-81952b849500" />







