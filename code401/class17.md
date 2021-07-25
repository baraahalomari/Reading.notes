## Review, Research, and Discussion

**Describe “The Cloud”**
The cloud" refers to servers that are accessed over the Internet, and the software and databases that run on those servers. Cloud servers are located in data centers all over the world. By using cloud computing, users and companies don't have to manage physical servers themselves or run software applications on their own machines.

**What is a container (as it relates to computers and servers)?**
A container consists of an entire runtime environment: an application, plus all its dependencies, libraries and other binaries, and configuration files needed to run it, bundled into one package. By containerizing the application platform and its dependencies, differences in OS distributions and underlying infrastructure are abstracted away.

**What is auto-scaling?**
It is a method used in cloud computing that dynamically adjusts the amount of computational resources in a server farm - typically measured by the number of active servers - automatically based on the load on the farm.

**What is bandwidth?**
Is the maximum rate of data transfer across a given path. Bandwidth may be characterized as network bandwidth, data bandwidth, or digital bandwidth.

**How do cloud providers compute service costs?**

When setting price, cloud providers determine the expense to maintaining the network. They start by calculating costs for network hardware, network infrastructure maintenance, and labor. These expenses are added together and then divided by the number of rack units a business will need for its IaaS cloud.

## Document the following Vocabulary Terms

**Server Instances :** is a collection of SQL Server databases which are run by a solitary SQL Server service or instance. The details of each server instance can be viewed on the service console which can be web-based or command-line based.

**Containers :**  is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another. A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings.

**Cloud Services :**  services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party and provide users with access to computing services such as analytics or networking via the internet.

**Cloud Architecture :** is how individual technologies are integrated to create clouds—IT environments that abstract, pool, and share scalable resources across a network. Cloud architecture is how all the components and capabilities necessary to build a cloud are connected in order to deliver an online platform on which applications can run.

**AWS :** is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis. These cloud computing web services provide a variety of basic abstract technical infrastructure and distributed computing building blocks and tools.

**EC2/Beanstalk vs Heroku :** Heroku and AWS Elastic Beanstalk, solutions (production configurations) is that they have comparable features and pricing. One big difference is that Heroku’s pricing takes exponential price jumps as one adds common additional features, e.g., auto-scaling, where-as AWS pricing is fairly linear. On the other hand, Heroku is generally simpler to get up and running as AWS has a fairly steep initial learning curve.

## Preview

**Which 3 things had you heard about previously and now have better clarity on?**
server

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**
aws,auth

**What are you most excited about trying to implement or see how it works?**
aws

# AWS S3

> Amazon S3 or Amazon Simple Storage Service is a service offered by Amazon Web Services that provides object storage through a web service interface. Amazon S3 uses the same scalable storage infrastructure that Amazon.com uses to run its global e-commerce network.


# AWS Lambda Basics
* “serverless computing service provided by Amazon Web Services (AWS). Users of AWS Lambda create functions, self-contained applications written in one of the supported languages and runtimes, and upload them to AWS Lambda, which executes those functions in an efficient and flexible manner”.

To complete a Serverless stack we need:

* computing service;
* database service; and
* HTTP gateway service.


# AWS Lambda Functions

> No servers to manage :AWS Lambda automatically runs your code without requiring you to provision or manage infrastructure.

> Continuous scaling :AWS Lambda automatically scales your application by running code in response to each event.

> Cost optimized with millisecond metering :With AWS Lambda, you only pay for the compute time you consume, so you’re never paying for over-provisioned infrastructure.

> Consistent performance at any scale :With AWS Lambda, you can optimize your code execution time by choosing the right memory size for your function.

# CDN

Content Delivery Network : “is a geographically distributed group of servers that work together to provide fast delivery of Internet content. A CDN allows for the fast transfer of data needed for loading Internet content including HTML pages, javascript files, stylesheets, images, and videos”.

