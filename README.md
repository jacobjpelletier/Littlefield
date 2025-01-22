# Littlefield Technologies Factory Management Strategy

## Overview
This repository documents strategies, analysis, and implementation details for managing the Littlefield Technologies factory simulation. The goal is to maximize the factory's **cash balance** by optimizing **capacity, inventory, scheduling, lot sizing, and contract pricing**.

The simulation involves managing a digital satellite system (DSS) receiver assembly line over a simulated period of 316 days. The final score is based on the **cash balance** at the factory's shutdown.

## Key Objectives
- **Maximize Cash Balance**: By efficiently allocating resources and minimizing costs.
- **Optimize Lead Times**: Leverage premium pricing contracts while maintaining timely order fulfillment.
- **Adapt to Dynamic Demand**: Use historical and real-time data to predict and meet order demands.
- **Maintain Process Control**: Ensure all processes are running smoothly using Six Sigma techniques.

## Strategy Summary
### 1. **Initial Conditions**
- **Starting Resources**:
  - 3 Stuffers
  - 1 Tester
  - 1 Tuner
  - Raw Materials: 9600 kits
  - Initial Cash Balance: $10,000
- **Default Contract**:
  - Price: $750
  - Quoted Lead Time: 7 days
  - Maximum Lead Time: 14 days

### 2. **Key Decisions**
#### a. **Capacity Management**
- Monitor utilization rates at all stations.
- Purchase additional machines to prevent bottlenecks, especially at the **testing** and **tuning** stages.
- Sell surplus machines to free up cash when utilization drops.

#### b. **Inventory Management**
- Use **EOQ (Economic Order Quantity)** principles to set reorder points and batch sizes.
- Place orders proactively to avoid stockouts while minimizing holding costs.

#### c. **Lot Sizing**
- Experiment with different lot sizes to balance setup times and processing times.
- Use data from test runs to determine optimal lot sizes, minimizing idle time and maximizing throughput.

#### d. **Pricing and Contract Selection**
- Shift to premium pricing contracts as capacity allows:
  - $1000 contract: Quoted lead time of 1 day.
  - $1250 contract: Quoted lead time of 5 days.

#### e. **Process Optimization**
- Apply Six Sigma techniques:
  - **Define**: Identify bottlenecks and root causes using tools like fishbone diagrams.
  - **Measure**: Use control charts and statistical data to monitor performance.
  - **Analyze**: Evaluate workflow and test potential improvements.
  - **Improve**: Implement changes like increasing capacity or altering scheduling.
  - **Control**: Standardize successful changes to maintain process stability.

### 3. **Performance Monitoring**
- Utilize simulator tools to:
  - Monitor cash flow and overall standings.
  - Analyze machine utilization and throughput data.
  - Adjust strategies in real-time based on performance metrics.

## Tools and Techniques
- **Data Analysis**: Python scripts for data conversion and statistical analysis.
- **Visualization**: Gantt charts, swim lane diagrams, and Pareto charts for workflow clarity.
- **Process Control**: Statistical control charts to track and stabilize processes.
- **Documentation**: Comprehensive summaries and reports using SharePoint and Excel.

## Lessons Learned
- Importance of **proactive resource allocation** to prevent bottlenecks.
- Trade-offs between **setup times and lot sizes** in achieving throughput efficiency.
- Flexibility and adaptability are crucial for responding to random demand fluctuations.

## Future Work
- Explore advanced predictive analytics for demand forecasting.
- Automate data collection and analysis processes to reduce manual effort.
- Integrate AI-driven recommendations for capacity and inventory adjustments.

---

**Contributors**: This repository is managed by [Jacob Pelletier](https://github.com/jacobjpelletier)
