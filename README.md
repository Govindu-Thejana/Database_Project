# 🚀 Space Launch Database Management System

## 📝 Overview
A comprehensive MySQL database system designed to manage and track space launches, vehicles, payloads, and related space mission data.

## 💫 Project Description
This database system manages various aspects of space launches, including launch vehicles, payloads, spacecraft, satellites, and launch sites. It's designed to handle data from major space agencies and private space companies, with support for complex queries and performance optimization.

## ✨ Features
- **📊 Normalized Design**: Fully normalized database design (2NF compliant)
- **🛸 Complete Tracking**: Comprehensive tracking of space launches and related entities
- **⚡ Performance**: Optimized query performance with strategic indexing
- **🏢 Multi-Agency Support**: Support for multiple space agencies and launch providers
- **🔄 Complex Operations**: Advanced relational operations and joins
- **🛡️ Data Integrity**: Built-in data integrity constraints and validations

## 🎨 Design and Implementation

### 📐 Conceptual Design
- **🔄 UML & ER Diagrams**: Created using Visual Paradigm
- **📊 Entity Structure**:
  - 6+ strong entities
  - 2+ weak entities
  - Recursive relationships
  - Multivalued and composite attributes
  - Derived attributes
  - Multiple candidate keys
- **🔗 Relationship Modeling**:
  - (min, max) structural constraints
  - Defined role names
  - Complex relationship mappings

### 🛠️ Implementation Details
- **📝 Schema Development**:
  - MySQL implementation (2NF compliant)
  - Comprehensive table definitions
  - Complete CRUD operations
  - Sample data population

### 📊 Query Operations
- **🔍 Basic Queries (7)**:
  - SELECT operations
  - PROJECT operations
  - Aggregation functions
  - User-defined views
- **🎯 Advanced Queries (13)**:
  - Complex relational algebra
  - Set operations
  - Multiple table joins
  - Nested queries

### ⚡ Performance Optimization
- **📈 Query Tuning**:
  - Optimization of 10 complex queries
  - Strategic indexing implementation
  - Performance metric analysis using EXPLAIN
  - Documented efficiency improvements

## 🗄️ Database Schema

### 📌 Core Tables

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

## 🔗 Entity Relationships
- Each launch is associated with one launch site, payload, and launch vehicle
- Payloads can be either spacecraft or satellites
- Launch vehicles can carry other launch vehicles (e.g., boosters)
- Multiple images can be associated with each launch
- 
## ⚙️ Setup Instructions

### 🔧 Prerequisites
- MySQL (version 8.0 or higher)
- Git
- Command-line interface

### 📥 Installation Steps
1. Clone the repository:
```bash
git clone https://github.com/your-username/space-launch-db.git
cd space-launch-db
```

2. Install MySQL (version 8.0 or higher recommended)
3. Run the SQL scripts in the following order:

## 📊 Performance Metrics

### 🎯 Query Optimization Results
- Execution time improvements
- Resource utilization reduction
- Query plan optimizations
- Index usage statistics

Example EXPLAIN analysis:
```sql
EXPLAIN SELECT * FROM launch 
JOIN launchvehicle ON launch.vehicle_id = launchvehicle.id 
WHERE launch.date > '2023-01-01';
```

## 👥 Authors
- **Govindu Thejana** 
- **Sudesh Thashmika** 
- **Pasan Thilakshana** 
## 🤝 Contributing

### 📋 Contribution Steps
1. 🍴 Fork the repository
2. 🌿 Create a new branch (`git checkout -b feature/improvement`)
3. 💻 Make your changes
4. 📤 Push to the branch (`git push origin feature/improvement`)
5. 🔄 Submit a pull request

## ⭐ Support
Feel free to star this repository if you find it useful!
