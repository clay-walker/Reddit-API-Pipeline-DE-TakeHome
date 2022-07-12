# DBT

dbt (data build tool) is a transformation tools that sits on top of our data warehouse.

[tutorials](https://docs.getdbt.com/docs/dbt-cloud/cloud-quickstart).

## Setup (development)

1. Create a dbt account [here](https://www.getdbt.com/signup/).

1. Create a project or just stick to the default project created.

1. Setup Up a `Database Connection` - Select Snowflake

1. On the next page, enter the relevant Snowflake details. 

1. Once the connection is established, choose `managed directory` and give it a name. You can also choose Github if you have a Github repo setup for the dbt part of this project, like I have, although this will require a bit of configuration.

1. Once you've worked through these initial steps, click on `Start Developing`.

You are now in an IDE which is connected to your Redshift cluster. Here we'll run some basic transformations on our data.

1. Click on `initialize project`. This will populate the directory on the left hand side with folder and files we may need.

[Back to main README](../README.md)
