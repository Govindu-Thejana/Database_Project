# Space Launch Database Management System

A comprehensive MySQL database system designed to manage and track space launches, vehicles, payloads, and related space mission data.

## 🚀 Overview

This database system manages various aspects of space launches, including launch vehicles, payloads, spacecraft, satellites, and launch sites. It's designed to handle data from major space agencies and private space companies, with support for complex queries and performance optimization.

## 📋 Features

- Fully normalized database design (2NF compliant)
- Comprehensive tracking of space launches and related entities
- Optimized query performance with strategic indexing
- Support for multiple space agencies and launch providers
- Complex relational operations and joins
- Built-in data integrity constraints

## 🏗️ Database Schema

### Tables
1. `launchsite` - Launch location information
2. `payload` - Payload details and ownership
3. `launchvehicle` - Launch vehicle specifications 
4. `launch` - Launch event details
5. `spacecraft` - Crewed spacecraft information
6. `satellite` - Satellite specifications
7. `launchprovider` - Launch service provider details
8. `occur` - Spacecraft-launch relationship
9. `utilize` - Launch vehicle utilization
10. `images` - Launch imagery

## Entity Relationships

- Each launch is associated with one launch site, payload, and launch vehicle
- Payloads can be either spacecraft or satellites
- Launch vehicles can carry other launch vehicles (e.g., boosters)
- Multiple images can be associated with each launch

## 🛠️ Setup Instructions

1. Clone this repository
2. Install MySQL (version 8.0 or higher recommended)
3. Run the SQL scripts in the following order:

##⚡ Performance Optimization
-Indexed foreign keys for faster joins
-Optimized view definitions
-Query tuning for complex operations
-Strategic use of UNION ALL instead of UNION where appropriate

##Authors
Govindu Thejana
Sudesh Thashmika
Pasan Thilakshana

🤝 Contributing

Fork the repository
Create a new branch
Make your changes
Submit a pull request

Feel free to star ⭐ this repository if you find it useful!
