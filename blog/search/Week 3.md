# Week 3: Indexing
The purpose for this week is to index the database from IMDB, using the correct mapping options. Also develop documentation on Swagger and implement unit tests.

## Session
### Indexing and mapping with Elasticsearch

*06/04/2022*

#### Participants & Content Deliverers

| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Alberto Villamayor](https://github.com/avillamayordevega) | \

\
&nbsp;

**Key learning points**
1. Elasticsearch indexing
2. Mapping configuration
3. Tokenizers, filters and analyzers
4. Elasticsearch data types
5. Documentation with Swagger

****


## Exercise
(Autonomous work)
<Statement>
### [Repository](https://github.com/MarcosTobias/imdb-academy)
**Author** [Marcos Tobías](https://github.com/MarcosTobias)

&nbsp;

## Implementation

Deciding how to map the documents regarding these aspects was not very dificult, but turning it into code was another story.

Here was when we had to get our heads deep into the documentation. Nonetheless, it proven to be easier to understand that we expected, and although it took some time to get accustomed to the sintax, we were able to implement a basic mapping.

We were aware that this very likely was not the optimal solution, but it certainly was better than using the default mapping Elasticsearch provides, so on we went and indexed the hole collection.

The collection is almost ten million entries, so it goes without saying that it took a _while_.

&nbsp;

## Documentation and tests
As any good programmer should, we had to write tests and documentation, especially since the API in the making was going to be used by ther other paths. For that we were asked to use [Swagger](https://swagger.io/), which altough we were not very familiar with, we knew what it was and how it was supposed to look.

Regarding tests, we had some experience from the previous weeks, so implementing them was easier than we expected.

&nbsp;

## Wrapping up
Overall, we all agree that this has been the most interesting week so far. Beeing finally given a project to work on and wrap our heads around was very fun, and although we had some banging our heads against a wall moments with the occasional cryptiness of the documentation, being able to make it work was a very satisfactory experience. 

In the end, discovering how to solve a problem on your own is the best path to understanding.
