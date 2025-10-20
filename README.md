Excellent — based on your Tableau workbook (`Anime Dashboard.twbx`), dataset (`Dataset Final.xlsx`), anime metadata document (`anime data terminology.docx`), and dashboard visuals you shared, here’s a complete, professional **`README.md`** file for your **Anime Dashboard Project** that you can upload directly to GitHub or your portfolio.

---

# 🎥 Anime Analytics Dashboard (Tableau)

### 📌 Project Overview

The **Anime Dashboard** is an interactive **Tableau visualization project** designed to analyze and explore global anime trends, popularity, and performance metrics.
It provides deep insights into the **ratings, genres, formats, audience engagement, and ranking** of over **20,000 anime titles**, enabling viewers and analysts to discover patterns in anime preferences, top-rated shows, and viewing behaviors across different formats (TV, Movies, OVA, ONA, etc.).

The project leverages data sourced from **MyAnimeList (MAL)** and cleaned in **Excel**, combining **data visualization** with **data storytelling** to create a dynamic experience for anime enthusiasts and data analysts alike.
<img width="1552" height="866" alt="Anime img 1" src="https://github.com/user-attachments/assets/0071c527-4e85-4054-afab-ce5e857c05ab" />

---

## 🎯 Project Objectives

* Analyze **anime performance** based on ratings, rankings, and user engagement.
* Visualize **distributions by source, type, and production studio**.
* Compare **scores versus viewer counts** to identify critically acclaimed vs popular shows.
* Enable **search and filter capabilities** for in-depth exploration of anime titles.
* Showcase **show-level details** such as producers, episode length, genres, and synopsis.

---

## 🧾 Dataset Description

The dataset used for this dashboard (`Dataset Final.xlsx`) contains detailed information about each anime’s production, airing, and audience metrics.

| **Column Name**                     | **Description**                                              |   |
| ----------------------------------- | ------------------------------------------------------------ | - |
| **anime_id**                        | Unique identifier for each anime.                            |   |
| **Name / English Name**             | Original Japanese and English-translated title.              |   |
| **Score**                           | Average viewer rating (1–10 scale).                          |   |
| **Genres**                          | Thematic categories like Action, Comedy, Fantasy, etc.       |   |
| **Synopsis**                        | Short summary of the anime’s storyline.                      |   |
| **Type**                            | Format (TV series, Movie, OVA, ONA, etc.).                   |   |
| **Episodes**                        | Total number of episodes.                                    |   |
| **Aired / Premiered**               | Airing date and season of release.                           |   |
| **Status**                          | Indicates if the anime is currently airing or finished.      |   |
| **Producers / Studios / Licensors** | Companies involved in creation and distribution.             |   |
| **Source**                          | Original medium (Manga, Game, Light Novel, Original).        |   |
| **Duration**                        | Average length per episode.                                  |   |
| **Rating**                          | Audience suitability (PG, R, R+, etc.).                      |   |
| **Rank**                            | Position relative to other anime titles.                     |   |
| **Popularity / Favorites**          | Viewer interest and fanbase engagement.                      |   |
| **Scored By / Members**             | Number of users who rated or added the anime to watch lists. |   |
| **Image URL**                       | Poster art or visual reference for the title.                |   |

---

## ⚙️ Data Preparation

Before visualization, several preprocessing steps were performed:

1. **Data Cleaning (Excel & Tableau Prep)**

   * Removed null or duplicate anime entries.
   * Standardized categorical values (e.g., “ONA”, “OAV” → “OVA”).
   * Normalized text fields (Genre, Studios, and Producers).
2. **Feature Engineering**

   * Derived key performance indicators (KPIs): `Avg Rating`, `Avg Duration`, `Avg Scored By`.
   * Grouped genres for broad-level comparison (Action, Romance, Fantasy, etc.).
3. **Integration**

   * Imported dataset into Tableau for visualization and applied **data blending** for anime-level details and aggregated summaries.

---

## 📊 Dashboard Components

### 🧩 **1. Overview Dashboard**

This high-level view summarizes the global anime dataset:

* **KPIs**:

  * *Anime Count*: 20,106
  * *Average Duration*: 24.67 min
  * *Average Rating*: 6.5
  * *Average Users Scoring Each Anime*: 36,487
* **By Source:** Highlights how many anime originated from *Manga*, *Games*, *Light Novels*, or *Original Works*.
* **By Type:** Visual breakdown by production format (TV, Movie, OVA, ONA, Special).
* **By Status:** Percentage of *Currently Airing* vs *Finished Airing* titles.
* **Score vs Scored By (Bubble Chart):** Correlation between viewer engagement and average rating.

---

### 🌟 **2. Score vs Rank Dashboard**

Focuses on the **Top Ranked Anime Titles**:

* Displays **Top N anime** ranked by score and engagement (selectable parameter).
* **KPIs:** Average duration, rating, and scoring engagement.
* **Visuals:**

  * Horizontal bar chart ranking titles like *Fullmetal Alchemist: Brotherhood*, *Hunter x Hunter (2011)*, *Steins;Gate*, etc.
  * Comparison of `Score`, `Members`, and `Favorites`.
* **Interactivity:** Filters by *Genre*, *Type*, *Producer*, and *Source*.

---

### 🎬 **3. Show-Level Dashboard**

Dedicated view providing details for a specific anime (selected via filter).

* **Title Example:** *Fullmetal Alchemist: Brotherhood*
* **Displayed Attributes:**

  * Genre: Action, Adventure, Drama, Fantasy
  * Producers: Aniplex, Square Enix, Mainichi Broadcasting System, Studio Moriken
  * Rank: 1 | Rating: 9.1/10 | Rated By: 2,020,030 users
  * Runtime: 24 minutes per episode | Total Episodes: 64
  * Suitability: R–17+ (violence & profanity)
  * Overall Attention: 31.7M | Impacted Viewers: 217K
* **Description Panel:** Summarized storyline and background of the selected show.
* **Click-through Links:** Navigation to individual anime info or back to the overall view.

---

## 💡 Key Insights

* Over **20K anime titles** analyzed, with **TV series** making up nearly **37%** of total content.
* **Average episode length** is ~25 minutes, aligning with standard TV broadcasting slots.
* **Top genres:** Action, Fantasy, Drama, and Comedy dominate the dataset.
* **Most popular sources:** *Manga* (4,038 titles) and *Original Works* (7,437 titles).
* **Fullmetal Alchemist: Brotherhood** ranks **#1** with the highest attention and engagement score.

---

## 🧠 Business & Analytical Impact

This dashboard can serve:

* **Streaming platforms:** To identify trending anime genres or top studios for licensing.
* **Production houses:** To benchmark ratings and viewer engagement.
* **Fans & Analysts:** To explore correlations between rating, popularity, and source material.
* **Market researchers:** To forecast demand for specific anime genres or formats.

---

## 🛠️ Tools & Technologies

| **Tool**                         | **Purpose**                                        |
| -------------------------------- | -------------------------------------------------- |
| **Tableau Desktop**              | Dashboard design and analytics visualization       |
| **Microsoft Excel**              | Data cleaning and preparation                      |
| **Data Blending & Filters**      | Linking detailed and aggregated datasets           |
| **Parameters & Dynamic Filters** | Interactive exploration of top N titles and genres |
| **KPIs & Charts**                | Donut, Bar, Bubble, and Scatter Plots              |

---

## 🧩 Skills Demonstrated

* Data Cleaning & Preprocessing
* Tableau Dashboard Design
* Interactive Parameter & Filter Configuration
* KPI Derivation & Visual Storytelling
* Analytical Reasoning & Genre Pattern Identification

---

## 📁 Deliverables

* **Tableau Workbook:** `Anime Dashboard.twbx`
* **Dataset:** `Dataset Final.xlsx`
* **Documentation:** `anime data terminology.docx`
* **Dashboard Previews:**
<img width="1552" height="868" alt="Anime img 2" src="https://github.com/user-attachments/assets/a1dee471-448c-45ea-ab69-82e0bd0f587a" />
<img width="1552" height="871" alt="Anime img 3" src="https://github.com/user-attachments/assets/e045081c-61ce-48c4-83a5-66de09e82c46" />


---

## 🚀 Insights Summary

The **Anime Dashboard** provides a 360° perspective on global anime trends by merging storytelling with analytics.
It allows stakeholders to:

* Discover the most **popular and highest-rated anime** across formats.
* Analyze how **source material** and **production type** affect ratings.
* Gain **data-driven insights** into viewer engagement and fandom behavior.

---

## 👨‍💻 Author

**Puneeth Vijay Krishna Samarla**
M.S. in Information Science (Machine Learning) — University of Arizona
📧 [puneethvks9@email.com](mailto:puneethvks9@email.com)
🔗 [LinkedIn](https://www.linkedin.com/in/puneeth-samarla)
