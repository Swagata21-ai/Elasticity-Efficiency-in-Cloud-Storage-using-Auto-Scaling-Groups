# Elasticity-Efficiency-in-Cloud-Storage-using-Auto-Scaling-Groups
Elasticity Efficiency in Cloud Storage using AWS Auto Scaling Groups (ASG). This project evaluates static vs dynamic cloud provisioning using AWS EC2, ASG, CloudWatch, ALB, and EBS with multi-metric auto-scaling, self-healing infrastructure, cost-aware elasticity analysis, and Elasticity Efficiency Index (EEI).


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
