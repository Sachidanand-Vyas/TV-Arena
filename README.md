# 📺 TV Arena
### Entertainment Analytics & Audience Intelligence Platform

TV Arena is an entertainment analytics platform designed to explore audience discussions, discover trending television shows and movies, and understand public sentiment through community-driven data.

The goal is to go beyond traditional ratings and rankings by analysing what audiences are discussing, how actively they engage, and what opinions emerge across online entertainment communities.

> **Project Status:** Research & Development  
> **Reddit API Access:** Pending approval

---

## 🎯 Project Vision

Traditional entertainment platforms primarily focus on ratings, reviews, and watchlists. TV Arena aims to introduce another perspective: **audience buzz and discussion-driven popularity.**

By analysing aggregated discussions from entertainment communities, the platform aims to provide insights into:

- Which television shows and movies are trending?
- What are audiences talking about?
- Is the overall discussion sentiment positive or negative?
- Which shows are generating the most engagement?
- How does the popularity of two shows compare?

---

## ✨ Planned Features

### 1. Trending Leaderboard
Discover television shows and movies generating significant online discussions and engagement.

### 2. Buzz Score
A proposed popularity metric combining discussion volume, engagement, and activity over time.

### 3. Audience Sentiment Analysis
Analyse public discussion sentiment using an existing pretrained sentiment analysis model.

Sentiment categories:
- Positive
- Negative
- Neutral
- Mixed

### 4. Show Comparison
Compare two television shows or movies based on:
- Discussion volume
- Engagement
- Audience sentiment
- Popular discussion topics

### 5. Discussion Insights
Identify recurring themes, audience reactions, and frequently discussed topics.

### 6. AI-Powered Summaries
Generate concise summaries of aggregated audience discussions to help users understand what people are saying about a particular show.

---

## 🔍 Data Collection Strategy

Reddit is being investigated as a potential primary data source.

The proposed integration will use Reddit's official Data API, subject to approval and applicable developer policies.

### Proposed Subreddits

- r/television
- r/StrangerThings
- r/netflix
- r/TVShows
- r/movies

### Proposed Data Fields

| Data | Purpose |
|---|---|
| Post title | Discussion identification |
| Post body | Context and audience opinions |
| Subreddit | Community identification |
| Post score | Engagement measurement |
| Comment count | Discussion activity |
| Timestamp | Trend analysis |
| Comment text | Sentiment analysis |
| Comment score | Engagement analysis |

Data collection will be limited to the scope approved by Reddit.

TV Arena will operate in read-only mode and will not automate posting, commenting, voting, messaging, or moderation activities.

---

## 🏗️ Proposed Technology Stack

| Component | Technology |
|---|---|
| Frontend | React |
| Backend | Python, FastAPI |
| Database | PostgreSQL |
| Data Collection | Reddit Data API, PRAW |
| Data Processing | Python, Pandas |
| Sentiment Analysis | NLP, pretrained models |
| AI Integration | LLM-based summarization |
| Version Control | Git, GitHub |

---

## 🔄 Proposed System Architecture

```text
       Reddit Data API
              |
              v
      Python Data Collector
              |
              v
        Data Processing
              |
       +------+------+
       |             |
       v             v
  Engagement     Sentiment
  Analytics      Analysis
       |             |
       +------+------+
              |
              v
         PostgreSQL
              |
              v
       FastAPI Backend
              |
              v
        React Frontend
              |
              v
          TV ARENA
```

---

## 🔐 Data Privacy & Compliance

TV Arena is being designed with responsible data handling in mind.

- Use only API access explicitly authorized by Reddit.
- Respect Reddit's API rate limits and usage policies.
- Avoid collecting unnecessary personal information.
- Do not train AI models using Reddit content without explicit permission.
- Respect content deletion and retention requirements.
- Present aggregated insights rather than redistributing raw datasets.
- Provide links to original Reddit discussions where appropriate.

No Reddit data collection will begin until the necessary access and permissions are established.

---

## 🚧 Development Roadmap

- [x] Project concept and initial scope
- [x] Proposed technology stack
- [x] Initial data collection strategy
- [x] GitHub repository setup
- [ ] Reddit API access and policy approval
- [ ] Reddit API authentication
- [ ] Data collection proof of concept
- [ ] Data cleaning and preprocessing
- [ ] PostgreSQL database integration
- [ ] Buzz Score implementation
- [ ] Sentiment analysis pipeline
- [ ] Analytics dashboard
- [ ] Show comparison functionality
- [ ] AI-powered discussion summaries
- [ ] Deployment

---

## 🎯 Long-Term Vision

TV Arena aims to become a discussion-driven entertainment intelligence platform that helps audiences explore entertainment trends through the collective voice of online communities.

Rather than simply asking how highly a show is rated, TV Arena aims to answer a different question:

**What is everyone talking about, and why?**

---

## 📌 Project Information

- **Project:** TV Arena
- **Category:** Entertainment Analytics / Data Science / NLP
- **Development Status:** Research & Development
- **Developer:** Sachidanand Vyas

This project is currently under development. Features and integrations described above represent proposed functionality and are not yet implemented.
