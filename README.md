# Reddit ETL Pipeline

Original project here: https://github.com/ABZ-Aaron/Reddit-API-Pipeline 

A data pipeline to extract Reddit data from [r/dataengineering](https://www.reddit.com/r/dataengineering/). 

## Architecture

1. Extract data using [Reddit API](https://www.reddit.com/dev/api/)
1. Load into [AWS S3](https://aws.amazon.com/s3/)
1. Copy into [Snowflake](https://snowflake.com)
1. Transform using [dbt](https://www.getdbt.com)

## Output

Python code walkthrough (panel presentation)

Snowflake dashboard which depicts the following:

1. Total Authors
2. Total Posts
3. Top Posters
4. Upvote ratio of posts
5. Number of posts/day (visualized over time)
5. Cluster showing the correlation of votes to comments

## Setup

Follow below steps to setup pipeline.

> **NOTE**: This was developed using an M1 Macbook Pro. If you're on Windows or Linux, you may need to amend certain components if issues are encountered.

As AWS offer a free tier, this shouldn't cost you anything unless you amend the pipeline to extract large amounts of data, or keep infrastructure running for 2+ months.

1. [Reddit API Configuration](instructions/reddit.md)
1. [AWS Account](instructions/aws.md)
1. [Snowflake](instructions/snowflake.md)
1. [dbt](instructions/dbt.md)
