# DBT Cloud Run Deployment Template

The purpose of this repository is to have a template starting point for deploying a dbt project to cloud run in gcp. 

## Prerequisites

To run this locally you will need to have:
- A local environment with `dbt-bigquery` installed
- The gcloud sdk setup and installed 
- A billable gcp project

## Getting Started

1. Clone this repository `git clone https://github.com/matthh9797/dbt-cloud-run-template.git`
2. Update the YOUR_PROD_DATASET, YOUR_LOCATION, YOUR_PROJECT, YOUR_DEV_DATASET in `profiles.yml`
3. Update your project name in the folder, `dbt_profiles.yml` and `profiles.yml`
4. Run the scripts in the `setup/` folder one by one
5. Optionally, create a key for the dbt-sa service account and setup your dev target in profiles to connect via the key. This make things a bit more seemless in development.

## References

- Deployment Scripts: [https://github.com/meteatamel/cloudrun-tutorial/blob/master/docs/scheduled-dbt-service-bigquery.md](https://github.com/meteatamel/cloudrun-tutorial/blob/master/docs/scheduled-dbt-service-bigquery.md)
- More Background: [https://medium.com/@ivan_toriya/step-by-step-guide-to-run-dbt-in-production-with-google-cloud-platform-fb1f035f3c7b](https://medium.com/@ivan_toriya/step-by-step-guide-to-run-dbt-in-production-with-google-cloud-platform-fb1f035f3c7b)