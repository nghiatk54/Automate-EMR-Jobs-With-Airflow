Automate-EMR-Jobs-With-Airflow
Data pipeline end to end
Redfin data source -> Amazon EMR <--> S3 Bucket(raw/transform data) (trigger) -> Snowpipe (load) -> Snowflake -> PowerBI
DAG: start_pipeline >> create_emr_cluster >> is_emr_cluster_created >> add_extraction_step >> is_extraction_completed >> add_transformation_step >> is_transformation_completed >> remove_cluster >> is_emr_cluster_terminated >>  end_pipeline
Công nghệ sử dụng: Python, Amazon EMR, Amazon EC2, Amazon S3, Apache Airflow, Snowflake, PowerBI
