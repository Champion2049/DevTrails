# RainShield AI: Parametric Income Protection for Delivery Riders

## 1. Problem Understanding
Delivery riders in India rely on daily earnings for financial stability. External disruptions such as heavy rainfall, flooding, and platform downtime reduce their ability to work, leading to immediate income loss. Currently, there is no system that compensates them for such short-term disruptions.

Our goal is to design a parametric insurance system that automatically detects such disruptions and compensates riders for lost income.

---

## 2. Persona & Scenarios

### Persona:
Food delivery rider working with platforms such as Swiggy or Zomato in urban areas.

### Scenario 1: Heavy Rainfall
- Rider logs in to start work
- Sudden heavy rain reduces order volume
- Rider’s earnings drop significantly

### Scenario 2: Extreme Disruption
- Continuous rainfall leads to near-zero orders
- Rider is unable to work for multiple hours

### Scenario 3: Platform Downtime (Simulated)
- Delivery app experiences outage
- Rider remains active but receives no orders

---

## 3. System Workflow

1. Rider registers and selects a weekly insurance plan  
2. System assigns a premium based on risk factors  
3. Platform continuously monitors simulated disruptions  
4. AI model estimates expected income  
5. Actual income is simulated under disruption conditions  
6. System calculates income loss  

$$
\text{Income Loss} = \text{Expected Income} - \text{Actual Income}
$$

7. If predefined thresholds are met, payout is triggered automatically  
8. Compensation is credited to the rider  

---

## 4. Weekly Premium Model

The system follows a subscription-based weekly pricing model aligned with gig worker earning cycles.

### Premium Calculation Factors:
- Zone-based risk (flood-prone vs low-risk areas)
- Historical disruption frequency
- Predicted weather patterns

### Example Logic:
- Higher rainfall probability → higher premium  
- Lower risk zone → lower premium  

### Example Plans:
| Plan     | Weekly Cost | Coverage Limit |
|----------|-------------|----------------|
| Basic    | ₹30         | ₹500           |
| Standard | ₹50         | ₹1000          |
| Premium  | ₹80         | ₹2000          |

---

## 5. Parametric Triggers

Payout is triggered automatically when:

$$
\text{Rainfall} > R_{threshold} \quad \land \quad \text{Income Loss} > L_{threshold}
$$

Key Characteristics:
- No manual claim process
- Fully automated decision-making
- Predefined transparent conditions

---

## 6. AI/ML Integration Plan

### 1. Income Prediction Model
- Type: Regression Model
- Predicts expected earnings under normal conditions
- Inputs:
  - Time of day
  - Location/zone
  - Weather conditions

---

### 2. Risk Scoring Model
- Estimates disruption likelihood
- Used for dynamic premium calculation

---

### 3. Fraud Detection (Rule-Based + ML)
- Detects anomalies such as:
  - Rider inactive during disruption
  - Mismatch between location and event
  - Repeated suspicious claims

---

## 7. Platform Choice: Web vs Mobile

We propose a **Web-based platform** for Phase 1 and Phase 2.

### Justification:
- Faster development and iteration during hackathon
- Easier to simulate dashboards and analytics
- No dependency on device-specific constraints

### Future Scope:
- Mobile application for real-world deployment

---

## 8. Tech Stack

### Frontend:
- React.js

### Backend:
- Node.js with Express

### AI/ML:
- Python (scikit-learn)

### Database:
- MongoDB / JSON-based storage

### Integrations:
- Simulated weather data
- Mock delivery activity data
- Simulated payment system

---

## 9. Development Plan

### Phase 1:
- Problem definition and system design
- Workflow and architecture planning

### Phase 2:
- Implement core features:
  - Registration
  - Premium calculation
  - Parametric trigger system

### Phase 3:
- Add advanced components:
  - Fraud detection
  - Analytics dashboard
  - Payout simulation

---

## 10. Additional Considerations

- Ensure transparency in payout logic
- Maintain fairness in premium calculation
- Design system to scale across multiple cities
- Keep user experience simple and intuitive

---

## Conclusion
RainShield AI aims to provide a scalable and automated solution for protecting gig workers from income instability using parametric insurance and AI-driven decision-making.
