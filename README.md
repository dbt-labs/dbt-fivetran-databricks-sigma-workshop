Welcome to your new dbt project!

### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [dbt community](https://getdbt.com/community) to learn from other analytics engineers
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices


Errors while doing project:

- Q: Encountered an error: Runtime Error Database Error in model stg_retail_customers (models/staging/retail/stg_retail_customers.sql [INSUFFICIENT_PERMISSIONS] Insufficient privileges: User does not have SELECT on Table 'raw.retail.customers'. SQLSTATE: 42501
- A: Check that correct permissions are set on raw, retail, and customers. 

- Q: Infinite loading when trying to preview.
- A: Make sure that in Catalog a cluster is selected from dropdown menu in top left. 

- Q: 04:32:44 Encountered an error:
Database Error
  Database Error
    [INSUFFICIENT_PERMISSIONS] Insufficient privileges:
    User does not have permission CREATE on CATALOG. SQLSTATE: 42501
- A: Make sure that catalog for user such as "dbt_srobb" already exists or that user has permission to create Catalog. In optional setting under connections verify that Catalog name matches.
# dbt-fivetran-databricks-sigma-workshop
