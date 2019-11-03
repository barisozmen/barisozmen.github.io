# Spark Resources

## Quick start

Spark 101 (14 min read) ([blogpost](https://mapr.com/blog/spark-101-what-it-what-it-does-and-why-it-matters/))

Getting Started with Apache Spark 2.x (4 hour read) ([e-book](https://mapr.com/ebook/getting-started-with-apache-spark-v2/assets/Spark2018eBook.pdf))

Advanced Data Science On Spark (2 hour watch) ([Spark Summit Talk](https://www.youtube.com/watch?v=hde53g-VXdg&feature=youtu.be&list=PL-x35fyliRwioDix9XjD3HptH8ro55SuB&t=5602)) ([slides](http://stanford.edu/~rezab/slides/sparksummit2015/))

## Longer reads

Mastering Apache Spark ([e-book](https://jaceklaskowski.gitbooks.io/mastering-apache-spark/))

## Tuning & Debugging

Configuration parameters ([Spark docs](https://spark.apache.org/docs/latest/configuration.html))

7 tips to debug ... ([databricks blog](https://databricks.com/blog/2016/10/18/7-tips-to-debug-apache-spark-code-faster-with-databricks.html))
  - Scale up slowly
  - In Spark UI, drill down to task page, sort tasks, examine "Erros" column
  - Reproduce errors
  - Examine dataset partitioning 
      - large data + too few partitions (symptom: there are few tasks, but each takes a lot of time)
      - small data + too many parititions (overhead of many partitions can slow down the job)
      - spark.sql.shuffle.partitions
  - Beware bad inputs
  
Spark UI ([databricks blog](https://databricks.com/blog/2015/06/22/understanding-your-spark-application-through-visualization.html))

<img width="350" alt="Screen Shot 2019-10-26 at 11 06 20 AM" src="https://user-images.githubusercontent.com/14996155/67624013-b2711080-f7e0-11e9-8876-7b344a364fff.png">

Practical optimization ([databricks training](https://databricks.com/session_eu19/apache-spark-core-practical-optimization))

Spark: The Definitive Guide Book ([Ch18-Monitoring and Debugging](https://learning.oreilly.com/library/view/spark-the-definitive/9781491912201/ch18.html))  ([Ch19-Performance Tuning](https://learning.oreilly.com/library/view/spark-the-definitive/9781491912201/ch19.html))

Debugging and logging best practices ([blogpost](https://dzone.com/articles/talend-and-apache-spark-debugging-and-logging-best))

## RDD, DataFrame, Dataset APIs

A tale of three Apache Spark APIs:... ([databricks blog](https://databricks.com/blog/2016/07/14/a-tale-of-three-apache-spark-apis-rdds-dataframes-and-datasets.html)) ([Spark summit video](https://www.youtube.com/watch?v=Ofk7G3GD9jk))

<img width="400" alt="Screen Shot 2019-10-26 at 10 50 22 AM" src="https://user-images.githubusercontent.com/14996155/67623828-a5ebb880-f7de-11e9-93ac-0ae1084794d9.png">




