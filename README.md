
Table of Contents
1. [What's My Definition of DevOps:](#whats-my-definition-of-devops)
    1. [The 3Cs of DevOps:](The3CsofDevOps:)
2. [Monitoring:](#Monitoring:)
3. [Where to implement monitoring](#Wheretoimplementmonitoring)
    1. [Resource monitoring:](#Resourcemonitoring:)
4. [What you need from your data](#Whatyouneedfromyourdata)
.
.
.


# What's My Definition of DevOps:
 DevOps = Developer + Operations
 So we always had a developer who writes the code, maybe a build/release team that will do deployment in different environments, and a Operations person who owns and manages the infrastructure. In other words, a typical pre-DevOps era setup, with minimal or no automation.
 These teams used to work in silos, completely unaware of the workings of other teams. But the problem arises when there is a production outage, and when chaos and confusion starts, the Operations team blames the release team for wrong deployment and release team passes it back to Development for a buggy code. I am sure we all have been in similar situations at one time or another.
 Now comes the interesting part: with new startups getting into the Agile model and new automation tools readily available, there was a pressing need that, for small teams, Development should be able to understand and handle the deployment and infrastructure while Operations should be able to differentiate between an infrastructure and code issue. This would lead to a smooth deployment and better and timely resolution in case of production issues.
 This is how a need for DevOps expertise came into picture, creating the need for someone who understands the code and can also maintain the infrastructure and administrative responsibilities.
 This still best the question, can anyone who knows coding, some fancy automation tools, and how to sufficiently manage infrastructure provide that DevOps expertise?
 I am not against this definition, but I personally feel that in all this discussion, the key point that is completely neglected is developing a flexible mindset that would lead to what we now call a "DevOps culture.”
 In my opinion, instead of giving so much importance to the the DevOps toolchain (Cloud, CI/CD, containers, monitoring, configuration management, etc.) for building a state-of-the-art DevOps team, organizations should focus on existing individuals and teams within the organization who have a flexible mindset and are open to learn and adapt to new technologies.
 The focus should be on retraining these people into the latest skills and build what I call as a Flexible DevOps Culture.

 ## The 3Cs of DevOps:
  I read somewhere that a successful DevOps is made of 3Cs: Continuous Change, Collaboration and Culture. 
  And it is so true: without developing a collaborative environment within the teams, and a culture to adapt to continuous change, no organization can claim to have achieved DevOps implementation success, no matter what tools or technologies you use.
  So for me, DevOps was and will always be more about having a flexible mindset and collaborative culture within the organization, and less about the tools specifically. That does not mean that I deny the benefits of these tools and do not give them importance, but I would prefer a team or an individual that is more receptive and open to a DevOps culture than someone with a knowledge of the entire DevOps toolchain but is rigid and unwilling to learn or change.
  And what makes me happy is that I now see a lot of people and organizations understanding the importance of DevOps culture and not just the DevOps toolchain.

# Monitoring:
When developing for reliability or implementing resilient DevOps practices, the heart of your decision-making is data. Without carefully monitoring key metrics like uptime, network load, and resource usage, you’ll be blind to where to spend development efforts or refine operation practices. Fortunately, a wide variety of monitoring tools are available to help you collect and get visibility into this data.
While it might be tempting to try to monitor absolutely everything in your system, more focused monitoring will be easier to implement and leave you with more actionable data. SRE practices like SLOs are most useful when based on metrics for customer impact. Deciding what and how to monitor is an important decision. We’ll walk you through the basics in this blog post. We’ll also suggest a few popular monitoring tools for your consideration.

## Where to implement monitoring
It’s important to decide where in your system architecture you’ll implement monitoring. This will allow you to develop your architecture around the monitoring tool, rather than having to retrofit existing code. Depending on the location of implementation, monitoring tools will be able to observe different types of data. Here’s a breakdown of the most common types of monitoring implementations, along with examples of tools offering that type of monitoring:
### Resource monitoring:
Also known as server monitoring or infrastructure monitoring, this operates by gathering data on how your servers are running. Resource monitoring tools report on RAM usage, CPU load, and remaining disk space. In architectures with physical servers, information on hardware health—like CPU temperatures and component uptime—can also be helpful to avoid server failure. In cloud-based environments, aggregates of your virtual server system are more useful. 
### Network monitoring:
This looks at the data coming in and out of your computer network. Your monitoring tool captures all incoming requests and outgoing responses across all components such as switches, firewalls, servers, and more. The data collected from network monitoring can be as simple as the total amount of data coming and going or as nuanced as the frequency of particular requests. 
### Application performance monitoring:
APM solutions collect data on how an overall service is performing. These tools will send their own requests to the service and track metrics such as the speed and completeness of the response. The goal is to drive detection and diagnosis of application performance issues to ensure services perform at expected levels. 
### Third-party component monitoring:
This involves monitoring the health and availability of third-party components in your architecture. In this era of microservices, it’s likely that your service depends on the proper functioning of external services, from cloud hosting to ad servers. Like application performance monitoring, tools can check the status of these services with their own requests. 
You will likely want to include some of each type of monitoring in your overall solution. Prioritize having robust, redundant monitoring tools to ensure potential issues aren’t missed. At the same time, metrics and alerts should be tied to services to ensure relevance with business impact.
## What you need from your data
Having actionable data isn’t just about the data itself; in order to respond properly to what your monitoring tools are reporting, you need to have that data presented in the most useful way. Here are some things that monitoring tools can do for you:

- Trigger alerts when metrics exceed certain thresholds
- Create logs of events, highlighting based on parameters
- Create graphs of metrics over time
- Provide a dashboard of key service health components at a glance
- Create databases of logs that can be queried

When making development decisions or responding to an incident, try to get in the habit of asking yourself, “What would I need to be looking at right now to make the best choice?”. Visualize what data it would contain and the metrics that matter.

## Open source vs purchased
Another important point to consider is where you’ll find your monitoring tools and who will maintain them. There are both open source and purchasable tools with their own pros and cons.

### Open source monitoring tools 
These tools are free, which is an advantage for companies with limited tooling budgets. They’re also completely customizable, allowing you to integrate them into your own architecture. However, this customization will require dedicated development time and perhaps specialized knowledge. Furthermore, there is no SLA guaranteeing availability, security, update frequency, etc. Your team would own these responsibilities.

### Purchased monitoring tools
These tools cost but offer  robustness that open source tools cannot. The service provider will be accountable for keeping the tool functioning and up-to-date. The provider will likely offer customer service, training, documentation, and other resources to help you integrate the tool with your stack. In the era of reliability, making investments to ensure your monitoring eyes are always open is worth considering.

# Monitoring in DevOps:
 will first try to understand the concept of usage of DevOps tools in totality. We will also try to understand the advantages that these tools bring to the table if they are deployed to our Production grade environments. Alongside the benefits that these bring to the table, there are also pointers that these try to show on how the applications are maintained in a better manner for the best to reap. DevOps can be best understood as the gap that can be bridged to bring in both the software development and the IT operations together. By bringing in both these extremes to one, there will be a better and a responsible team of individuals who would respond to the situation accordingly rather than waiting on each other to do their particular responsibilities.

 ## DevOps Monitoring Tools:
  It should come as no surprise that we’re starting our discussion of DevOps tools with a focus on the set we know best: monitoring tools. A good monitoring platform lets you monitor infrastructure and application performance, whether on-prem, in the cloud, or across containerized environments — so you have complete visibility into every system, all the time.
  Whether you want to monitor Kubernetes, IoT devices, or bare metal, the right monitoring tool helps make it possible.
  Benefits: An effective monitoring tool improves system performance and productivity, and helps you reduce (or even eliminate) downtime. You can adequately plan for upgrades and new projects, and better allocate your time and resources. You can detect problems — and solve them — before they impact users.

  ### 1.Prometheus:
   Relies on the pull method to collect information, with a built-in database.
   Prometheus is yet another metrics based time series database that is primarily designed for white-box monitoring. It is an open source system monitoring tool and also an alerting tool which has an active ecosystem. Since its inception, many Organizations and Companies have adopted the tool itself into their ecosystems – thus enabling the user community and the developer community to be active. It is now a standalone open source project that is being independently maintained without any dependency from any Organization as such. It is next to Kubernetes to join the Cloud Native Computing Foundation in the year of 2016.
   Following are some of the advantages of using Prometheus, let us now take a look at each and every one of them:
   Advantages:
   It is an easy to deploy an application with any of the configuration management tools available in the market.
   It is a tool that’s written in Go language, making an apt choice for future developments
   It also addresses monitoring micro-services for your Organization
   It can also collect time series data for your Organization
   Provides seamless integration with a PagerDuty tool as well
   It has no dependencies altogether and provides a good amount of Web API for custom development
   The data thus collected with this application finds its use in Business Intelligence space as well
   It can provide fairly simple pre-made docker images and also other pre-made configurations for similar tools as like Docker.

  ### 2.Solarwinds:
   This app offers several products, each specializing in different areas of monitoring: Network Management, Systems Management, Database Management, IT Security, IT Service Management, Application Management, and Managed Service Providers. Each can be tried for free.

  ### 3.Sensu:
   A flexible and scalable telemetry and service health checking solution for monitoring servers, containers, services, applications, functions, and connected devices.

  ### 4.Nagios:
   The legacy monitoring tool that introduced monitoring practices to a generation of operators.
   Nagios provides application, network, and server monitoring using a combination of agentless and agent-based software tools for Unix, Linux, Windows and web environments. The system offers uptime, response, and availability using a variety of reporting formats and visualization.

  ### 5.OpManager:
   OpManager is an end-to-end network management software for heterogeneous, multi-vendor enterprise IT networks. It offers a unified approach to scale and manage distributed IT infrastructure, advanced fault and performance management functionality across critical IT resources viz. network devices, WAN or VoIP links, servers, virtual servers (VMware and Hyper-V), Domain controllers, MS Exchange, MS SQL and other IT infrastructure components.
   Applications Manager provides you with critical information (like CPU and memory usage, thread count and PGSQL database details) essential to track the performance of OpManager. Let’s take a look at what you need to see to monitor OpManager and the performance metrics to gather with Applications Manager

  ### 6.Zabbix:
   This app  is a mature and effortless enterprise-class open source monitoring solution for network monitoring and application monitoring of millions of metrics.

 ## DevOps Configuration Management Tools:
  Configuration management tools allow you to automate the provisioning and deployment of systems, enforce desired configurations, and remediate configuration drift. By modeling your infrastructure as code, you can apply software delivery practices like version control, automated testing, and continuous delivery to infrastructure and applications.
  Benefits: Automating work that used to be manual, repetitive, and error-prone results in greater speed, predictability, and scalability — and the assurance of standardized configurations across test, dev, and production environments. Eliminating snowflake servers reduces time (and headaches) and lets you deploy software faster and more reliably.

  ### 1.Ansible:
   Written in Python, agent-less, utilizes an imperative (rather than declarative) approach.

  ### 2.Chef:
   Written in Ruby, also relies on an imperative config management approach.

  ### 3.Puppet:
   Relies on a declarative config management approach, using a domain-specific language and an agent/master architecture.

 ## DevOps Alerting Tools:
   Alerting tools provide both actionable and informational system alerts, and can be customized to fit the complexities of your systems. For example, your alerting system needs to be sensitive enough to cover an outage — but not so sensitive that you’re catching frequent, intermittent problems that A) users aren’t going to see and B) inundate you with needless alerts.
   Benefits: Alerting tools help lay the foundation for your alerting policies, so you can determine who to notify, how to track issues and outcomes, and how to prioritize remediation.

  ### 1.PagerDuty:
   On-call management platform with add-ons for analytics, event intelligence, and automated incident response.
  ### 2.ServiceNow:
   Utilizes automated workflows for ITSM, as well as customer service and business processes.
  ### 3.Slack:
   Lets you consolidate alerts into the same platform you use for group chats and collaboration.

 ## DevOps Visualization Tools:
   A visualization tool might be considered the pièce de résistance of your DevOps toolchain for monitoring: you get to combine all of your data, sort and visualize it, and display it on customizable dashboards.
   Benefits: Visualization tools provide context and meaning, allow you to track changes and improvements over time, and give management a real-time view that helps guide strategic decisions. Customization options make it easy for team members to design and share their own dashboards.

  ### Grafana:
   Can be used on top of a variety of different data stores, including Graphite, InfluxDB, and Elasticsearch.

 ## Metrics Storage:
  What: Once you’ve automated configuration management, alerting, and monitoring, you’ll have a whole lot of data at your disposal to learn from. The challenge: How do you securely store and analyze it? You need a storage system that lets you aggregate and learn from system capacity, user behavior, service levels, security risks, and more.
  Benefits: The insights you gain from your metrics inform decisions across all layers of your business, improving your ability to meet SLAs, satisfy customer expectations, and make the case for new strategic investments. Data-driven decisions promote a culture of continuous learning and improvement.

  ### 1.Splunk:
   Splunk comes as a powerful platform that helps analyze machine data (especially logs that get generated on a frequent basis but seldom used effectively). Best scenarios to understand the prowess of the tool are the Production data center and the other in the Marketing department. Splunk the Organization produces software that finds its usage in the areas of Search, Monitoring and analyzing machine-generated data via the web-style interface. It gathers all the relevant information into a Central index that can rapidly search for the required details.
   Splunk can provide an eagle’s view on what is happening in your machine-generated data. We can also rely on Splunk for identifying the historical trends and also correlate a varied number of sources of information and also helps in many ways. Splunk can efficiently capture and also analyze massive amounts of unstructured, time series textual machine data – this is done by Splunk alone and no other tool can replace this for this requirement as such.
   Following are some of the advantages of using Splunk, let us now take a look at each and every one of them:
   Advantages:
   One of the biggest advantages of using Splunk is the ease of use that it offers to the individuals who use it.
   It allows us to analyze data from network, servers, applications and also from various other sources of information.
   It is very easy for anyone to deploy it on a Production environment too
   Provides tools like Splunk lite which can be used to push your data from various servers to the main Splunk engine for all the required analysis.
   The way Splunk indexes the data is such that it provides fantastic analytic results
   Reports that are generated by Splunk are accurate to the decimal which helps any Organization to determine the improvement steps and also to act upon them, should the need be.
   Alongside all this, the pricing model is pretty reasonable
   There is a great number of articles available online to find its usages perfect and to make full use out of it.
  ### 2.InfluxDB:
   Time-series database that’s suited for long-term data storage.
  ### 3.AWS:
   Supports a wide range of storage purposes, including relational and non-relational databases, a data warehouse for analytics, a time-series database, a ledger database to store transactions, and more.

 ## Next Steps: Evaluating Your DevOps Tools:
  No matter where you are in your DevOps journey, it’s wise to re-evaluate the tools you’re using and identify where you can fine-tune. Think about the DevOps tools in the monitoring ecosystem as more than their capabilities; how you use them begins to define your habits, values, and work culture — and accordingly, the quality of your product or service and the value you bring to your users.
  To learn more about how DevOps tools work together — and their place within the monitoring ecosystem — be sure to visit Bonsai, the Sensu asset index, where you can search and discover monitoring use cases as well as many of the above-mentioned solutions and integrations.
