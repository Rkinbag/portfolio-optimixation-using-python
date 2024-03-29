<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://github.com/AnnaSkarpalezou/Portfolio-Optimization-using-Machine-Learning/blob/main/Pictures/unnamed.png" alt="Logo" width="150" height="100">
  </a>

  <h3 align="center">Machine Learning in Finance</h3>

  <p align="center">
    Predictive Portfolio Optimization using Machine Learning
    <br />
    <br />
  </p>
</p>







<!-- ABOUT THE PROJECT -->
## About The Project

Portfolio optimization is a process of allocating funds into financial assets with the goal of maximizing returns over risk. This repository is our attempt at utilising machine learning methods to create a sparsified and optimized portfolio that will perform well into the future. We went about doing this, by utilising 3 different techniques to forecast stock prices, namely : 

* Moving average prediction
* Multiple linear regression prediction
* Prediction using Reccurent Neural Networks, specifically Long short-term memory.

Having predicted the stock prices, we then calculate the relevant expected returns. From these we apply an optimisation technique, using a custom sharpe ratio loss function that optimises the returns over the portfolio risk, while sparcifying the output weights, expressing the tradeoff between portfolio optimality and simplicity=.

The relevant project schematic follows
![alt text](https://github.com/AnnaSkarpalezou/Portfolio-Optimization-using-Machine-Learning/blob/main/Pictures/Model%20Architecture-2.jpeg)

### Built With

This section should list all the main packages used in the project 
* pandas
* numpy
* matplotlib.pyplot 
* seaborn
* sklearn
* os
* torch
* keras
* SciPy

### Methods Used
* Principal Component Analysis
* Autoencoders
* Muliple Linear Regression
* Reccurrent Neural Networks (LSTM)
* Optimisation

### Technologies
* R 
* Python

<!-- GETTING STARTED -->
## Getting Started

The data set used in this project can be accessed and imported directly into each model, from google drive. It is available to the entirety of the NYU network, however not publicly available as the information is of sensitive. The data preprocessing for each model is done in its respective jupyter notebook. The suggested order to view the jupyter notebooks begins with moving_average+linear_regression, then PCA+LSTM and lastly Optimization. 

### Prerequisites

- [PyTorch](https://pytorch.org/) (An open source deep learning platform) 


<!-- USAGE EXAMPLES -->
## Usage

Each of the models in the models folder, can be used to predict futute stock prices. The dataset expected is a 2d dataframe, with dates as rows and different metrics for stocks in columns. The Portfolio Optimizer file, when fed predicted prices will output the weights for a portfolio of maximised returns over risk (sharpe ratio), sparcified through the l1 Lasso loss function.


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
