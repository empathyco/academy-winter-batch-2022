# Week 4: Getting better at indexing :smirk_cat:
Going on with the first approach to indexing of week 3, the purpose for this week was to reduce the time spent by the indexing task, for which we had to evaluate different code alternatives and choose one that fitted our code. ([Alberto Villamayor](https://github.com/avillamayordevega) helped us a bit :eyes:)

## Session
### Indexing review with Alberto

*06/04/2022*

#### Participants & Content Deliverers

| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Alberto Villamayor](https://github.com/avillamayordevega) | \

\
&nbsp;

**Key learning points**
1. BulkRequest indexing
2. Technology and design recommendations

****


## Exercise
With all the mapping and requests created, we were set to index every document in _title.basics.tsv_. Unfortunately for us, the 
indexing was very slow, so we had to find some sort of solution :snail:.

Going through the jungle of ElasticSearch Java API documentation, we discovered something that could do the trick: **BulkRequest**. **BulkRequest** is an API class that allows sending to ElasticSearch batches of documents to be indexed, dramatically increasing the performance. We struggled a bit with it to keep it working but as always, **academy search team** overcame the difficulties :sunglasses::ok_hand:.

After making everything work (:mage:) [Alberto](https://github.com/avillamayordevega) reviewed our code and told us about some code improvements that could be made and recommended us the usage of some coding tools such like _SonarLint_ and _Insomnia_.

<Statement>

**Author** [Daniel Barrientos](https://github.com/DaniBAIG7)
- Research regarding options for improving the indexing time
- Introduction of changes (BulkRequest) to improve indexing
- Swagger documentation
- Javadoc

**Author** [Alberto Díez](https://github.com/uo266536)
- Research regarding options for improving the indexing time
- Introduction of changes (BulkRequest) to improve indexing
- Swagger documentation
- Javadoc

**Author** [Marcos Tobías](https://github.com/MarcosTobias)
- Research regarding options for improving the indexing time
- Introduction of changes (BulkRequest) to improve indexing
- Swagger documentation
- Javadoc
