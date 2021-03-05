# Overview

This project seeks to model a system of bank transactions based on this [data](https://www.kaggle.com/ntnu-testimon/paysim1) in order to detect fraudulent transactions. And, it's being done within a microservices architecture to provide for scalability and modularity. 

The pub/sub design pattern is implemented for simulating the high volumes of bank transaction data, and the MVC pattern is used to provide user access to the processed data.

# Transaction Simulation

Using the messaging service Kafka, transactions can be simulated.

https://github.com/jmsaylor/Transaction-Producer

# Fraud Detection

Observations in the data
https://github.com/jmsaylor/ML-Tutorials/blob/master/fraud-training/main.py

![sample frauds](https://imgur.com/KYOguJ8.jpg)
![sample frauds showing transfer cash-out scheme](https://imgur.com/7RWAMVU.jpg)

Most fraud in this dataset consists of a TRANSFER -> CASH_OUT scheme.  

https://github.com/jmsaylor/Fraud-Detection/tree/master/src/main


# Gateway

https://github.com/jmsaylor/gateway


# Auth Server

https://github.com/jmsaylor/first-auth-server

# Data Upload (Multithreaded)

https://github.com/jmsaylor/MultithreadingTest
