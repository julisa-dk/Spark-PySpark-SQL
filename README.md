# Spark-PySpark-SQL
Week 5

1. Connect to VM in GCP by ssh key

2. Add PYTHONPATH:
   export PYTHONPATH="${SPARK_HOME}/python/:$PYTHONPATH"
   export PYTHONPATH="${SPARK_HOME}/python/lib/py4j-0.10.9.5-src.zip:$PYTHONPATH"
   
3. Set up connection:
   spark = SparkSession.builder \
    .master("local[*]") \
    .appName('test') \
    .getOrCreate()
