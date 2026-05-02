# EC2 Debug Lab — Case 3: Local vs External Testing

## 🎯 Objective
To determine whether a failure originates from the application layer or the network layer using curl testing.

## 🧪 Scenario
A web server is not accessible, and the goal is to identify whether the issue is internal (service) or external (network).

## ☁️ Environment
- EC2 (Ubuntu)
- nginx web server

## 🔍 Focus
- Local testing (localhost)
- Internal IP testing
- External access comparison

## 🧠 Key Idea
Comparing local and external responses helps isolate the layer where failure occurs.
