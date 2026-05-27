# Elasticity-Efficiency-in-Cloud-Storage-using-Auto-Scaling-Groups
Elasticity Efficiency in Cloud Storage using AWS Auto Scaling Groups (ASG). This project evaluates static vs dynamic cloud provisioning using AWS EC2, ASG, CloudWatch, ALB, and EBS with multi-metric auto-scaling, self-healing infrastructure, cost-aware elasticity analysis, and Elasticity Efficiency Index (EEI).

# Elasticity Efficiency in Cloud Storage using Auto Scaling Groups (ASG)

## 📌 Project Overview

This project focuses on evaluating **cloud elasticity efficiency** in storage-intensive environments using **AWS Auto Scaling Groups (ASGs)**. The study compares traditional static cloud provisioning with dynamic ASG-based provisioning using real AWS infrastructure and monitoring services.

The project introduces:
- Multi-metric auto-scaling
- Cost-aware elasticity analysis
- Self-healing cloud infrastructure
- Elasticity Efficiency Index (EEI)
- Comparative evaluation of static vs dynamic provisioning

The implementation is entirely AWS console-based and does not require application-level coding, making it lightweight, reproducible, and research-oriented.

---

# 🎯 Objectives

- Study limitations of traditional cloud auto-scaling approaches
- Implement multi-metric scaling using CPU and Network traffic
- Compare static provisioning with ASG-based elastic provisioning
- Evaluate elasticity efficiency using AWS services
- Demonstrate self-healing cloud infrastructure
- Analyze cost-performance trade-offs
- Propose storage-aware elasticity as future enhancement

---

# ❗ Problem Statement

Existing cloud auto-scaling techniques primarily rely on single-metric CPU-based scaling and often lack practical, cost-aware evaluation for storage-intensive workloads.

Most existing studies:
- Focus on simulations or theoretical models
- Ignore storage-access behavior
- Lack real-world AWS experimentation
- Do not quantitatively evaluate elasticity efficiency

This project addresses these gaps using infrastructure-level experimentation with AWS services.

---

# 🏗️ System Architecture

## Architecture Components

- **Amazon EC2**
  - Compute infrastructure for workload execution

- **Elastic Block Store (EBS)**
  - Persistent storage attached to EC2 instances

- **Application Load Balancer (ALB)**
  - Distributes incoming traffic

- **Auto Scaling Group (ASG)**
  - Dynamically adjusts resources based on workload

- **AWS CloudWatch**
  - Monitors CPU and Network metrics

- **Scaling Policies**
  - Trigger scale-out and scale-in actions

- **Self-Healing Layer**
  - Automatically replaces failed instances

- **Evaluation Layer**
  - Performs cost and elasticity analysis

---

# ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| Amazon EC2 | Virtual machine infrastructure |
| Auto Scaling Group (ASG) | Dynamic resource scaling |
| AWS CloudWatch | Monitoring and alarms |
| Elastic Load Balancer (ALB) | Load distribution |
| Amazon Machine Image (AMI) | Instance replication |
| Elastic Block Store (EBS) | Storage volumes |
| AWS Billing & Cost Analysis | Cost evaluation |

---

# 🧪 Methodology

## 1. Static Environment Setup
- Single EC2 instance
- Fixed infrastructure
- No elasticity support

## 2. Dynamic ASG Environment
- Multiple EC2 instances
- Auto Scaling Group enabled
- Dynamic scaling policies configured

## 3. Workload Generation
Synthetic workloads were generated using:
- CPU stress
- Network traffic simulation

This enables elasticity evaluation without application-level complexity.

## 4. Monitoring
AWS CloudWatch continuously monitored:
- CPU Utilization
- Network In Traffic

## 5. Auto-Scaling Policies

### CPU-Based Scaling
- Scale-Out: CPU > 60%
- Scale-In: CPU < 25%

### Network-Based Scaling
- Scale-Out triggered using Network In threshold

## 6. Self-Healing Demonstration
- Manual EC2 instance termination
- ASG automatically launches replacement instance

## 7. Evaluation
Comparison performed between:
- Static provisioning
- Dynamic ASG provisioning

Based on:
- Resource utilization
- Scaling behavior
- Availability
- Cost efficiency
- Elasticity Efficiency Index (EEI)

---

# 📊 Elasticity Efficiency Index (EEI)

The project proposes a lightweight empirical indicator called the **Elasticity Efficiency Index (EEI)** for comparative evaluation.

> ⚠️ EEI is used only as a comparative indicator within this study and is not claimed as a universal elasticity metric.

## EEI Parameters
- CPU Utilization
- Network Usage
- Estimated Cost

---

# ✅ Key Features

- Multi-metric auto scaling
- Real AWS implementation
- Cost-aware elasticity analysis
- Self-healing cloud infrastructure
- Dynamic resource provisioning
- Comparative performance evaluation
- Infrastructure-level experimentation

---

# 📈 Outcomes

## Static Environment
- Fixed instance count
- High CPU spikes during load
- No fault tolerance
- Resource wastage during idle periods
- Constant infrastructure cost

## ASG-Based Environment
- Dynamic instance scaling
- Improved workload distribution
- Reduced idle resource usage
- Automatic failure recovery
- Better cost-performance balance

---

# 🔄 Self-Healing Mechanism

The project demonstrates AWS ASG self-healing capability:

1. EC2 instance manually terminated
2. ASG detects unhealthy instance
3. Replacement instance launched automatically
4. Service availability maintained

---

# 💰 Cost-Aware Analysis

The project evaluates:
- Resource utilization efficiency
- Dynamic provisioning benefits
- Infrastructure cost implications

This promotes:
- Efficient cloud resource consumption
- Sustainable cloud infrastructure management

---

# 🌍 SDG Mapping

## SDG 12 — Responsible Consumption and Production

This project supports sustainable cloud computing through:
- Elastic resource allocation
- Reduced infrastructure waste
- Cost-aware cloud provisioning
- Efficient utilization of cloud resources

---

# 📚 Learning Resources

Recommended learning flow:
1. EC2 Launch & Monitoring
2. AMI Creation
3. Auto Scaling Groups
4. CloudWatch Metrics
5. Scaling Policies
6. Self-Healing Demonstration
7. Cost Analysis

---

# 🎓 Academic Contribution

This project provides an incremental research contribution by integrating:
- Multi-metric auto-scaling
- Cost-aware elasticity evaluation
- Lightweight EEI analysis
- Practical AWS experimentation

for storage-intensive cloud workloads.

---

# 👨‍💻 Author

**Swagata Sinha**  
B.Tech CSE (Cloud Technology & Virtualization)

---

# 📌 Conclusion

The project demonstrates that AWS Auto Scaling Groups significantly improve elasticity efficiency, availability, and cost-performance balance compared to static provisioning models.

The study highlights the importance of:
- Dynamic scaling
- Multi-metric monitoring
- Self-healing infrastructure
- Cost-aware resource management

for modern cloud computing environments.
