# Text Recognition using AWS Textract

## Introduction

The Text Recognition Application is a cloud-based solution that leverages AWS services to offer users the ability to extract text from images using Amazon Textract. This user-friendly application facilitates the extraction of text from various sources, including handwritten notes, scanned documents, printed text, and code snippets.

![Project Architecture](![AWS_Image](https://github.com/GIRISHARAN/TextExtraction/assets/30079876/8528dba7-8a01-47e5-96a2-f65186fd37a8)
)

## Project Links and Demo

Hosted Application: http://EC2-PublicIP:3000/

Architecture and flow


Short Demo


## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Project Goals and Objectives](#project-goals-and-objectives)
- [Target Users](#target-users)
- [Performance Targets](#performance-targets)
- [Services Used](#services-used)
- [How Cloud Mechanisms Fit Together](#how-cloud-mechanisms-fit-together)
- [Data Storage](#data-storage)
- [Programming Languages](#programming-languages)


## Project Goals and Objectives

The primary goal of this project is to create an efficient and secure application for text recognition using Amazon Textract. Key objectives include:

- Enabling users to log in securely.
- Accepting image uploads in multiple formats.
- Accurate and efficient text recognition.
- Support for various use cases and input types.
- High availability, scalability, and cost-effectiveness.

## Target Users

This application is designed for individuals and professionals who require accurate text extraction from diverse sources. Target users include students, researchers, programmers, administrators, and anyone dealing with text data from various inputs.

## Performance Targets

- **Response Time:** The application aims for fast processing with minimal response time per image.
- **Accuracy:** The text recognition engine strives for high accuracy to minimize extraction errors.
- **Versatility:** The application is designed to handle a wide range of text recognition tasks.
- **Scalability:** The system is built to efficiently scale to accommodate user demand and task complexities.

## Services Used

The following AWS services are utilized in this project:

- **Compute:** Amazon EC2, AWS Lambda
- **Storage:** Amazon S3, Amazon DynamoDB
- **Security:** AWS Secrets Manager
- **Text Recognition:** Amazon Textract
- **Network:** Amazon API Gateway

## How Cloud Mechanisms Fit Together

Amazon API Gateway serves as the entry point, routing user requests from the frontend hosted on Amazon EC2 to relevant AWS Lambda functions. These functions handle user login, image uploads, and text extraction. Amazon DynamoDB securely stores user data, while Amazon S3 stores uploaded images. The Lambda function responsible for text extraction employs Amazon Textract to process images and extract text. AWS Secrets Manager ensures secure access to DynamoDB and S3. The combination of these cloud mechanisms creates a robust and scalable system, offering users a seamless experience.

## Data Storage

- User information and login credentials are stored in Amazon DynamoDB, a secure NoSQL database.
- Uploaded images are stored in Amazon S3 Bucket, providing scalable and durable object storage.

## Programming Languages

- Python: Used for writing AWS Lambda functions.
- ReactJs: Used for frontend build single-page application development.
