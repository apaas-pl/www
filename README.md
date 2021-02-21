![aPaaS](https://logo.apaas.pl/1/cover.png)
# aPaaS.pl

+ [Strona informacyjna www](https://www.apaas.pl/)
+ [Dokumentacja aPaaS](https://docs.apaas.pl/)

## Tom Sapletta, DevOps Engineer at Softreck

I will delve deeper into meta-data aPaaS and general purpose programming aPaaS and provide key points that help enterprises choose the right aPaaS.
Pre-integrated stack of technology that we call "platform" should have happened around the 2003-05 timeframe. 
Hence the PaaS solutions we know of today in my view are only a necessary condition and not sufficient to really help large enterprises with where they need to go.

## Pre-cloud era

In the pre-cloud era there were:
+ no platforms
+ only products
+ IT departments (in big enterprises) had different structue, with "enterprise architecture groups" that defined the platform for their enterprise. 
+ They hand-crafted a platform definition standard for their enterprise by combining various products like:
  + app servers
  + web servers
  + databases
  + middleware
  + integration servers
  + portal servers
  + workflow engines
  + ...

### Managing IT software infrastructure

That is the only way they could manage the IT software infrastructure of very large multi-country, multi-location enterprises. 
Every large enterprise had its own blueprint platforms and they did a lot of heavy lifting not directly connected to their business outcomes.

## Cloud era
This presents an opportunity to move away from large capital technology expenses and align technology costs directly with business growth




## What is the difference between iPaaS and aPaaS?


### Platform Usage, Lines of Business
+ Modeling driven process/app development
+ Fast, Iteratove, Visual, Colaborative

### Platform Covernance, Enterprise IT
+ 

### PLatform Engineering, PaaS Vendor


## Post-cloud era


+ all is streaming
zamiast zarządzać infrastrukturą, kreaować ją z inteligencją w odpowiedni spersonalizowany strumień danych i funkcjonalnośći zamiast sformatowanych iu zdefiniowanych struktur aplikacji i baz danych.




## why you decided to dockerize your app?

Today’s modern trend is to build applications using the Cloud-Native approach which revolves mainly around the following buzzwords:

+ Microservices
+ DevOps
+ Continuous Delivery

Let’s see how these concepts actually affect our decision of dockerizing our app.

### Effects of Microservices

By adopting the microservices architectural style, we end up building a single application as a suite of small services.
+ Each services running in it's own process and communicating with lightweight mechanisms. 
+ These services are built around business capabilities and independently deployable by DevOps (fully automated deployment machinery).

So, committing to this architectural approach most of the time implies developing and delivering our front-end as an independent service.


### Effects of DevOps

The adoption of DevOps culture, tools and agile engineering practices has, among other things, the nice effect of increasing the collaboration between the roles of development and operations. One of the main problem of the past (but also today in some realities) is that the dev team tended to be uninterested in the operation and maintenance of a system once it was handed over to the ops team, while the latter tended to be not really aware of the system’s business goals and, therefore, reluctant in satisfying the operational needs of the system (also referred to as “whims of developers”).

So, delivering our app as a Docker image helps reducing, if not removing entirely, the difference between running the service on a developer’s laptop, the production environment or any environment we may think of.


###  Effects of Continuous Delivery

By leveraging the Continuous Delivery discipline we build our software in a way that it can potentially be released to production at any time. 

Such engineering practice is enabled by means of what is normally called continuous delivery pipeline. The purpose of a continuous delivery pipeline is to split our build into stages (e.g. compilation, unit tests, integration tests, performance tests, etc.) and let each stage verify our build artifact whenever our software changes. Ultimately, each stage increases our confidence in the production readiness of our build artifact and, therefore, reduces the risk of breaking things in production (or any other environment for that matters).

So, creating a Docker image for our app is a good choice here because that would represent our final build artifact, the same artifact that would be verified against our continuous delivery pipeline and that could potentially be released to production with confidence.


