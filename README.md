# 👋 Hi!

- 👋 Hi, We are the Data Team that works on [XING's jobs marketplace](https://xing.com/jobs) :-) We work at [NEW WORK SE](https://www.new-work.se/) which is the company behind [XING](https://xing.com/). 
- 👀  We develop recommender systems, search services and other machine learning based components and provide data insights that help shaping strategy and product.
- 🇪🇺 We are a distributed team of Data Engineers, Data Analysts and Data Scientists located in Germany (Hamburg) and Spain (Valencia, Barcelona). 
- ✨ We are continuously seeking Data Engineers, ML Engineers and Data Scientists who are passionate about solving hard problems at scale to help millions of people to find a job. See also: [Open Positions](#open-positions)
- 📫 Contact: Fabian Abel ([XING](https://www.xing.com/profile/Fabian_Abel), [LinkedIn](https://de.linkedin.com/in/fabianabel), email:  firstname.lastname@xing.com). 

⚠️ This github account is primarily intended to give people who are interested in joining our team some insights about our work. Our actual code is hosted on our internal Github enterprise instance. 

ToC:

- [Open Positions](#open-positions)
- [About Us](#about-us)
  + [Team](#team)
  + [Topics that we work on](#topics-that-we-work-on)
  + [Technologies that we are using](#technologies-that-we-are-using)
  + [Problems that we are dealing with](#problems-that-we-are-dealing-with)
  + [Modus operandi: how we work](#modus-operandi-how-we-work)
  + [Contact](#contact)

# Open Positions

We are fairly flexible regarding locations, e.g. we have offices in Hamburg, Barcelona or Valencia and allow for remote work from countries in which XING / NEW WORK SE has a legal entity (currently: Germany, Spain, Portugal, Poland, Italy, Austria, Switzerland). 

We currently seek people who can help us building search & recommender services + related services/components (e.g. one of it would be a real-time processing engine equipped with extractors and classifiers that help increasing the quality of job ads): 

- **[(Senior) Data Engineers](https://www.new-work.se/de/karriere/jobs/job/senior-data-engineer-m-f-x-1320823)** 
- **[Scala Developers](https://www.new-work.se/de/karriere/jobs/job/senior-scala-developer-1337608)** 

# About Us

## Team

- we are 10 people and are a quite international team (people from Spain, Argentina, Mexico, Brazil, Germany)
- most of us live in Hamburg and sometimes work from the headquarter which is [located in the harbour](https://www.google.com/maps/place/Unilever+Haus,+Strandkai+1,+20457+Hamburg/@53.5389891,9.991192,17z/data=!3m1!4b1!4m5!3m4!1s0x47b18f004b230c6f:0xa7b6b23ba647bbd8!8m2!3d53.5389891!4d9.9933807), 2 people are located in Valencia and 1 in Barcelona. 
- Currently, we are organized in two teams: 
  + (1) Analytics: in-depth analyses supporting product development and reporting to help steering product development, strategy and business
  + (2) Data Engineering & Science: development of search and recommender services, data processing components and other ML-based components that are part of the production system


## Topics that we work on

- Analytics: product analytics (e.g. ad-hoc analyses to support product decisions), reporting (e.g. development of Tableau dashboards)
- Forecasting: predicting business KPIs, predicting performance of job ads
- Search: everything related to search and discovery. 
- Personalization: Recommender Systems such as [job recommendations](https://www.xing.com/jobs/), etc. 
- Data Quality: enriching existing data assets, text processing, various classification tasks, etc.
- Data Science Platform: contributing to tooling and libraries for building data services and facilitating the usage of machine learning & Co.


## Technologies that we are using

- [Cassandra](http://cassandra.apache.org/) is the key-value store that we often use for making pre-computed stuff available to the REST services that provide, e.g. MYMK recommendations, job recommendations & Co.
- [Scala](http://scala-lang.org/) is our main programming language (for both service layer (= REST services) as well as for writing MapReduce batch jobs or custom [Hive](https://hive.apache.org/) UDFs)
- [Python](https://www.python.org/) is used for analyses, data visualization and also for some of our workflows running in production. 
- [Elasticsearch](https://www.elastic.co/) is our search technology/infrastructure
- [Hortonworks](http://hortonworks.com/) is the Hadoop distribution that we are using as infrastructure for batch processing. In particular, we use: [Spark](http://spark.apache.org/) and [Hive](https://hive.apache.org/) for both exploratory analyses as well as for workflows that are running in production, plain MapReduce, [Airflow](https://airflow.apache.org/), [Oozie](http://oozie.apache.org/) and an own Scala DSL for specifying Oozie workflows, ...
- [Exasol](https://www.exasol.com/) is another data warehouse that we use for analytics. 
- [Kubernetes](https://kubernetes.io/) is used as deployment infrastructure on which we run our delivery services
- [Kafka](http://kafka.apache.org/) and [Akka](http://akka.io/) come often into play when we do stream processing
- [Tableau](https://www.tableau.com/) is what we use for dashboards. We also make use of the [Adobe Experience Cloud](https://business.adobe.com/) for some parts of our reporting. 

## Problems that we are dealing with

- Machine learning problems ranging from classification problems to learning to rank tasks, hyper-parameter optimization and automated machine learning
- Automating machine learning processes, CI/CD for machine learning
- Search, personalized search, inferring meaning of search queries
- Recommender systems: trying to predict in which items a XING user may be interested in
- Realtime processing pippelines: building pipelines that process new incoming data on the fly
- Scalable REST services: developing serach/recommende/... REST services that receive thounds of requests per second
- Data quality: measuring and monitoring data quality and trying to enhance the value/utility of XING's data assets
- Entity resolution: given some text we try to understand to which entity this text may refer to (e.g. location, XING member, company, jobrole, etc.)
- Matching problems: (a) given an entity, try to find similar entities or (b) given two entities, try to find the commonalities between those entities
- ...

## Modus operandi: how we work

- we focus on getting things done and are flexible regarding the tools, methods, organizational structures, etc. that we use
- we heavily run A/B tests to proof that new things really help our users
- we try to automate as much as possible (including deployment of services, training of ML models, A/B testing; see e.g.: [Automating ML for RecSys](http://fabianabel.de/dn19/2019-11-automating-ml-for-recsys.pdf))
- hierarchies are flat and there is no strict separation between job roles (e.g. Software Engineers are free to dive into data analyses and Data Scientists push code to production). In fact, all of us write code. 
- we collaborate with folks from universities (e.g. with our friends from [CrowdRec](http://crowdrec.eu/) or as part of the [ACM RecSys Challenge](http://recsyschallenge.com/) that we organized [2016](http://2016.recsyschallenge.com/) and [2017](http://2017.recsyschallenge.com/))
- we go to / organize conferences, meetups, workshops and give talks 
- our services/apps get a huge amount of traffic. Hence, when joining our team, you can have quite a big impact on XING and our users (e.g. by building stuff that helps people to find a job and helps companies to attract and find talents)
- See also what others think about working at NEW WORK SE / XING: reviews on Kununu for [NEW WORK SE](https://www.kununu.com/new-work) and [XING](https://www.kununu.com/xing)

## Contact

Feel free to drop me (Fabian Abel) a message, e.g. via email (pattern: firstname.lastname@xing.com).
