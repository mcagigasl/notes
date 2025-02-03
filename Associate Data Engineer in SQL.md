---
tags:
  - Index
---

## Courses

- [x] **Understanding Data Engineering**
  - [x] What is Data Engineering?
  - [x] Data Engineering Ecosystem
  - [x] Data Pipelines: ETL and ELT
  - [x] Data Storage and Formats

- [x] **Introduction to SQL**
  - [x] Selecting Columns
  - [x] Filtering Rows
  - [x] Aggregate Functions
  - [x] Sorting and Grouping

- [x] **Intermediate SQL**
  - [x] Subqueries
  - [x] Window Functions
  - [x] Advanced Joins
  - [x] Modifying Data

- [ ] **Joining Data in SQL**
  - [ ] Introduction to Joins
  - [ ] Inner Join
  - [ ] Outer Join
  - [ ] Cross Join and Self Join

- [ ] **Introduction to Relational Databases in SQL**
  - [ ] Database Design
  - [ ] Keys and Constraints
  - [ ] Indexes
  - [ ] Views

- [ ] **Database Design**
  - [ ] Data Modeling
  - [ ] Normalization
  - [ ] Denormalization
  - [ ] Star and Snowflake Schemas

- [ ] **Data Warehousing Concepts**
  - [ ] Introduction to Data Warehousing
  - [ ] OLAP vs OLTP
  - [ ] Data Warehouse Architecture
  - [ ] ETL Processes

- [ ] **Introduction to Snowflake**
  - [ ] Snowflake Architecture
  - [ ] Loading and Unloading Data
  - [ ] Querying Data
  - [ ] Performance Optimization

- [ ] **Understanding Data Visualization**
  - [ ] Principles of Data Visualization
  - [ ] Types of Visualizations
  - [ ] Designing Effective Visualizations
  - [ ] Tools for Data Visualization

## Projects

- [ ] **Exploring London's Travel Network**
  - [ ] Data Exploration
  - [ ] Data Cleaning
  - [ ] Analysis and Visualization
  - [ ] Reporting Findings

- [ ] **Installing PostgreSQL**
  - [ ] Introduction to PostgreSQL
  - [ ] Installation on Windows
  - [ ] Installation on Mac
  - [ ] Basic Configuration

```dataviewjs
const tasks = dv.current().file.tasks;
const completed = tasks.filter(t => t.completed).length;
const incomplete = tasks.filter(t => !t.completed).length;

const chartData = {
	type: 'pie',
	title: 'cxs',
	data: 
		{ 
		labels: ['Completed', 'Incomplete'],
	    datasets: [{ 
			data: [completed, incomplete],
            backgroundColor: [
                'rgba(118, 169, 250, 0.3)', // Cozy Muted Blue
                'rgba(255, 244, 232, 0.3)'  // Warm Muted Orange
            ],
			borderWidth: 0.5,
			title: 'xy'
		 }],

		 }, 
}
// Create a container div
const container = this.container;
container.style.display = 'flex';
container.style.justifyContent = "left";
container.style.gap = "20px";

// Create two chart containers
const chartContainer1 = document.createElement("div");
chartContainer1.style.width = "30%";
container.appendChild(chartContainer1);

const chartContainer2 = document.createElement("div");
chartContainer2.style.width = "30%";
container.appendChild(chartContainer2);

// Render charts in separate divs
window.renderChart(chartData, chartContainer1);
window.renderChart(chartData, chartContainer2);


```


