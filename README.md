# RainShield AI: Parametric Income Protection for Delivery Riders

## Problem Statement
Delivery partners in India, such as food delivery riders, experience significant income loss due to uncontrollable external disruptions like heavy rainfall, flooding, and platform downtime. Currently, there is no structured mechanism to protect their daily earnings during such events.

---

## Solution Overview
RainShield AI is a simulation-based parametric insurance platform designed to automatically compensate delivery riders for income loss caused by external disruptions. The system eliminates the need for manual claims by detecting disruptions, estimating income loss using AI models, and triggering payouts automatically.

---

## Objectives
- Protect delivery riders from income loss due to external disruptions
- Enable automated and transparent insurance payouts
- Use AI-driven models for risk assessment and income prediction
- Simulate a real-world insurance workflow within a controlled environment

---

## Key Features

### Disruption Detection Engine
- Simulates environmental conditions such as rainfall intensity
- Supports multiple disruption types:
  - Heavy rainfall
  - Flood conditions
  - Platform downtime (simulated)

### AI-Based Income Estimation
- Predicts expected income per hour under normal conditions
- Compares expected income with actual simulated earnings
- Computes real-time income loss

### Parametric Insurance Automation
- Eliminates manual claim filing
- Automatically triggers payouts based on predefined conditions

### Payout System (Simulated)
- Wallet-based payout mechanism
- Instant credit simulation upon trigger activation
- Weekly payout limits enforced

### Fraud Detection System
- Validates rider activity and location (simulated)
- Detects anomalies such as:
  - Inactive riders during claims
  - Mismatch between disruption and activity
  - Duplicate claims

### Dashboard and Analytics
#### Rider Dashboard:
- Weekly insurance plan
- Earnings protected
- Wallet balance
- Active disruptions

#### Admin Dashboard:
- Risk analysis across zones
- Total payouts processed
- Fraud detection logs
- Disruption impact metrics

---

## Target Persona
Food delivery riders operating on platforms such as Swiggy and Zomato.

---

## System Workflow
1. Rider registers and selects a weekly insurance plan  
2. System calculates premium based on risk factors  
3. Platform continuously monitors simulated disruptions  
4. AI model estimates expected income  
5. Actual earnings are simulated and compared  
6. If thresholds are met, payout is triggered automatically  
7. Compensation is credited to the rider’s wallet  

---

## AI and Machine Learning Approach

### Income Prediction Model
- Model Type: Regression (Linear Regression or Random Forest)
- Input Features:
  - Time of day
  - Location or delivery zone
  - Weather conditions (rainfall intensity)
- Output:
  - Expected income per hour

### Risk Scoring Model
- Estimates likelihood of disruptions in a given zone
- Used for dynamic weekly premium calculation

### Anomaly Detection
- Identifies fraudulent or inconsistent claims
- Based on deviations from expected behavioral patterns

---

## Weekly Pricing Model
The platform follows a subscription-based weekly pricing structure aligned with gig worker earnings cycles.

| Plan     | Weekly Cost | Coverage Limit |
|----------|-------------|----------------|
| Basic    | ₹30         | ₹500           |
| Standard | ₹50         | ₹1000          |
| Premium  | ₹80         | ₹2000          |

Premiums are determined based on:
- Zone-specific risk levels
- Historical disruption patterns
- Predicted weather conditions

---

## Parametric Trigger Conditions

Payout is triggered when predefined conditions are satisfied:

IF (Rainfall > Threshold)  
AND (Income Loss > Threshold)  
THEN Trigger Payout  

---

## Simulation Design
- Weather data is generated using predefined scenarios
- Delivery earnings are dynamically simulated
- AI models operate on synthetic datasets
- Disruption events can be triggered manually for demonstration

---

## Technology Stack

### Frontend
- React.js

### Backend
- Node.js with Express

### AI/ML
- Python with scikit-learn

### Database
- MongoDB or JSON-based storage

### Integrations
- Simulated Weather API
- Mock delivery activity data
- Simulated payment gateway

---

## Development Plan

### Phase 1: Ideation and Design
- Define system architecture
- Design workflows and simulation strategy
- Outline AI models and pricing logic

### Phase 2: Core Implementation
- User registration and onboarding
- Policy creation and management
- Dynamic premium calculation
- Parametric trigger engine

### Phase 3: Advanced Features
- Fraud detection module
- Analytics dashboard
- Simulated instant payout system

---

## Demonstration Flow
1. Display rider dashboard under normal conditions  
2. Simulate heavy rainfall event  
3. Observe reduction in delivery activity  
4. AI calculates income loss  
5. Parametric trigger activates automatically  
6. Payout is credited to rider wallet  
7. Dashboard updates with protected earnings  

---

## Innovation Highlights
- Fully automated parametric insurance model
- AI-driven income prediction and risk assessment
- Zero-touch claim processing
- Real-time disruption detection and response

---

## Conclusion
RainShield AI demonstrates a scalable and efficient approach to protecting gig workers from income instability caused by external disruptions. By leveraging AI and parametric insurance principles, the platform ensures timely and transparent compensation, improving financial resilience for delivery riders.
