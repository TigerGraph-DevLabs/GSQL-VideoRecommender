# GSQL VideoRecommender (for YouTube/TikTok)

### Setup (in order):

```gsql drop all```: Drops any previous queries/schema you were running locally

```gsql setup.gsql```: Declares graph schema and runs loading job on mock dataset

```gsql tiktok.gsql```: Interprets Lovain community algorithm, installs video recommendation query that assigns every video a "score" and sorts them by this metric. The scoring system is simplistic and should be refined for real-world applications.

### Mock datasets:
```0.csv```: Creates edges between videoIDs and tags

```1.csv```: Creates edges between videoIDs and audio, also matches each videoID to a country

```2.csv```: Creates edges between users and videos (watched)

```3.csv```: Creates directed edges between 2 users (following)

```4.csv```: Matches each user to a country
