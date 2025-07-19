# Canvas-Predictive-Analytics-Using-AI

# Canvas AI: Predicting Student Struggles and Delivering Personalized Recommendations

## Overview

Back when I was a university student, I relied heavily on Canvas LMS (Learning Management System), a widely used educational platform that allows students, instructors, and institutions to collaborate digitally, to manage my academic life—tracking assignments, checking grades, and staying on top of deadlines.  

But like many students, I occasionally missed deadlines—especially during finals or when juggling multiple courses. This experience sparked a deep curiosity: *Could we use data and AI to help students like me stay on track?* Especially when managing multiple courses or facing finals? Now, as a data analyst in the edtech space, I wanted to explore how platforms like Canvas could be enhanced with predictive analytics and personalized support systems. This project reflects that journey, from a student’s perspective to an analyst’s solution.


---

## Project Goal

To demonstrate how AI can improve educational outcomes by:
- Predicting which students are at risk of disengagement or failure.
- Recommending targeted, personalized interventions—before it's too late.
- Empowering both students and instructors to take meaningful action.

---

## My Approach

Behind the scenes, Canvas offers an API (Application Programming Interface) that enables developers to programmatically access platform data such as courses, grades, discussions, and student activity. However, as a student user, I discovered that API access is heavily restricted and does not allow visibility into broader student performance data.

Since I could not access real-time Canvas API data due to access restrictions and student privacy issues, I took the initiative to simulate a realistic dataset based on the structure and behavior of Canvas LMS.

### ✅ 1. **Data Simulation (`data_simulation.ipynb`)**
I created a synthetic dataset that mirrors real Canvas engagement patterns across:
- 2,000 students
- 8 courses over a 16-week semester
- Weekly metrics: logins, discussion posts, assignment scores, motivation levels, and more

This dataset includes risk labels for four key outcomes:
- Academic struggle
- Loss of motivation
- Disengagement
- Course dropout

### ✅ 2. **Model Building (`model_building.ipynb`)**
I developed two machine learning models:

#### **Predictive Model**  
A sequential LSTM-based (Long Short-Term Memory) neural network—a type of AI model that forecasts student risk **four weeks in advance**, using behavioral and academic signals. This is especially well-suited for time series data and sequential patterns. 

#### **Recommendation System**  
A system that provides **personalized feedback** to students based on their trackings of engagement and grades, instructors, and advisors, offering:
- Study strategies
- Time management prompts
- Academic support routing
- Peer learning suggestions

---

## Key Outcomes

- **Proactive Support**: Modeled interventions *before* risk peaks, rather than reacting post-failure.
- **Student-Centric**: Recommendations are contextualized to individual needs, not one-size-fits-all tips.
- **Impact-Oriented**: Targeted performance improvement and reduced dropout potential through AI-guided actions.
- **Scalable Design**: Can be adapted to real LMS APIs or institutional datasets in production environments.

---

## What This Means

This project bridges personal experience and professional ambition. I saw a problem as a student, and now I’ve built a prototype that could help solve it at scale. My goal is to contribute ideas and systems that edtech companies can adopt to create smarter, more supportive learning platforms, where no student falls through the cracks unnoticed.

---

## Repository Contents

| File | Description |
|------|-------------|
| `data_simulation.ipynb` | Code for generating a Canvas-style dataset with weekly student engagement and performance patterns |
| `model_building.ipynb` | LSTM-based prediction model + recommendation engine for at-risk students |
| `README.md` | Project overview, goals, and outcomes (this file) |

---

## What’s Next?

- Deploying the model with real-time or batch student data in a school environment
- Enhancing the recommendation engine with collaborative filtering or reinforcement learning
- Exploring real Canvas API integrations via instructor accounts or partnerships

