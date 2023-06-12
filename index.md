# CellularX: A Spatial-Temporal Dataset for User-Centric Sim2Real Learning in Telco Network
We introduce cellularX, the first spatial-temporal dataset focusing on user-level network experiences within telco networks. As opposed to most existing datasets that only offer cell-level Key Performance Indicators (KPIs), cellularX fills the gap by offering user-grained multi-dimensional KPI data. In particular, cellularX provides a synthetic dataset for simulation-to-reality (sim2real) research to address the challenge of scarcity of real-world data for specific scenarios. Additionally, a real-world dataset collected from almost one thousand users is open-sourced. Both datasets are capable of assisting user-level network experience modeling and monitoring, e.g., anomaly detection, anomaly prediction, and root cause analysis. 

The potential applications of cellularX include

**1) Sim2real study**: cellularX provides a controlled, flexible simulation platform and a set of real-world and simulated data that can be used to generate low-cost training data, while helping to understand the reality gap in sim2real learning and facilitate a fair comparison of sim2real algorithm.
**2) AIOps for telco network**: CellularX provides real-world KPI data, viewed as a snapshot of user access and network experience. Its unique multi-dimensional indicators enhance the suitability for supporting various AIOps tasks, including root cause analysis and anomaly prediction.

#### Data Composition

<!-- info: Provide a link to the dataset: -->
<!-- width: half -->

We propose **CellularX**, a large dataset focusing on user-level network e**X**perience in **cellular** networks. It provides two sub-datasets, cellularXsim and cellularXreal, enabling a comprehensive view of the user-level network experience.

- **CellularXsim** offers a controlled environment for simulating different scenarios and investigating their impacts on user-level network experience. It includes user-level KPIs gathered from a real-world study area and data generated in a corresponding simulation environment. 

<div align="center">
<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/map_sim2real.png" alt="map_sim2real" style="zoom: 33%;" />
</div>


- **CellularXreal** is collected by a top operator and records real-time multidimensional KPIs representing network experience over 982 anonymous users, providing an insightful snapshot of real-world user interactions and network experiences. This significantly contributes to understanding how users engage with the network in their daily lives.

<div align="center">
  <img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/map_real.png" alt="map_real" style="zoom:50%;" />
</div>


By integrating these two aspects, cellularX provides a richer understanding of the user-level network experience in wireless cellular networks. To the best of our knowledge, cellularX is the first dataset that focuses on user-level network experience.

#### Dataset Link

- CellularXsim:
    - The dataset can simulator configurations can be found at [this link](https://github.com/cellularXdataset/cellularXdataset.github.io/tree/main/cellularXsim).
    - We also provide the Wireless Insite [project file](https://github.com/cellularXdataset/cellularXdataset.github.io/tree/main/wireless_insite_project), which is the simulation platform used in this dataset. 

- CellularXreal: Will be uploaded soon.

#### License

This dataset is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/80x15.png" /></a> <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) License </a>. This means that you are free to use, copy, modify, and distribute the dataset for *non-commercial purposes* as long as you provide attribution to the original author. The license restricts the use of the dataset for any commercial purposes without obtaining prior permission from the author. Please note that this license ensures the dataset's availability for academic and non-profit research, but prohibits its usage for commercial gain.

**Author statement**: we bear all responsibility in case of violation of rights, etc., and confirmation of the data license.



#### Citation Guidelines

<!-- scope: microscope -->
<!-- info: Provide guidelines and steps for citing this dataset in research
and/or production. Use additional notes to capture any specific patterns that readers should look
out for, or other relevant information or considerations. -->


**BiBTeX:**

```
TODO
```



## Authorship

### Dataset Owners
#### Team(s)

<!-- scope: telescope -->
<!-- info: Provide the names of the groups or team(s) that own the dataset: -->

[anonymous]

<!--DNA Lab. Tongji University, Shanghai, China.-->

#### Author(s)

<!-- scope: microscope -->
<!-- info: Provide the details of all authors associated with the dataset: (Usage Note: Provide the affiliation and year if different from publishing
institutions or multiple affiliations.) -->

[anonymous]

<!--Shaoyu Dou, Ph.D. Student, Tongji University-->

<!--Kai Yang, Professor, Tongji University-->

<!--**Note:** We thank Xiangmin Zou, a PhD student at Tongji University, for his contribution to the simulation data in the cellularXsim dataset and to the writing of the paper.-->

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
| Number of Instances | x, ~18,000                  |

**Above:** Summary of CellularX dataset



#### Content Description

<!-- scope: microscope -->
<!-- info: Provide a short description of the content in a data point: -->
- **CellularXreal** dataset consists of two parts: multidimensional KPI data and cellular information, where each record corresponds to a _timestamp_ and a _sampling cell_. The data contains a significant number of missing values since not all indicators are reported for each access.
The published KPI data encompasses 982 users and consists of _eight dimensions_ of KPIs. These KPIs include uplink and downlink user experience rate, block error rate, the number of resource blocks, as well as RSRP of the service cell and uplink SINR. 

- **CellularXsim** provides **real-world KPI** data generated by user equipment while moving along four manually designed paths, as well as corresponding **simulated data** generated with six simulator configurations along the same routes. CellularXsim also includes a set of real-world data generated by randomly roaming within the study area. **Simulator configuations** and **cell infomation** are provided. Four KPI metrics are recorded, that are RSSI, SINR, RSRP, and RSRQ.


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

All user devices involved in the data set have been anonymized, and the data set only collected data from cells in a part of the city block, so any user's behavior and identity cannot be inferred using any additional methods.


### Dataset Version and Maintenance
#### Maintenance Status

<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Limited Maintenance: **  The data will not be updated, but any technical issues will be addressed.

#### Version Details

<!-- scope: periscope -->
<!-- info: Provide details about **this** version of the dataset: -->
Current Version: 1.0

Last Updated: 06/2023

Release Date: N/A

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
it typical. **Use additional notes to capture any other relevant information or
considerations.** -->

**Below are examples of kind data in the cellularXreal dataset.**

- Time series data in cellularXreal dataset, containing missing values.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/20230612142141.png" alt="Time series data in cellularXreal dataset"  />

- Geospatial data in cellularXreal dataset

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531162027544.png" alt="image-20230531162027544" style="zoom:50%;" />

**Below are examples of kind data in the cellularXsim dataset.**

- Simulated time series data in cellularXsim dataset.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531162310523.png" alt="image-20230531162310523"  />

- Collected time series data in cellularXsim dataset.

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/16681685521414_.pic.jpg" alt="16681685521414_.pic"  />

- Geospatial data in cellularXsim dataset

<img src="https://raw.githubusercontent.com/KMdsy/figurebed/master/img/image-20230531191915972.png" alt="image-20230531191915972" style="zoom:50%;" />



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
| CellID       | ID of cellular                          | /    | String |
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


## Limitations and Societal Impact

### Societal Impact

#### Positive Impact

- **Enhancing Efficiency in Network Optimization and Maintenance:** Researchers and operators can better understand user-level network experiences through this dataset. For instance, they can analyze factors that may impact the quality of user experience, such as network latency and packet loss rate. In this way, they can perform network optimization and maintenance targeted at specific indicators or groups of indicators, thereby improving the overall user network experience.
- **Providing Low-Cost Training Data:** CellularXsim offers a controlled and flexible simulation platform, as well as a set of real-world and corresponding simulated data. This data can be used to generate low-cost training data, which is extremely valuable for researchers in machine learning and artificial intelligence. They can use this data to train and test their models.
- **Enhancing Transparency and Replicability in Public Data Science Research:** CellularX is open-sourced, meaning that anyone can use and analyze this dataset for non-commercial purposes. Other researchers can validate and replicate studies conducted using this dataset, thus enhancing the transparency and replicability of public data science research.

#### Negative Impact

- **Privacy:** Although the user data in the CellularX dataset has been anonymized, it does not mean that it cannot be reverse-engineered. We have taken effort to protect users' privacy, but if malicious third parties with sufficient technology and resources gain access to this data, they may be able to re-identify some users. This could expose users' network usage habits and behavior patterns, thus invading their privacy.
- **Fairness:** The cellularX dataset primarily focuses on user-level network experiences, which could lead to the overemphasis of certain users or groups' network experiences and the neglect of others. For instance, if the dataset mainly includes data from urban areas, the needs and experiences of users in suburban areas may be overlooked in the process of using this dataset to develop or improve network services.
- **Potential malicious use:** The cellularX dataset can be used to simulate and predict user behavior under specific network conditions. This information could potentially be used for malicious purposes, such as network surveillance or targeted network attacks on specific users or groups.
- **Environmental impact:** Although the cellularX dataset itself may not directly cause significant environmental impact, the computational resources required to process and analyze this dataset could generate some carbon emissions. This is a common issue in the field of AI and ML, as training and running complex models often require a large amount of electricity.


### Limitations

- **Data coverage limitations:** If the CellularX dataset is primarily collected from a specific geographic region or type of network, the findings may not generalize well to other regions or networks. This could be a limitation if you're trying to use the dataset for a broader analysis of network behavior.
- **Research limitations:** As mentioned in the dataset description, the CellularXreal dataset contains a significant number of missing values since not all indicators are reported for each access. This could limit the types of research that can be performed with the dataset.
- **Temporal dynamics:** If the data was collected over a specific period of time, it might not capture the changes in user behavior and network performance over different periods of time, such as different times of day, week, or year.
- **Interpretability limitations:** Multi-dimensional KPI data could be complex to interpret and model, making it difficult to derive meaningful insights without substantial domain knowledge.
- **Generalizability limitations:** The experiments in this paper are limited to anomaly prediction as the AIOps task, verified across multiple indicators of a single user. Although we believe that the data characteristics analyzed in the text, as well as the proposed method, have universality in spatial-temporal data within telco networks or RANs, we cannot guarantee that the results can be broadly generalized to other regions or types of networks.
