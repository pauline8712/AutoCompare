# AutoCompare

A .NET 9 console application that evaluates whether a car is worth buying.

---

## Overview

Enter a license plate number and receive a recommendation based on mileage history, ownership count, insurance claims, and known model issues.

---

## Recommendation System

| Rating | Meaning |
|----------|----------|
| Good Buy | Low mileage, few owners, no serious flags |
| Ok Buy | Acceptable condition with some warning signs |
| Not a Good Buy | High risk — many owners, crashes, failed inspection, or known model problems |

---

## What the App Analyzes

### Mileage
- Aggregates history
- Calculates average mileage per year

### Number of Owners
- Tracks ownership changes

### Insurance Claims
- Crashes and repairs

### Inspection Records
- Passed
- Failed
- Remarks

### Known Model Issues
- Internal issue database

### AI Analysis
- GPT-4o-mini integration

---

## Tech Stack

| Component | Technology |
|------------|------------|
| Runtime | .NET 9 |
| Language | C# |
| UI | Spectre.Console |
| AI | GPT-4o-mini |
| SMS | Twilio Verify |
| Email | SMTP |

---

## Project Structure

```text
AutoCompare/
├── Program.cs
├── UIManager.cs
├── CarSearch.cs
├── Car.cs
├── User.cs
├── DataStore.cs
├── AIService.cs
├── AiHelper.cs
├── TwoFactor.cs
├── Admin.cs
├── Logger.cs
└── Config.cs
