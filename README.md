# RiskPredict - AI-Powered Project Risk Analyzer

This is an educational project for BOUN class SWE598.

**Elevate your project management with intelligent risk prediction and proactive mitigation.**

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Target Audience](#target-audience)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Key Challenges](#key-challenges)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Overview

Project Risk Analyzer is a cutting-edge web application that empowers project managers and teams by leveraging Google Gemini AI. It provides an intuitive, data-driven platform for comprehensive risk identification, visualization, mitigation planning, and interactive analysis.

---

## Features

### Core Functionality
- **Intelligent Data Collection**: User-friendly form for project parameters (name, description, industry, budget, timeline, team size, objectives, constraints)
- **AI-Driven Risk Analysis**: Uses Google Gemini API to generate structured risk assessments with:
  - Probability (likelihood of occurrence)
  - Impact (severity if it occurs)
  - Mitigation strategies (actionable steps)
- **Interactive Risk Visualization**: Dynamic risk matrix (heatmap) with detailed tabular views
- **Strategic Mitigation Grouping**: Organizes strategies by risk severity (Critical, High, Medium, Low)
- **Conversational Risk Assistant**: AI-powered chat interface for natural language questions about project risks
- **Summary & Reporting**: Key statistics, visual summaries, and export capabilities

### Additional Features
- Mock data fallback for demonstration and offline use
- Secure API key management
- Modern, responsive UI design
- Export and sharing capabilities

---

## Target Audience

- **Project Managers**: Enhance risk management processes
- **Team Leads & Members**: Understand and mitigate project risks
- **Stakeholders & Executives**: Get clear project risk overviews
- **Consultants & Analysts**: Efficient client project risk assessments
- **Students & Educators**: Learn and apply risk analysis concepts

---

## Getting Started

### Prerequisites

- Node.js (v18 or higher recommended)
- npm or yarn
- Google Gemini API key ([Get one here](https://aistudio.google.com/app/apikey))

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd project-risk-analyzer
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure your Gemini API key:**
   
   Create a `.env.local` file in the project root:
   ```env
   GEMINI_API_KEY=YOUR_GEMINI_API_KEY
   ```
   
   *Alternative: Configure via the Settings page in the application*

4. **Run the development server:**
   ```bash
   npm run dev
   ```

5. **Open your browser:** Navigate to [http://localhost:3000](http://localhost:3000)

### Usage

1. Navigate to the Risk Analysis page
2. Fill in project details or select a sample template
3. Click "Analyze Risks"
4. Explore results across multiple tabs:
   - **Risk Matrix**: Visual risk overview
   - **Mitigations**: Detailed strategies by severity
   - **Summary**: Key statistics and export options
   - **Chat Assistant**: Ask questions about your risks

---

## Technology Stack

- **Frontend**: Next.js with React 19, Tailwind CSS
- **AI Integration**: Google Gemini API
- **Deployment**: Vercel
- **State Management**: React Hooks
- **API Security**: Environment variables and secure proxying

---

## Project Structure

```
/src
├── /app                 # Next.js App Router pages
│   ├── /api            # Backend API routes
│   ├── /risk-analysis  # Risk analysis page
│   ├── /settings       # API key configuration
│   └── page.js         # Home page
├── /components         # Reusable React components
├── /utils             # Utility functions
└── globals.css        # Global styles
```

---

## Key Challenges

1. **API Integration**: Secure communication with Google Gemini API and fallback mechanisms
2. **Deterministic AI Outputs**: Ensuring consistent risk identification for reliable analysis
3. **User Experience**: Presenting complex risk data in an easily digestible format
4. **Data Validation**: Maintaining quality of input data and AI-generated outputs

---

## Future Directions (Not planned)

- **Advanced AI**: Custom models and predictive trending
- **Collaboration**: Team workspaces and version history
- **Integrations**: Bi-directional sync with Jira, Trello, Asana
- **Enhanced Reporting**: Customizable dashboards and advanced exports
- **Mobile App**: PWA or native mobile application
