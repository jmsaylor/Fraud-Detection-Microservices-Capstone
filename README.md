# Overview

This project seeks to model a system of bank transactions based on this [data](https://www.kaggle.com/ntnu-testimon/paysim1) in order to detect fraudulent transactions. And, it's being done within a microservices architecture to provide for scalability and modularity. 

The pub/sub design pattern is implemented for simulating the high volumes of bank transaction data, and the MVC pattern is used to provide user access to the processed data.

![Diagram of Microservices](https://imgur.com/9Q0kurz.jpg)

# Transaction Simulation

Using the messaging service Kafka, transactions can be simulated.

https://github.com/jmsaylor/Transaction-Producer

# Fraud Detection

Observations in the data
https://github.com/jmsaylor/ML-Tutorials/blob/master/fraud-training/main.py

Isolating all frauds  together, the majority of frauds consists of this pattern.

TRANSFER -> CASH_OUT with the same amount

![sample frauds showing transfer cash-out scheme](https://imgur.com/7RWAMVU.jpg)

These are the rest of the frauds that need a method for detection.

![sample frauds](https://imgur.com/KYOguJ8.jpg)

## Gateway

https://github.com/jmsaylor/gateway


## Auth Server

https://github.com/jmsaylor/first-auth-server

## Data Upload (Multithreaded)

https://github.com/jmsaylor/MultithreadingTest
