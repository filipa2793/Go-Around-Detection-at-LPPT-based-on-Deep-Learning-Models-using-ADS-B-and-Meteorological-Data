# Go-Around-Detection-at-LPPT-based-on-Deep-Learning-Models-using-ADS-B-and-Meteorological-Data

Go-arounds are a standard manoeuvre during the final approach, often initiated by pilots flying or requested by air traffic controllers to abort the landing procedures. While there are few go-arounds, they represent a safety critical manoeuvre that impact negatively airport operations and air traffic control (ATC). Humberto Delgado Airport (LPPT) is the largest airport in Portugal and one of the busiest airports in Europe, despite having only two terminals and one runway, and it has experienced a significant growth in passengers and aircraft movements. This study investigates the use of deep learning models, to detect go-around events in the final approach phase at LPPT using ADS-B and meteorological data. Results show that the attention-based Long Short Term Memory (LSTM) model achieves a promising performance, identifying 50\% to 60\% of go-arounds, comparable to other state-of-the-art approaches. Meteorological features, such as turbulence and wind related features, aircraft energy and glideslope were particularly informative. Overall, this study contributes to a more comprehensive understanding of go-around risk at LPPT and supports the study and development of early-warning tools for air traffic control.

This repository contains the code used to obtain and process the data, to create new features and the models used. Additionally, it contains all the flight data and meteorological data gathered throughout the months and the post-processing dataset at Humberto Delgado Airport (LPPT). The flight data came from Automatic Dependent Surveillance-Broadcast (ADS-B) transmissions and it was collected from two distinct sources: through a Software Defined Radio (SDR) setup and from the historical dataset provided by the [OpenSky Network](https://opensky-network.org/). The meteorological data was collected from Meteorological Aviation Routine Weather Report (METAR) using the Python's [get-metars](https://pypi.org/project/get-metars) and short-term forecasts from the European Centre for Medium-Range Weather Forecasts (ECMWF) provided by [Instituto Português do Mar e da Atmosfera (IPMA)](https://www.ipma.pt/pt/index.html). The final dataset has 243 522 flights, starting from June 2023 to August 2025, with a go-around percentage of 0.48\%. The following figure shows the methodological process.

# 🛫 Go-Around Detection at LPPT using Deep Learning Models and ADS-B + Meteorological Data

Go-arounds are standard manoeuvres during final approach, often initiated by pilots or requested by air traffic controllers to abort landing. While rare, they are safety-critical events that significantly affect airport operations and air traffic control (ATC).

Humberto Delgado Airport (LPPT) is Portugal’s busiest airport and one of the most constrained in Europe, operating with only one runway. This study investigates the use of **deep learning models** to detect go-around events during the final approach at LPPT using **ADS-B** and **meteorological data**.

The attention-based **Long Short-Term Memory (LSTM)** model achieved strong performance, correctly identifying around **50–60% of go-arounds**, comparable to other state-of-the-art approaches. Features such as **turbulence**, **wind-related parameters**, **aircraft energy**, and **glideslope** proved particularly informative.

This repository contains the **code, datasets, and trained models** used in the analysis. It aims to support research into **early-warning systems** and **risk modeling** for air traffic control.

---

## 📁 Repository Structure



