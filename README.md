# Reddit Data Pipeline with Airflow, Celery, PostgreSQL, S3, AWS Glue, Athena, and Redshift

This project provides a robust data pipeline for extracting, transforming, and loading (ETL) Reddit data into an Amazon Redshift data warehouse. The solution integrates various tools and services, including Apache Airflow, Celery, PostgreSQL, Amazon S3, AWS Glue, Amazon Athena, and Amazon Redshift, to handle and manage the entire data processing workflow.

## Table of Contents

- [Overview](#overview)
- [Architecture](#architecture)
- [Prerequisites](#prerequisites)
- [System Setup](#system-setup)
- [Video](#video)

## Overview

The pipeline performs the following tasks:

1. Extracts data from Reddit using its API.
2. Stores the raw data into an S3 bucket using Airflow.
3. Transforms the data using AWS Glue and Amazon Athena.
4. Loads the transformed data into Amazon Redshift for analytics and querying.

## Architecture

The data pipeline architecture is designed as follows:

1. **Reddit API**: Acts as the source of the data.
2. **Apache Airflow & Celery**: Orchestrates the ETL process and manages task distribution.
3. **PostgreSQL**: Temporary storage and metadata management.
4. **Amazon S3**: Used for raw data storage.
5. **AWS Glue**: Manages data cataloging and ETL jobs.
6. **Amazon Athena**: Handles SQL-based data transformations.
7. **Amazon Redshift**: Data warehousing and analytics.

![Architecture Diagram](images/RedditDataEngineering.png)

## Prerequisites

Before setting up the system, ensure you have the following:

- An AWS account with permissions for S3, Glue, Athena, and Redshift.
- Reddit API credentials.
- Docker installed.
- Python 3.11 or higher.

## System Setup

To set up the project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/airscholar/RedditDataEngineering.git



