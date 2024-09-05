
# TemporalGraphPrediction-Indego

This project aims to study Philadelphia's Indego Bike-sharing system and leverage analytics to perform future link prediction task

## Introduction
Bike-sharing systems like Philadelphia's Indego Bike offer sustainable transportation, reducing traffic congestion and emissions. Launched in April 2015 with 72 stations, Indego has grown to over 165 stations and 1,500 bikes, including electric models introduced in 2019. The City of Philadelphia and Bicycle Transit Systems provide anonymized trip data, which is ideal for predictive analytics.

This study leverages the Indego Bike dataset to address temporal graph predictions, crucial for understanding bike-sharing dynamics, such as predicting bike availability, optimizing station placements, and anticipating maintenance needs. By modeling the dataset as a dynamic graph with bike stations as nodes and trips as edges, we employ Continuous Time Dynamic Node Embeddings (CTDNE) to capture temporal behaviors and predict future interactions. These predictive models aim to enhance operational efficiency and service reliability, benefiting commuters and contributing to urban planning and smart city initiatives through advanced temporal graph analysis.
## Problem Statement
Adopting a novel approach, the bike sharing dataset is modelled as temporal graphs, where bike stations serve as nodes and trips as edges. This study delves into the dynamic landscape by using the openly available 2023 Indego dataset. The primary objective revolves around forecasting future links within this network, treating link prediction as a binary classification problem and using **Continuous Time Dynamic Node Embeddings (CTDNE)** to generate node embeddings. Various time resolutions, spanning from seconds to weeks, are utilized to capture the temporal dynamics of interactions. Leveraging a suite of classification algorithms including logistic regression and decision trees, predictive models are constructed and evaluated.
## Project Flow
1. **Data Preprocessing**
   - Handling Missing data
   - Removing irrelevant features
2. **Proposed Approach**
    - Dynamic Graph Creation
    - Splitting the edges
    - Node Embedding Creation using Continuous-Time Dynamic Network Embeddings (CTDNE)
        - Random Walk Generation
        - Embedding Creation
    - Positive & Negative Edges
    - Link Prediction 

 
## Code Details
- Code 1 : **Code A.ipynb** is a consolidated script that contains some basic Exploratory Data Analysis (EDA) on both the datasets, trip and station. It also contains codes for performance of link prediction tasks across various time resolutions (Seconds, Hourly, Daily, Weekly), comparing temporal and static walks.
- Code 2 : **Code B.ipynb** is the script that include code for the models used for this classification task: Logistic Regression, Support Vector Machines (SVM), Decision Tree and Feed Forward Neural Network. It also includes code for the accuracy comparison of varying percentages of edges included in node embedding creation.
## Acknowledgements

 - [Indego Trip Data](https://www.rideindego.com/about/data/)
 - [Continuous-Time Dynamic Network Embeddings](http://ryanrossi.com/pubs/nguyen-et-al-WWW18-BigNet.pdf)
 - [Link prediction with Continuous-Time Dynamic Network Embeddings (CTDNE)](https://stellargraph.readthedocs.io/en/stable/demos/link-prediction/ctdne-link-prediction.html#Link-prediction-with-Continuous-Time-Dynamic-Network-Embeddings-(CTDNE))


## Contributing
Contributions are welcome! If you have a bug fix, improvement, or a new feature to add, please follow these steps:
- Fork the repository
- Create a new branch
- Make your changes and commit them
- Push to the branch
- Open a Pull Request


## Contact
If you have any questions or suggestions, feel free to reach out to me:
- Email: hardik.sharma@temple.edu
- GitHub: hrdikshrma

Thank you for visiting TemporalGraphPrediction-Indego ! Happy coding!