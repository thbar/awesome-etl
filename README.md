# awesome-etl
A curated list of notable ETL (extract, transform, load) frameworks, libraries and software.

- [Awesome ETL](#awesome-etl)
    - [ETL Tools (GUI)](#etl-tools-gui)
    - [Workflow Management/Engines](#workflow-managementengines)
    - [Job Scheduling](#job-scheduling)
    - [Python](#python)
    - [Ruby](#ruby)
    - [Go](#go)
    - [Talks/Articles](#talksarticles-1)
    - [Cloud Services](#cloud-services)
    - [Big Data (Hadoop Stack)](#big-data-hadoop-stack)


## ETL Tools (GUI)
* [Pentaho Kettle](http://community.pentaho.com/projects/data-integration/) - The most popular open-source graphical ETL tool.
* [Talend](https://www.talend.com/products/talend-open-studio) - "an open source application for data integration job design with a graphical development environment"
* [Informatica PowerCenter](https://www.informatica.com/products/data-integration/powercenter.html) - "a toolset for establishing and maintaining enterprise-wide data warehouses. It has a customer base of over 5,000 companies."
* [Microsoft SSIS](https://technet.microsoft.com/en-us/library/ms141026.aspx) - "a component of the Microsoft SQL Server database software that can be used to perform a broad range of data migration tasks."
* [Apache NiFi](https://nifi.apache.org/) - "a rich, web-based interface for designing, controlling, and monitoring a dataflow."

## Workflow Management/Engines
* [Luigi](https://github.com/spotify/luigi) - "a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built in."
* [TaskFlow](https://wiki.openstack.org/wiki/TaskFlow) - "allows the creation of lightweight task objects and/or functions that are combined together into flows (aka: workflows) in a declarative manner. It includes engines for running these flows in a manner that can be stopped, resumed, and safely reverted."
* [Airflow](https://github.com/airbnb/airflow) - "Use airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The airflow scheduler executes your tasks on an array of workers while following the specified dependencies. Rich command line utilities make performing complex surgeries on DAGs a snap. The rich user interface makes it easy to visualize pipelines running in production, monitor progress, and troubleshoot issues when needed."
* [Pinball](https://github.com/pinterest/pinball) - "a scalable workflow management platform developed at Pinterest. It is built based on layered approach."
* [Azkaban](https://azkaban.github.io/) - "a batch workflow job scheduler created at LinkedIn to run Hadoop jobs. Azkaban resolves the ordering through job dependencies and provides an easy to use web user interface to maintain and track your workflows."
* [Dray.it](http://dray.it/) - "Docker workflow engine. Allows users to separate a workflow into discrete steps each to be handled by a single container."

## Job Scheduling
* [Chronos](https://github.com/mesos/chronos) - "a distributed and fault-tolerant scheduler that runs on top of Apache Mesos that can be used for job orchestration."
* [Dagobah](https://github.com/thieman/dagobah) - "a simple dependency-based job scheduler written in Python. Dagobah allows you to schedule periodic jobs using Cron syntax. Each job then kicks off a series of tasks (subprocesses) in an order defined by a dependency graph you can easily draw with click-and-drag in the web interface."

## Python
### Libraries
* [Pandas](http://pandas.pydata.org/) - Implements dataframes in Python for easier data processing and includes a number of tools that make it easier to extract data from multiple file formats.
* [Bubbles](https://github.com/stiivi/bubbles) - "a Python ETL Framework and set of tools. It can be used for processing, auditing and inspecting data. Focus is on understandability and transparency of the process."
* [SQLAlchemy](http://www.sqlalchemy.org/) - "the Python SQL toolkit and Object Relational Mapper that gives application developers the full power and flexibility of SQL."
* [dataset](https://dataset.readthedocs.org/en/latest/) - A wrapper around SQLAlchemy that simplifies database operations (including upserting).
* [Dask](https://github.com/blaze/dask) - Ever tried using Pandas to process data that won't fit into memory? Dask makes it easy.
* [Blaze](https://github.com/blaze/blaze) - "translates a subset of modified NumPy and Pandas-like syntax to databases and other computing systems."
* [Odo](https://github.com/blaze/odo) - Moves data across containers (SQL, CSV, MongoDB, Pandas, etc). Claims to be the easiest and fastest way to load a CSV into your database.
* [xmltodict](https://github.com/martinblech/xmltodict) - Makes working with XML as easy as working with JSON. Also allows streaming so you don't run out of memory on large XML files.
* [Celery](http://www.celeryproject.org/) - "an asynchronous task queue/job queue based on distributed message passing. It is focused on real-time operation, but supports scheduling as well."
* [MrJob](https://pythonhosted.org/mrjob/) - "lets you write MapReduce jobs in Python 2.6+ and run them on several platforms. The easiest route to writing Python programs that run on Hadoop."
* [Joblib](https://pythonhosted.org/joblib/) - "a set of tools to provide lightweight pipelining in Python."
* [Orange](http://orange.biolab.si/) - "data visualization and analysis for novice and experts. Data mining through visual programming or Python scripting. Components for machine learning. Add-ons for bioinformatics and text mining. Packed with features for data analytics."
* [BeautifulSoup](http://www.crummy.com/software/BeautifulSoup/) - Popular library used to extract data from web pages.
* [PyQuery](https://pythonhosted.org/pyquery/) - Extracts data from web pages with a jquery-like syntax.
* [PETL](https://github.com/alimanfoo/petl) - "a general purpose Python package for extracting, transforming and loading tables of data." Slower than Pandas and not as good for larger amounts of data, but simpler.

### Talks/Articles
* https://vimeo.com/73628111
* http://www.parsely.com/misc/slides/streamparse/notes/

## Ruby
* [Kiba](https://github.com/thbar/kiba) - "provides you with a DSL to define ETL jobs"
* [Square ETL](https://github.com/square/etl)

## Go
* [Crunch](https://github.com/jondot/crunch) - "A fast to develop, fast to run, Go based toolkit for ETL and feature extraction on Hadoop."

## Talks/Articles
* https://medium.com/@samson_hu/building-analytics-at-500px-92e9a7005c83
* http://www.slideshare.net/g33ktalk/data-pipeline-acial-lyceum20140624
* http://chairnerd.seatgeek.com/building-out-the-seatgeek-data-pipeline/
* http://www.garynissen.com/etl-hand-code-or-tool/
* http://www.slideshare.net/CasertaConcepts/big-data-warehousing-meetup-bigetl-trad-tool-vs-pig-vs-hive-vs-python-what-to-use-when-slide-set-2
* https://deepfriedcode.com/books/darps/index.html
* http://blog.cloudera.com/wp-content/uploads/2010/01/IntroToPig.pdf
* http://tech.adroll.com/blog/data/2015/10/15/luigi.html?adrolldev

## Cloud Services
* [Google Dataflow](https://cloud.google.com/dataflow/what-is-google-cloud-dataflow) - "Google Cloud Dataflow provides a simple, powerful model for building both batch and streaming parallel data processing pipelines."
* [Amazon Data Pipeline](https://aws.amazon.com/datapipeline/) - "a web service that helps you reliably process and move data between different AWS compute and storage services, as well as on-premise data sources, at specified intervals."
* [Amazon SWF](https://aws.amazon.com/swf/) - "helps developers build, run, and scale background jobs that have parallel or sequential steps. You can think of Amazon SWF as a fully-managed state tracker and task coordinator in the Cloud."
* [Snaplogic](http://www.snaplogic.com/) - "a self-upgrading, elastic execution grid that streams data between applications, databases, files, social and big data sources."

## Big Data (Hadoop Stack)
* [Spark](https://spark.apache.org/docs/0.9.0/index.html) - "a fast and general-purpose cluster computing system. It provides high-level APIs in Scala, Java, and Python that make parallel jobs easy to write, and an optimized engine that supports general computation graphs. It also supports a rich set of higher-level tools including Shark (Hive on Spark), MLlib for machine learning, GraphX for graph processing, and Spark Streaming."
* [Pig](https://pig.apache.org/) - "a platform for analyzing large data sets that consists of a high-level language for expressing data analysis programs, coupled with infrastructure for evaluating these programs."
