### Serverless Architectures (FaaS, BaaS)
###### Luis Fernando de Mingo López
###### 2019

#### Cloud Computing for IoT
---

## Add Some Slide Candy

![](assets/img/presentation.png)

---
@title[Customize Slide Layout]

@snap[west span-50]
## Customize Slide Content Layout
@snapend

@snap[east span-50]
![](assets/img/presentation.png)
@snapend

---?color=#E58537
@title[Add A Little Imagination]

@snap[north-west]
#### Add a splash of @color[cyan](**color**) and you are ready to start presenting...
@snapend

@snap[west span-55]
@ul[spaced text-white]
- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**
@ulend
@snapend

@snap[east span-45]
@img[shadow](assets/img/conference.png)
@snapend

---?image=assets/img/presenter.jpg

@snap[north span-100 headline]
## Now It's Your Turn
@snapend

@snap[south span-100 text-06]
[Click here to jump straight into the interactive feature guides in the GitPitch Docs @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend



---

# BackEndless

[Official link](https://www.backenless.com)

---

#  FireBase

[Official link](https://firebase.google.com)

####### Firebase is a mobile and web application development platform developed by Firebase, Inc. in 2011, then acquired by Google in 2014. As of October 2018, the Firebase platform has 18 products, which are used by 1.5 million apps

---

# Serverless Architecture

Serverless computing is a cloud computing model which aims to abstract server management and low-level infrastructure decisions away from developers. In this model, allocation of resources is managed by the cloud provider instead of the application architect, which can bring some serious benefits. In other words, serverless aims to do exactly what it sounds like — allow applications to be developed without concerns for implementing, tweaking, or scaling a server (at least, to the perspective of a user).

---

# Function As a Service (FaaS)

Function as a service (**FaaS**) is a category of cloud computing services that provides a platform allowing customers to develop, run, and manage application functionalities without the complexity of building and maintaining the infrastructure typically associated with developing and launching an app.

>Building an application following this model is one way of achieving a *serverless* architecture, and is typically used when building microservices applications.

---

## Providers

- AWS Lambda, was the first FaaS offering by a large public cloud vendor, followed by 
- Google Cloud Functions, 
- Microsoft Azure Functions, 
- IBM/Apache's OpenWhisk (open source) in 2016 and 
- Oracle Cloud Fn (open source) in 2017.

---

## PaaS vs FaaS (1/2)

![bg 100%](images/faas.png)

A similar concept to FaaS are platform as a service (PaaS) application hosting services, in that such application hosting services also hide *servers* from developers. However, such hosting services typically always have at least one server process running that receives external requests. 

- Scaling is achieved by booting up more server proceses, which the developer is typically charged directly for. Consequently, scalability remains visible to the developer.

---

## PaaS vs FaaS (2/2)

FaaS by contrast does not require any server process constantly being running. While an initial request may take longer to be handled than an application hosting platform (up to several seconds), caching may enable subsequent requests to be handled within milliseconds. As developers only pay for function execution time (and no process idle time), lower costs at higher scalability can be achieved (at the cost of latency).

---

## FaaS Advantages

![bg 100%](images/faas-adv.png)


- Fewer developer logistics — server infrastructure management is handled by someone else.
- More time focused on writing code / app specific logic — higher developer velocity.
- Inherently scalable. Rather than scaling your entire application you can scale your functions automatically and independently with usage.
- Never pay for idle resources.
- Built in availability and fault tolerance.
- Business logic is necessarily modular and conform to minimal shippable unit sizes.

---

## FaaS Disadvantages

- Decreased transparency. Someone else is managing your infrastructure so it can be tough to understand the entire system.
- Potentially tough to debug. There are tools that allow remote debugging and some services (i.e. Azure) provide a mirrored local development environment but there is still a need for improved tooling.
- Auto-scaling of function calls often means auto-scaling of cost. This can make it tough to gauge your business expenses.
- You now have a ton of functions deployed and it can be tough to keep track of them. This comes down to a need for better tooling (developmental: scripts, frameworks, diagnostic: step-through debugging, local runtimes, cloud debugging, and visualization: user interfaces, analytics, monitoring).
- Solutions for caching resources between stateless requests (i.e. DB connections) and recycling network requests are still pending.
