# VPC Breach Simulation — Investigation

## 🔍 Step 1: Check Network Design
- Review VPC layout
- Confirm single subnet structure

## 🔍 Step 2: Check Route Tables
- Confirm all traffic routes to Internet Gateway

## 🔍 Step 3: Check Security Groups
- Identify overly permissive rules (0.0.0.0/0)

## 🔍 Step 4: Identify Root Problems
- No private subnet
- No network segmentation
- Excessive exposure at SG level

## 🧠 Findings
- Flat architecture
- No isolation boundaries
- High lateral movement risk
