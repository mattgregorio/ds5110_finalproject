Fitness App Tracker

Description:

This project demonstrates the implementation of the entire backend of a fitness tracker application. Using the Faker library, artificial and random datasets were generated for various entities, totaling 10,000 records for each entity type. These entities and their relationships were constructed through foreign keys and inserted into a database from CSV files. The project includes CRUD operations to allow users and administrators to interact with the database. Additionally, various analyses were performed to extract user statistics and generate administrative reports.

Key entities include:

Users

Exercises

Workouts

Goals

Progress

Each entity type includes log reports for create, update, and delete operations. Sample alterations were tested to ensure changes were accurately reflected in the database. Statistical analyses, such as age versus weight regression and weight histograms, were conducted, and a sample administrative report was created.

Future directions include implementing cascade mechanisms for update and delete functions and constructing a frontend GUI for users.

Installation

This project was developed using Google Colab. To run the project, you'll need to import the following libraries:

import pandas as pd

from faker import Faker

import random

from enum import Enum

import sqlite3

from sqlalchemy import create_engine, Column, Integer, String, Float, Date, ForeignKey

from sqlalchemy.orm import sessionmaker, relationship

from sqlalchemy.ext.declarative import declarative_base

from datetime import date

from sklearn.linear_model import LinearRegression

from sklearn.model_selection import train_test_split

from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score

import matplotlib.pyplot as plt

Usage:

Clone the repository to your local machine.

Open the project in Google Colab.

Ensure all necessary libraries are installed.

Run the provided code cells to generate the datasets, insert them into the database, and perform the CRUD operations and analyses.

Features:

Data generation using Faker for 10,000 records per entity type.

Creation of a SQLite database with relationships and foreign keys.

Implementation of CRUD operations for database interaction.

Statistical analyses to extract user insights.

Sample administrative report generation.

Technologies Used:

Python

Pandas

Faker

SQLite

SQLAlchemy

Scikit-learn

Matplotlib

Desired Contribution:

We welcome contributions to improve the project, particularly in the following areas:

(1) Ensuring foreign key propagation.

(2) Developing a frontend GUI for users.

If you're interested in contributing, please contact us.

Contact Information:

Email: khalsa.i@northeastern.edu
Email: gregorio.m@northeastern.edu
