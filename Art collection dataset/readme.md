#### This analysis demonstrates a full data workflow, including data loading, merging, cleaning, aggregation, and visualization. It’s an excellent case study for a portfolio project or YouTube tutorial because it:

- Works with real-world museum data.
- Involves multiple datasets that require merging.
- Uses time-series and categorical analysis.
- Applies modern visualization techniques with Plotly.
- Tells a compelling data story about trends in the art world.


#### Summary of the MoMA Art Collection Analysis
### 📌 Goal of the Analysis
The primary goal of this analysis was to explore the Museum of Modern Art (MoMA) collection and extract meaningful insights about the artists, artworks, and acquisition trends. We aimed to:

- Understand the dataset structure by merging multiple files.
- Analyze artist demographics, including nationality and gender.
- Explore artwork classifications and department distributions.
- Identify trends in acquisitions over time.
- Check which artworks are currently on display at MoMA.
- This analysis serves as a real-world data project for aspiring data analysts and showcases data cleaning, merging, and visualization techniques using Python.

### 🔍 Key Findings from the Data
Artists & Demographics
- There are ~15,600 unique artists in the dataset.
- The top nationalities of artists include American, French, German, British, and Italian.
- Male artists significantly outnumber female artists in the dataset.
  
Artwork Characteristics
- The most common classifications of artworks include prints, photographs, paintings, drawings, and sculptures.
- The department with the most artworks is Drawings and Prints.

Acquisition Trends
- The number of artworks acquired by MoMA peaked in the 1960s and 2010s.
- Acquisitions have declined in recent years (2020-2024).

Current On-Display Artworks
- Around 1,210 artworks are currently on display at MoMA.

### 📊 Data Analyst Tools & Techniques Used
Throughout this project, we applied fundamental data analysis techniques:

- 1️⃣ Data Exploration & Cleaning
Loaded multiple datasets (Artists, Artworks, OnView) and merged them.
Handled missing values and converted data types (e.g., DateAcquired to datetime).
- 2️⃣ Data Merging
Used merge() in pandas to join datasets on ConstituentID, allowing us to connect artists with their artworks and check which are on display.
- 3️⃣ Data Aggregation & Summarization
Used value_counts() to analyze the most common nationalities, artwork classifications, and artist demographics.
Used nunique() to count unique artists.
- 4️⃣ Time-Series Analysis
Converted acquisition dates into a time-series format using pd.to_datetime().
Created a trend analysis of MoMA’s acquisitions over time.
- 5️⃣ Data Visualization (Using Plotly)
Bar Charts: Nationalities, Gender Distribution, Artwork Classifications.
Line Chart: Acquisition trends over time.

###💡 What We Learned
- MoMA’s collection is dominated by Western artists, particularly American and French.
- The gender imbalance in art history is visible in MoMA’s dataset, with far more male artists than female artists.
- Prints and photographs are the most common types of artworks in the collection.
- Acquisitions have fluctuated significantly over time, with major peaks in the 1960s and 2010s.
