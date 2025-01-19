It is a [Next.js](https://nextjs.org/) project built on React and TailwindCSS.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the code in `src`. The page auto-updates as you edit the file.

To learn more, take a look at the following resources:

- [React Documentation](https://react.dev/) - learn about React
- [TailwindCSS Documentation](https://tailwindcss.com/) - learn about TailwindCSS
- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
- # ART Finder

## Overview
**ART Finder (Automated Research and Trigger Finder)** is an innovative tool designed to streamline the research phase of ad creation by automating data gathering and analysis. It empowers marketers to craft effective, user-centric ad campaigns by providing actionable insights and recommendations derived from various data sources.

---

## Objective
The primary goal of ART Finder is to simplify and enhance ad creation by:
- Identifying user pain points and triggers from multiple platforms (Google, YouTube, Reddit, Quora, and app reviews).
- Analyzing competitor ads to uncover high-performing hooks, CTAs, and content formats.
- Generating actionable suggestions for user-centric campaigns.

---

## Key Features

### 1. Comprehensive Research Automation
- Scrapes data from blogs, forums, social media, and app reviews.
- Analyzes YouTube videos and competitor ads to identify trends, pain points, and effective solutions.

### 2. Actionable Insights Generation
- Summarizes key triggers and user problems.
- Suggests best-performing hooks, CTAs, and content formats tailored to the audience.

### 3. Reference Dashboard
- Provides direct links to scraped YouTube videos and competitor ads for easy validation.
- Visualizes insights using graphs, word clouds, and sentiment analysis.

### 4. User-Centric Interface
- Simple input fields for topics and brand guidelines.
- Intuitive dashboard showcasing insights and recommendations at a glance.

---

## Problem Solved
ART Finder addresses the following challenges:
- **Time-Consuming Research**: Automates the collection and analysis of scattered data.
- **Lack of Insights**: Derives meaningful insights from large datasets.
- **Inconsistent Campaign Performance**: Suggests data-driven hooks and CTAs.
- **Limited Scalability**: Enables agencies to manage multiple campaigns effectively.
- **Compliance Risks**: Reduces reputational risks through sentiment analysis.

---

## Practical Applications
1. **Streamlined Ad Research**: Simplifies trend analysis and identifies user pain points.
2. **Competitor Analysis**: Benchmarks successful ad strategies.
3. **Personalized Suggestions**: Generates tailored recommendations for campaigns.
4. **Data Visualization**: Presents insights in easy-to-understand formats.
5. **Agency Scalability**: Manages multiple clients with automated workflows.

---

## Installation

### Prerequisites
- Python 3.9+
- [LangFlow](https://github.com/langflow/langflow)
- Astra DB account (for database setup)

### Setup Instructions
1. **Clone the Repository**
   ```bash
   git clone https://github.com/username/ARTFinder.git
   cd ARTFinder
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Astra DB**
   - Create an Astra DB account at [Astra DB](https://www.datastax.com/astra).
   - Set up your keyspace and download the secure connect bundle.
   - Place the secure connect bundle in the project directory.

4. **Run the Application**
   ```bash
   python app.py
   ```

---

## Database Schema

### Tables
1. **scrap_data**
   - Stores raw data from scraping sources.
   - **Columns**: `data_id`, `source`, `content`, `keywords`, `sentiment`, `timestamp`

2. **competitor_ads**
   - Tracks competitor ad insights.
   - **Columns**: `ad_id`, `brand_name`, `ad_url`, `ad_hook`, `call_to_action`, `content_format`, `performance_score`, `insights`

3. **insights**
   - Stores actionable insights and suggestions.
   - **Columns**: `insight_id`, `research_id`, `competitor_ad_id`, `suggested_hook`, `suggested_cta`, `topic`, `performance_prediction`

4. **user_dashboard**
   - Stores user-specific campaign details.
   - **Columns**: `user_id`, `topic`, `brand_guidelines`, `visualized_insights`, `generated_suggestions`

5. **video_and_ad_links**
   - Links to relevant videos and competitor ads.
   - **Columns**: `link_id`, `source`, `source_url`, `title`, `description`, `related_insights`

---

## Usage
1. **Input Your Campaign Topic**: Enter your desired topic and brand guidelines.
2. **View Insights**: Explore visualized insights, competitor strategies, and suggested hooks.
3. **Validate References**: Access direct links to competitor ads and YouTube videos.
4. **Download Reports**: Export insights for further analysis or presentation.

---

## Future Enhancements
- Integration with more platforms (e.g., Twitter, Instagram).
- Advanced AI for real-time sentiment analysis.
- Mobile-friendly dashboards for on-the-go access.

---

## Contribution
Contributions are welcome! Please fork the repository and create a pull request with your changes.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For support or inquiries, contact us at **support@artfinder.com**.

