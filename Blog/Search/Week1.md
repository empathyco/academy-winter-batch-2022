# Search Week 1: Settling down

## Initial meeting
With the objective of getting everything ready for working the next weeks, we did an initial brief meeting with our mentors of the Search team: Jesús Rebordinos, Miriam Ábalo and Alberto Villamayor, where we got a bird's eye view of the different technologies that we were going to work with on the following weeks and solved a few initial doubts that we had with them.

## Autonomous work
Just after the meeting, the Search team facilitated us the slides that we saw with them, just to have some reference to install everything on our own.

### Technologies to get working
- **SdkMan**: A handy software kit manager that allows easy installing and managing of different versions of SDK
- **Java**: Essential programming language (that we know very well), famous for its lemma _write once, run anywhere_, that pretty much summarizes what this extensively used language is capable of.
- **Maven**: Dependency manager for Java projects that centralizes and facilitates the managing of project builds, reporting and documentation.
- **Spring Framework**: A widely used JVM based framework that facilitates the development of micro-services and web applications, for example. It is famous for its serverless and reactive approach, as well of the configurations of the framework, that facilitate a lot otherwise much more complicated aspects, such like security and URL mapping.
- **Docker**: A lighter alternative to virtualization, that automates the application deploys by using Docker Containers. There exist plenty of Docker Images provided by different technologies (ElasticSearch, for example) that can be run in containers, thus providing an straightforward, encapsulated installation and running of these technologies.
- **ElasticSearch**: A search and analytics solution well known for its speed and the use of reverse indexing of documents.
- **Mockito**: Mocking framework that facilitates testing.

### What we had to do with them
We had to create a basic API, _/search_, as kind of a showcase of all these technologies working together; Just a simple reponse for a simple request, which shown the correct integration between the API REST in Spring and the ElasticSearch Docker container running.
Apart from this, we had to develop the corresponding tests with Mockito.

### Problems faced
Although it seemed very easy at first, we had problems with the version of the Elastic Java API and the ElasticSearch version. At first, we installed version 8.1.1 for Elastic Java API, and 7.11.1 for ElasticSearch Docker image, which made the interaction between Spring and the Docker ElasticSearch container impossible. We took a while to figure out which the problem actually was, but after downloading an image of ElasticSearch 8.1.1, we were able to solve it.
