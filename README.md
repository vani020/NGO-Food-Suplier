# NGO-Food-Suplier
FoodBridge is an intelligent NGO food supply system designed to reduce food wastage by connecting donors and NGOs. The platform uses priority calculation and Greedy Algorithms to allocate available food efficiently, ensuring fair distribution and maximizing social impact through technology.
# FoodBridge – Intelligent Food Distribution System for NGOs

## Introduction

Food wastage is one of the most significant challenges faced by society today. Every day, large quantities of edible food are discarded by hostels, restaurants, mess facilities, event organizers, and households. At the same time, many NGOs and charitable organizations struggle to provide adequate meals to underprivileged communities due to limited resources and irregular donations.

FoodBridge was developed as a technology-driven solution to address this gap. The platform creates a digital ecosystem where food suppliers can easily donate surplus food and NGOs can receive food based on their needs and priority. By automating the allocation process, the system ensures that available resources are utilized efficiently and reach the organizations that can create the maximum social impact.

The project combines web technologies with algorithmic decision-making to build a transparent, scalable, and efficient food distribution network.

## Problem Statement

Traditional food donation systems often face several challenges:

- Lack of communication between food donors and NGOs
- Manual allocation of food resources
- Unequal distribution of available food
- Difficulty in identifying the most deserving NGO
- Absence of centralized tracking and monitoring
- Significant food wastage due to delayed distribution

These challenges result in inefficient utilization of donated food and reduced social impact.

FoodBridge aims to solve these issues through a centralized platform that intelligently manages donations and food allocation.

## Project Objective

The primary objective of FoodBridge is to reduce food wastage and improve food accessibility for NGOs by providing an automated and data-driven food distribution system.

The project focuses on:

- Connecting food suppliers with NGOs
- Creating transparency in food distribution
- Prioritizing NGOs based on actual requirements
- Reducing manual intervention in allocation decisions
- Ensuring fair and efficient distribution of resources
- Demonstrating the practical implementation of Data Structures and Algorithms in a real-world social problem

## System Overview

FoodBridge consists of three major stakeholders:

### Food Suppliers

Food suppliers such as hostels, restaurants, canteens, and event organizers can register available food details on the platform. Information such as food quantity, availability, and expiry time can be submitted through the system.

### NGOs

NGOs can register themselves and provide details regarding:

- Number of beneficiaries
- Current food requirements
- Urgency level
- Available resources

This information is used to calculate priority scores.

### Administrator

The administrator oversees the entire system and manages:

- NGO records
- Food inventory
- Donation history
- Allocation reports
- Platform analytics

## Working of the System

The workflow of FoodBridge follows a structured process.

First, food suppliers enter information about available food donations. Once the food is added to the system, NGO data is analyzed to determine which organizations require immediate assistance.

A priority score is calculated for each NGO based on multiple factors such as beneficiary count, urgency level, and food demand. After ranking NGOs according to their priority scores, the system applies a Greedy Allocation Algorithm to distribute food resources.

The algorithm starts allocating food to the highest-priority NGO and continues until the available stock is exhausted. This approach ensures that limited resources create the maximum possible benefit.

All allocations are recorded and can be viewed through the administrative dashboard.

## Algorithmic Approach

One of the major highlights of this project is the integration of Data Structures and Algorithms.

### Priority Calculation

Each NGO receives a dynamic priority score.

Factors considered include:

- Number of beneficiaries
- Urgency of food requirement
- Food shortage level
- Previous allocations

The higher the score, the greater the priority assigned to the NGO.

### Sorting Mechanism

After calculating priorities, NGOs are sorted in descending order based on their scores.

### Greedy Allocation Algorithm

The Greedy Algorithm allocates available food to the NGO with the highest priority first and continues until all resources are distributed or exhausted.

## Technical Implementation

The backend of FoodBridge is developed using C++, which handles data processing, priority calculations, sorting operations, and food allocation logic.

The frontend is developed using HTML, CSS, and JavaScript to provide a user-friendly interface for interacting with the platform.

Communication between the frontend and backend is achieved through REST APIs. The cpp-httplib library is used to create lightweight HTTP endpoints that enable seamless data exchange.

## Key Features

- NGO registration and management
- Food donation management
- Real-time food stock monitoring
- Priority-based NGO ranking
- Automated food allocation
- Donation tracking and history
- Dashboard analytics and reporting
- REST API integration
- Scalable and modular architecture

## Social Impact

The project is designed to create measurable social impact by reducing food wastage and improving access to food for vulnerable communities.

Benefits include:

- Better utilization of surplus food
- Faster distribution of donations
- Increased transparency in allocation decisions
- Improved support for NGOs
- Greater community participation in food donation programs

## Challenges Addressed

- Fair resource distribution
- NGO prioritization
- Handling limited food inventory
- Reducing allocation bias
- Maintaining transparency
- Designing a scalable architecture

## Future Scope

Future enhancements may include:

- MySQL or MongoDB integration
- AI-based demand forecasting
- Real-time notifications
- Geo-location based NGO matching
- Delivery route optimization
- Mobile application development
- Cloud deployment
- Analytics powered by Machine Learning

## Conclusion

FoodBridge demonstrates how technology, algorithms, and software engineering can be combined to solve a meaningful social problem. The project not only reduces food wastage but also ensures that available resources reach the organizations that need them the most.

## Developed By

**Vani Tyagi**  
*B.Tech (AI & ML)*
