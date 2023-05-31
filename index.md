# CellularX: A Spatial-Temporal Dataset for User-Oriented AIOps in Cellular Network
We introduce cellularX, the first large-scale dataset focusing on user-level network experiences within cellular networks. Unlike existing datasets that either overlook user experience or merely provide traffic data, cellularX fills the gap in supporting Artificial Intelligence for IT Operations (AIOps) by offering multi-dimensional Key Performance Indicator (KPI) data collected from over thirty thousand users. It allows for individual-oriented network optimization to become a reality. Additionally, cellularX also provides a synthetic dataset specifically designed for the sim2real study within the AIOps. CellularX serves as a benchmark, enabling AIOps applications such as anomaly prediction and root cause analysis in cellular networks. 

The potential applications of CellularX include: 
- **Digital twin for 5G/6G Radio Access Networks (RAN)**: CellularX provides large-scale real-world KPI data that can be used to build a digital twin for RAN. The digital twin can simulate and preview unpredictable or costly operations in the real world, such as predictive maintenance, network optimization, etc.
- **Simulation-to-Real (sim2real) study**: CellularX provides a real and simulated comparison to help researchers understand the reality gap in user-level RAN scenarios and facilitate efficient knowledge transfer from simulated data to real scenarios.

#### Dataset Link

<!-- info: Provide a link to the dataset: -->
<!-- width: half -->
[cellularxdataset.github.io/](https://cellularxdataset.github.io/)



#### License

The dataset provided here is licensed under the **Creative Commons Attribution-NonCommercial (CC BY-NC)** license. This means that you are free to use, copy, modify, and distribute the dataset for *non-commercial purposes* as long as you provide attribution to the original author. The license restricts the use of the dataset for any commercial purposes without obtaining prior permission from the author. Please note that this license ensures the dataset's availability for academic and non-profit research, but prohibits its usage for commercial gain. For more details about the license, refer to the accompanying license file.



## Authorship

### Dataset Owners
#### Team(s)

<!-- scope: telescope -->
<!-- info: Provide the names of the groups or team(s) that own the dataset: -->
DNA Lab. Tongji University, Shanghai, China.


#### Author(s)
<!-- scope: microscope -->
<!-- info: Provide the details of all authors associated with the dataset:

(Usage Note: Provide the affiliation and year if different from publishing
institutions or multiple affiliations.) -->
- Shaoyu Dou, Ph.D. Student, Tongji University
- Kai Yang, Professor, Tongji University
- Xiangmin Zou, Ph.D. Student, Tongji University

### Funding Sources
#### Institution(s)
<!-- scope: telescope -->
<!-- info: Provide the names of the funding institution(s): -->
- Name of Institution
- Name of Institution
- Name of Institution

#### Funding or Grant Summary(ies)

<!-- scope: periscope -->
<!-- width: full -->
<!-- info: Provide a short summary of programs or projects that may have funded
the creation, collection, or curation of the dataset.

Use additional notes to capture any other relevant information or
considerations. -->
*For example, Institution 1 and institution 2 jointly funded this dataset as a
part of the XYZ data program, funded by XYZ grant awarded by institution 3 for
the years YYYY-YYYY.*

Summarize here. Link to documents if available.

**Additional Notes:** Add here

## Dataset Overview
#### Data Subject(s)
<!-- scope: telescope -->
<!-- info: Select ***all applicable**** subjects contained the dataset: -->
- Non-Sensitive Data about people
- Synthetically generated data
- Data about systems or products and their behaviors

#### Dataset Snapshot
<!-- scope: periscope -->
<!-- info: Provide a snapshot of the dataset:<br><br>(Use the additional notes
to include relevant information, considerations, and links to table(s) with
more detailed breakdowns.) -->

| Category            | Data                        |
| :------------------ | :-------------------------- |
| Dataset Name        | CellularXreal, CellularXsim |
| Size of Dataset     | x MB, 2.0 MB                |
| Number of Instances | xxx, ~18,000                |

**Above:** Summary of CellularX dataset



#### Content Description

<!-- scope: microscope -->
<!-- info: Provide a short description of the content in a data point: -->
- **CellularXreal** dataset consists of two parts: multidimensional KPI data and cellular information, where each record corresponds to a _timestamp_ and a _sampling cell_. The data contains a significant number of missing values since not all indicators are reported for each access.
The published KPI data encompasses 37947 users and consists of _eight dimensions_ of KPIs. These KPIs include uplink and downlink user experience rate, block error rate, the number of resource blocks, as well as RSRP of the service cell and uplink SINR. 

- **CellularXsim** provides **real-world KPI** data generated by user equipment while moving along four manually designed paths, as well as corresponding **simulated data** generated with six simulator configurations along the same routes. CellularXsim also includes a set of real-world data generated by randomly roaming within the study area. **Simulator configuations** and **base station infomation** are provided. Four KPI metrics are recorded, that are RSSI, SINR, RSRP, and RSRQ.


### Sensitivity of Data
#### Sensitivity Type(s)
<!-- scope: telescope -->
<!-- info: Select ***all applicable*** data types present in the dataset: -->
- Anonymous Data

#### Field(s) with Sensitive Data
<!-- scope: periscope -->
<!-- info: List fields in the dataset that contain S/PII, and specify if their collection was intentional or unintentional.

Use additional notes to capture any other relevant information or
considerations. -->

**Intentional Collected Sensitive Data**

No sensitive data was intentionally collected.

**Unintentionally Collected Sensitive Data**

All user devices involved in the data set have been anonymized, and the data set only collected data from base stations in a part of the city block, so any user's behavior and identity cannot be inferred using any additional methods.


### Dataset Version and Maintenance
#### Maintenance Status
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Limited Maintenance** - The data will not be updated, but any technical issues will be addressed.

#### Version Details
<!-- scope: periscope -->
<!-- info: Provide details about **this** version of the dataset: -->
**Current Version:** 1.0

**Last Updated:** 06/2023

**Release Date:** N/A

#### Maintenance Plan
<!-- scope: microscope -->
<!-- info: Summarize the maintenance plan for the dataset: -->
CellularX is collected in the real world at one time for academic purposes, and maintenance will be limited.

**Feedback:** For feedback, reach out to shaoyu@tongji.edu.cn.



## Example of Data Points
#### Primary Data Modality
<!-- scope: telescope -->
<!-- info: Select **one**: -->
- Time Series
- Geospatial Data


#### Typical Data Point
<!-- width: half -->
<!-- info: Provide an example of a typical data point and describe what makes
it typical.

**Use additional notes to capture any other relevant information or
considerations.** -->

Below are examples of kind data in the cellularX dataset.
- Time series data in cellularXreal dataset, containing missing values.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531162154445.png" alt="Time series data in cellularXreal dataset"  />

- Geospatial data in cellularXreal dataset

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531162027544.png" alt="image-20230531162027544" style="zoom:50%;" />

- Simulated time series data in cellularXsim dataset.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531162310523.png" alt="image-20230531162310523"  />

- Collected time series data in cellularXsim dataset.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/16681685521414_.pic.jpg" alt="16681685521414_.pic"  />

- Geospatial data in cellularXsim dataset

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/16691685521499_.pic.jpg" alt="16691685521499_.pic"  />



## Data Fields

### CellularXreal dataset

#### Time Series Data

| KPI Name | Description                            | Unit | Type    |
| :------- | :------------------------------------- | :--- | :------ |
| RSRP     | RSRP of service cell                   | dBm  | Integer |
| ULThrp   | Uplink experience rate                 | Mbps | Float   |
| DLThrp   | Downlink experience rate               | Mbps | Float   |
| DLPrbNum | The number of downlink resource blocks | /    | Integer |
| ULPrbNum | The number of uplink resource blocks   | /    | Integer |
| DLBLER   | Downlink block error rate              | %    | Float   |
| ULBLER   | Uplink block error rate                | %    | Float   |
| ULSINR   | Uplink SINR                            | dB   | Float   |

#### Geospatial Data


| KPI Name     | Description                             | Unit | Type   |
| ------------ | --------------------------------------- | ---- | ------ |
| Cell ID      | ID of cellular                          | /    | String |
| Average RSRP | Average of Service Cell RSRP            | dBm  | Float  |
| lon          | Longitude of the cell                   | /    | Float  |
| lat          | Latitude of the cell                    | /    | Float  |
| azimuth      | Azimuth of outdoor cell, or indoor cell | /    | String |

### CellularXsim dataset

#### Simulated Time Series Data

| KPI Name                           | Description                                                  | Unit | Type    |
| ---------------------------------- | ------------------------------------------------------------ | ---- | ------- |
| # Receiver Point (#)               | Index of sample point in the path                            | /    | Integer |
| X(m)                               | Coordinates of sampling points                               | m    | Float   |
| Y(m)                               | Coordinates of sampling points                               | m    | Float   |
| Z(m)                               | Coordinates of sampling points                               | m    | Float   |
| Distance (m)                       | The distance from the sampling point to the start of the path | m    | Float   |
| Strongest Power (dBm)              | Maximum signal power at sampling point                       | dBm  | Float   |
| Total Power With Phase (dBm)       | The total power at the sampling point                        | dBm  | Float   |
| Best SINR (dB)                     | Best SINR at sampling point                                  | dB   | Float   |
| RSSI (dBm)                         | Reference Singal Strength Indicator                          | dBm  | Float   |
| RSRP (dBm)                         | Reference Singal Receiving Power                             | dBm  | Float   |
| RSRQ (dB)                          | Reference Signal Receiving Quality                           | dB   | Float   |
| Strongest power transmitter (Tx #) | Base station index with maximum power                        | /    | Integer |

#### Collected Time Series Data 

| KPI Name  | Description                                    | Unit | Type    |
| --------- | ---------------------------------------------- | ---- | ------- |
| LATITUDE  | Longitude of the sample point                  | /    | Float   |
| LONGITUDE | Latitude of the sample point                   | /    | Float   |
| TYPE      | Type of cell                                   | /    | String  |
| TAC       | Tracking Area Code                             | /    | Integer |
| PCI       | Physical Cell Identifier                       | /    | Integer |
| ECI       | E-UTRAN Cell Identifier                        | /    | Integer |
| EARFCN    | E-UTRA Absolute Radio Frequency Channel Number | /    | Integer |
| RSSI      | Received Signal Strength Indicator             | dBm  | Float   |
| RSRP      | Reference Singal Receiving Power               | dBm  | Float   |
| RSRQ      | Reference Signal Receiving Quality             | dB   | Float   |
| SINR      | Signal to Interference plus Noise Ratio        | /    | Float   |

#### Geospatial Data

| KPI Name           | Description                                        | Unit | Type    |
| ------------------ | -------------------------------------------------- | ---- | ------- |
| cell(ECI)          | E-UTRAN Cell Identifier                            | /    | Integer |
| lat                | Longitude of the cell                              | /    | Float   |
| lon                | Latitude of the cell                               | /    | Float   |
| radius             | Positioning error radius                           | m    | Integer |
| address            | Address of cell                                    | /    | String  |
| BSIndexInSimulator | Index of base station in Wireless Insite simulator | /    | Integer |
| BSNameInSimulator  | Name of base station in Wireless Insite simulator  | /    | Integer |



## Motivations
### Purpose(s)
<!-- scope: telescope -->
<!-- info: Select **one**: -->
- Research

### Domain(s) of Application
<!-- scope: periscope -->
<!-- info: Provide a list of key domains of application that the dataset has
been designed for:<br><br>(Usage Note: Use comma-separated keywords.) -->
`AIOps`, `Prediction`, `Anomaly Detection`, `Root Cause Analysis`

### Motivating Factor(s)
<!-- scope: microscope -->
<!-- info: List the primary motivations for creating or curating this dataset:(Usage Note: use this to describe the problem space and corresponding
motivations for the dataset.) -->

- Encourages fair comparisons between methods and contributes to the development of the AIOps research community.
- Bringing User Experience to the Forefront: By focusing on user-level network experience, the CellularX dataset aims to shift the focus from base station performance to user experience. This could encourage academics and industry practitioners to consider the end-user perspective more closely in their work, leading to improvements in user experience.
- Encouraging Scenario-Diverse Model Development: By providing both real-world and simulated data, the CellularX dataset encourages researchers and practitioners to develop and test models under a wide range of network conditions. This could lead to the creation of more robust and adaptive models, contributing to the overall improvement of wireless cellular network performance.


#### Citation Guidelines
<!-- scope: microscope -->
<!-- info: Provide guidelines and steps for citing this dataset in research
and/or production. Use additional notes to capture any specific patterns that readers should look
out for, or other relevant information or considerations. -->


**BiBTeX:**
```
TODO
```

## Provenance

### Collection
#### Method(s) Used

<!-- scope: telescope -->
<!-- info: Select **all applicable** methods used to collect data: -->
- Artificially Generated
- Provided by Collaborators

#### Methodology Detail(s)

<!-- scope: periscope -->
<!-- info: Provide a description of each collection method used. Use additional notes to capture any other relevant information or
considerations. (Usage Note: Duplicate and complete the following for collection method type.) -->
**Artificially Generated:**

- **Platform:** CellularXsim includes data generated by the [Wireless Insite](https://www.remcom.com/wireless-insite-em-propagation-software/) simulation platform, which is a suite of RF propagation models, providing 3D ray-tracing, fast ray-based methods, and empirical models for the analysis of site-specific radio wave propagation and wireless communication systems. CellularXsim also contains data collected by experimenters using the Cellular-Z application in an Android smartphone.
- **Primary modality of collection data:** Time Series
- **Update Frequency for collected data:** Static



#### Collection Cadence

<!-- scope: telescope -->
<!-- info: Select **all applicable**: -->
**Static:** Data was collected once from single or multiple sources.

#### Data Processing
<!-- scope: microscope -->
<!-- info: Summarize how data from different sources or methods aggregated, processed, or connected. Use additional notes to capture any other relevant information or considerations. (Usage Note: Duplicate and complete the following for each source OR collection method.) -->

The raw data of cellularXreal contains a large number of data points filled with default values, indicating that they were not collected. To avoid ambiguity, we replaced these default values with null values.


## Extended Use

### Use in ML or AI Systems
#### Dataset Use(s)
<!-- scope: telescope -->
<!-- info: Select **all applicable** -->
- Training
- Testing
- Validation
- Fine Tuning

#### Usage Guideline(s)

When studying sim2real with the cellularXsim dataset, we have the following recommendations for the construction of training, validation, and testing sets. Recall that we manually design four paths in the study area when we constructed the data set. CellularXsim provides real-world data generated by user equipment while moving along these paths, as well as corresponding simulated data generated along the same routes. We recommend that these data can be used as training and validation sets. CellularXsim also includes a set of real-world data generated by randomly roaming within the study area. We encourage the use of this randomly sampled data as a testing set to validate the effectiveness of machine learning models, in order to avoid unfair comparisons caused by specific optimizations tailored to the given paths.