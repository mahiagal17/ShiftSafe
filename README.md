## ShiftSafe
**AI-Powered Parametric Income Protection for India's Gig Delivery Workers**

------------------------------------------------------------------------------------------------------------------------------------------------------------
## Table of Contents
- The Problem
- Our Solution
- Key Innovation
- System Workflow
- Insurance Plans
- AI Integration
- API Integration
- Tech Stack
- Key Features
- User Journey
- Impact
- Conclusion

------------------------------------------------------------------------------------------------------------------------------------------------------------

## The Problem
India's food delivery system depends on a huge number of gig workers who deliver orders daily through platforms like Zomato and Swiggy. Most of these workers earn on a daily or weekly basis, so their income directly depends on how many deliveries that can complete.
The problem is that they do not have any proper financial backup when something unexpected occurs.Even small disruptions can affect their earnings badly.

**When disruptions occur** -
- Rain / Floods              ->        Deliveries stop, income lost
- Extreme Heat               ->        Forced to stop mid-shift
- High Pollution             ->        Fewer orders, limited areas
- Curfews / Strikes          ->        Movement restricted

## Reality

Daily Earnings           -> ₹600 - ₹1200
Loss per disruption      -> ₹500 - ₹900

As a result, workers bear 100% of the loss.

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Our Solution

ShiftSafe is a smart AI-powered platform that protects the income of gig delivery workers in India(Zomato & Swiggy)
It predicts risks like *rain, heat , pollution , or disruptions* and automatically activates weekly insurance - ensuring workers never lose income.

| Traditional Insurance       | ShiftSafe                     |
|-----------------------------|-------------------------------|
| Disruption happens          | Risk predicted Sunday night   |
| Worker files claim          | Protection auto-activated     |
| Insurer reviews claim       | Disruption detected live      |
| Worker waits 3–7 days       | Payout triggered instantly    |
| Maybe gets paid             | Worker paid same day          |

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Key Innovation: Hyperlocal Disruption Intelligence

SmartShield introduces a **Hyperlocal Disruption Score (HDS)** that measures the likelihood of income disruption in a specific delivery zone.

The score is calculated using multiple signals:

### Environmental Signals
-   Rainfall intensity
-   Temperature extremes
-   Pollution levels (AQI)

### Social Signals
-   Curfew announcements
-   Strike alerts
-   Zone or market closures

The **HDS determines:**
-   Weekly insurance premium
-   Risk category of delivery zones
-   Automated claim triggers

This allows the system to provide **data‑driven and location‑specific insurance protection**

------------------------------------------------------------------------------------------------------------------------------------------------------------

## System Workflow

1.  Worker registers on the ShiftSafe platform.
2.  The system identifies the worker's delivery zone.
3.  AI calculates the **Hyperlocal Disruption Score**.
4.  The system generates a **dynamic weekly premium**.
5.  Worker activates weekly insurance coverage.
6.  Platform continuously monitors environmental and social data using
    APIs.
7.  When disruption thresholds are exceeded, the system automatically
    triggers a claim.
8.  Fraud detection verifies worker eligibility.
9.  Worker receives **instant simulated payout for lost income**.

Worker Registers
      ↓
Location Detected
      ↓
API Data Collected
      ↓
Risk Score Calculated
      ↓
Disruption Detected
      ↓
Claim Triggered
      ↓
Compensation Payout

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Weekly Insurance plans

| Plan        | Price | Max Payout |
| ----------- | ----- | ---------- |
|  Lite       | ₹25   | ₹400       |
|  Standard   | ₹55   | ₹1000      |
|  Pro        | ₹95   | ₹1800      |


Premium calculation -

Weekly Premium = Base Price × Zone Risk Factor

Zone Risk -
If disruptions are very low (below 10%) ->  × 0.90
If disruptions are moderate (10–25%) ->  × 1.00
If disruptions are high (above 25%) ->   × 1.15

Payout Formula:
Payout = Verified Disruption Hours × Worker Hourly Average Earnings 
Worker Hourly Average = Last 4-week average daily earnings ÷ Average active hours per day

------------------------------------------------------------------------------------------------------------------------------------------------------------

## AI / Machine Learning Integration
Artificial Intelligence powers multiple components of the platform.

1. Risk Prediction Model

Predicts disruption probability using environmental and historical data.

Output: **Hyperlocal Disruption Score**

2. Dynamic Premium Calculation

Machine learning models adjust weekly insurance premiums based on
disruption risk.

3. Fraud Detection Engine

AI detects suspicious claims using:

-   Location validation
-   Delivery activity patterns
-   Duplicate claim detection

------------------------------------------------------------------------------------------------------------------------------------------------------------

## API Integrations

ShiftSafe integrates multiple external data sources.

Weather API - 
Used to detect rainfall, temperature, and storm alerts.

Air Quality API - 
Used to monitor pollution levels and hazardous AQI conditions.

Maps or Location API - 
Used for delivery zone detection and traffic monitoring.

These APIs provide real-time external data to the system, which is used to detect disruptions.

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Technology Stack

Frontend :
- React.js –> used to build the user interface
- Tailwind CSS –> for styling and responsive design
- React Router –> for navigation between pages
- Recharts –> for showing charts and analytics
- Axios –> for handling API requests

Backend & Infrastructure :
- Firebase Firestore –> database to store user and claim data
- Firebase Authentication –> login using phone OTP
- Firebase Cloud Functions –> used for background tasks like risk calculation
- Firebase Hosting / Vercel –> for deploying the application

External APIs :
- OpenWeatherMap –> to get weather forecast data
- AQICN –> to get air quality data
- Google Maps API -> to get the location 
- Razorpay (Test Mode) –> to simulate UPI payments

AI / ML:
- JavaScript Rule Engine –> used for basic risk calculation 
- Python + scikit-learn –> planned for advanced predictions
- Isolation Forest –> planned for fraud detection

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Key Features 

- Weekly Risk Prediction –> System analyzes weather and pollution data to estimate risk for the upcoming week.

- Easy Plan Activation –> Workers can quickly choose and activate a plan.

- Live Monitoring –> Conditions are tracked continuously to detect disruptions.

- Auto Claim Processing –> Claims are handled automatically without any manual steps.

- Quick Payouts –> Earnings are credited instantly (simulated) after disruptions.

- Fraud Checks –> Basic validation to prevent misuse of claims.

- Weekly Summary –> Simple report showing earnings and protected income

------------------------------------------------------------------------------------------------------------------------------------------------------------

## User Journey

STEP 1 ── REGISTRATION

│ Open ShiftSafe → Enter mobile number                     │
│ → OTP verification (Firebase Auth)                       │
│ → Select delivery zone (city + area)                     │
│ → Enter average daily earnings                           │
│ → Link UPI ID for payments                               │
│ → Profile created                                        │
                          │
                          ▼
STEP 2 ── FIRST SUNDAY NIGHT
┌──────────────────────────────────────────────────────────┐
│ AI runs weekly forecast for the selected zone            │
│ → Risk Score: 72 / 100 (High)                            │
│ → Pro Shield recommended (₹95/week · max ₹1,800)         │
│ → Worker receives notification                           │
│ → Activates plan with one tap                            │
│ → Premium deducted at midnight                           │
│ → Coverage starts from Monday                            │
└──────────────────────────────────────────────────────────┘
                          │
                          ▼
STEP 3 ── DURING THE WEEK
┌──────────────────────────────────────────────────────────┐
│ Worker checks Live Protection Meter                      │
│ → Heavy rain detected in the area                        │
│ → Risk crosses threshold → Coverage activates            │
│ → Dashboard shows active protection                      │
│ → 4 hours of disruption recorded                         │
│ → Payout calculated automatically                        │
│ → Amount credited to UPI                                 │
└──────────────────────────────────────────────────────────┘
                          │
                          ▼
STEP 4 ── SUNDAY SUMMARY
┌──────────────────────────────────────────────────────────┐
│ Worker views Weekly Earnings Summary                     │
│ → Total hours worked and disrupted                       │
│ → Earnings protected and payout received                 │
│ → Insurance streak updated                               │
│ → Next week forecast and recommendation shown            │
└──────────────────────────────────────────────────────────┘

------------------------------------------------------------------------------------------------------------------------------------------------------------

## What Makes SmartShield Different

SmartShield uses a parametric insurance model where claims are triggered automatically based on real-time data, instead of manual requests.

Key highlights:
- Hyperlocal disruption detection
- Automatic claim processing
- No paperwork involved
- Faster payouts for workers

This makes the system simple, fast, and more accessible for gig workers.

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Impact

ShiftSafe aims to support millions of delivery workers in India who depend on daily earnings. Many of them face income loss due to factors like weather, pollution, or local restrictions.
Even small disruptions can reduce their weekly income, and currently very few workers currently have any form of protection. This solution helps provide a safety net and more financial stability.

With this approach, ShiftSafe can:
- Reduce income loss during disruptions
- Provide faster and automated payouts
- Improve financial security for gig workers

------------------------------------------------------------------------------------------------------------------------------------------------------------

## Conclusion

ShiftSafe is a simple step towards protecting gig workers from unexpected income loss. By using real-time data and automation, it makes insurance faster, easier, and more accessible.







