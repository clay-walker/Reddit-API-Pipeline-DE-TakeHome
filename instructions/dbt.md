# DBT

dbt (data build tool) is a transformation tools that sits on top of our data warehouse.

[tutorials](https://docs.getdbt.com/docs/dbt-cloud/cloud-quickstart).

## Setup (development)

1. Create a dbt account [here](https://www.getdbt.com/signup/).

1. Create a project or just stick to the default project created.

1. Setup Up a `Database Connection` - Select Redshift

1. On the next page, enter the relevant Redshift details. This includes the `hostname`. You'll find this in the AWS Redshift console, or from the `terraform output` command mentioned earlier. It will start with the name of your cluster and end with `amazonaws.com`. It will also require the port (likely `5439`), the database name (likely `dev`). You'll also need the database username (likely `awsuser`) and password for the database you specified in the `Terraform` step. Once everything is input, click the `Test` button at the top. If successful, click `Continue`. 

1. Once connection is established, choose `managed directory` and give it  a name. You can also choose Github if you have a Github repo setup for the dbt part of this project, like I have, although this will require a bit of configuration.

1. Once you've worked through these initial steps, click on `Start Developing`.

You are now in an IDE which is connected to your Redshift cluster. Here we'll run some basic transformations on our data.

1. Click on `initialize project`. This will populate the directory on the left hand side with folder and files we may need.

[Back to main README](../README.md)
