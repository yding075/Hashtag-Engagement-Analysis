# Hashtag-Engagement-Analysis
Analyzing the Relationship Between Keyword Popularity and Video Engagement on Video Platforms.

# Research Question
Does keyword popularity influence video engagement?

# Project Description
This project analyzes the relationship between keyword popularity and video engagement on video platforms.
The goal is to understand whether more popular topics are associated with higher engagement metrics such as views, likes, and comments.

# Data sources
1. YouTube API — collects keyword-based engagement data such as views, likes, and comments.
2. Kaggle dataset — provides large-scale YouTube video statistics for validation.
3. Google Trends — measures keyword popularity over time.

# Project Structure

- `src/` — source code for data collection and analysis  
- `data/` — collected datasets  
- `results/` — generated visualizations  
- `doc/` — project report  
- `main.py` — entry point for running pipelines  

# Outputs
Generated figures are saved in the `results/` folder.  
Processed datasets are saved in the `data/` folder.

# Results 
-Makeup videos show the highest average views, indicating strong visual-driven engagement.
-Food videos receive the highest average likes.
-Makeup videos generate the most comments.
-Keyword popularity is related to engagement, but the relationship is not always consistent.

# Challenges
-TikTok data was difficult to access because of the lack of a stable public API.
-Google Trends requests were limited by HTTP 429 errors.
-Multiple datasets required format standardization.
-Small-scale API data and large-scale Kaggle data were used differently for analysis and validation.

# Installation
- You need to set your YouTube API key in a `.env` file.
- Required Python packages include: `pandas`, `matplotlib`, `google-api-python-client`, `pytrends`, `python-dotenv`, and `pytest`.
- Install dependencies using:
```bash
pip install -r requirements.txt

```markdown
## Running Analysis

Run individual pipelines:

```bash
python src/main.py --youtube
python src/main.py --kaggle
python src/main.py --trends