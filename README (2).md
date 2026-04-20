# 🚀 Daily Job Aggregator with AI Personalization

An automated job discovery and outreach system built with **n8n** that scrapes multiple job platforms, filters high-quality opportunities, and generates **AI-personalized recruiter messages**.

---

## 🔥 Problem

Finding relevant jobs daily is:
- Time-consuming  
- Repetitive  
- Low ROI (most jobs are irrelevant)

Even worse — writing personalized messages for each job wastes hours.

---

## 💡 Solution

This workflow automates the entire pipeline:

1. Scrapes jobs from multiple platforms  
2. Cleans and normalizes the data  
3. Removes duplicates  
4. Scores jobs based on relevance  
5. Filters only high-quality opportunities  
6. Stores them in a structured database  
7. Generates **personalized cold messages using AI**

---

## ⚙️ Tech Stack

- **n8n** → Workflow automation  
- **Apify APIs** → Job scraping (LinkedIn, Indeed, Naukri)  
- **OpenAI (GPT-4o-mini)** → Message generation  
- **Data Tables** → Job storage  
- **Custom scoring logic** → Relevance filtering  

---

## 🧠 Key Features

### 📅 Automated Daily Execution
Runs every day at **10:00 AM** to fetch fresh job listings.

### 🌐 Multi-Platform Scraping
- LinkedIn  
- Indeed  
- Naukri  

### 🧹 Data Normalization
Unifies different job formats into a clean structure:
- Title  
- Company  
- Location  
- Link  
- Description  

### ❌ Duplicate Removal
Ensures no repeated job listings using unique job links.

### 🎯 Smart Job Scoring
Custom scoring system based on:
- Keywords (n8n, automation, APIs, workflows)  
- Remote availability  
- Location relevance  

Only jobs with **score ≥ 5** are kept.

### 🗂️ Data Storage
Stores filtered jobs in a structured data table for easy access.

### ✉️ AI-Powered Outreach
Automatically generates **short, human-like recruiter messages**:
- Non-generic  
- Context-aware  
- Under 80 words  

---

## 🔄 Workflow Overview

Schedule Trigger (10 AM)
        ↓
Scrape Jobs (LinkedIn, Indeed, Naukri)
        ↓
Normalize Data
        ↓
Remove Duplicates
        ↓
Score Relevance
        ↓
Filter (Score ≥ 5)
        ↓
Store in Database
        ↓
Generate AI Message

---

## 📦 Use Cases

- Job seekers who want **daily curated opportunities**
- Freelancers targeting **high-quality leads**
- Automation engineers building **lead pipelines**
- Anyone tired of manual job hunting

---

## 🚀 How to Use

1. Import the JSON workflow into n8n  
2. Add your API keys:
   - Apify  
   - OpenAI  
3. Customize keywords based on your niche  
4. Activate the workflow  

---

## ⚠️ Limitations

- Depends on external scraping APIs  
- Scoring logic is rule-based (can be improved with ML)  
- Message generation is generic unless further personalized  

---

## 🧪 Future Improvements

- AI-based job matching instead of keyword scoring  
- Resume-based personalization  
- Direct email/LinkedIn message sending  
- Dashboard UI for job tracking  

---

## 👨‍💻 Author

Built by an AI Automation Engineer focused on creating real-world systems that eliminate repetitive work and improve efficiency.
