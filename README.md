# Reddit ETL Pipeline

Original project here: https://github.com/ABZ-Aaron/Reddit-API-Pipeline 

A data pipeline to extract Reddit data from [r/dataengineering](https://www.reddit.com/r/dataengineering/). 

Please perform the following tasks:

1. Extract data using [Reddit API](https://www.reddit.com/dev/api/)
1. Load into [AWS S3](https://aws.amazon.com/s3/)
1. Copy into [Snowflake](https://snowflake.com)
1. Transform using [dbt](https://www.getdbt.com)
1. Extract high level analytics using Snowflake queries/dashboard.

## Output

The purpose of this exercise is to see how you think/code and solve problems. It is purposefully broad, and there are no purely right/wrong answers.

Please prepare the following:

1. A walk through of your solution, including all code and configuration. 
1. Snowflake dashboard which depicts the following:

- Total Authors
- Total Posts
- Top Posters
- Upvote ratio of posts
- Number of posts/day (visualized over time)
- Cluster showing the correlation of votes to comments

## Setup

Follow below steps to setup pipeline.

> **NOTE**: This was developed using an M1 Macbook Pro. If you're on Windows or Linux, you may need to amend certain components if issues are encountered.

This is intended to be run on aws free tier. Please keep pipeline extracts limited in order to avoid any charges, and terminate any services once complete. Reach out if you have any concerns!

1. [Reddit API Configuration](instructions/reddit.md)
1. [AWS Account](instructions/aws.md)
1. [Snowflake](instructions/snowflake.md)
1. [dbt](instructions/dbt.md)
