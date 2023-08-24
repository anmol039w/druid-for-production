# druid-for-production
This repo will serve as a guide on the journey to setup druid on kubernetes so others have what i didn't!!

This guide will cover my understanding of the database, it's components and why and hows of production issues

What is Druid??
In simple words Druid is an OLAP database, used for real time analytics, which allows ingestion from various sources, store the data in segments (more on this later) and supports sub-second queries at any scale.

We at Dukaan use Druid to collect,store and analyse data from users, we ingest around 2 Million data points everyday. The cost of running the setup mentioned in this repo is $1000 per-month (baremetal).But feel free to run this on any hosting provider of your choice. 