# Week 8: TSV cleaners and Suggestions :smirk_cat:
This week was kinda tough for us. We did some meetings with Front and Data paths, asking them for the data they wanted from the datasets available in IMDB. After these meetings, we reached an agreement with them, and so, we had to change some things, because we were indexing at that point 2 files, and now we had to index at least, 7. In principle, this was a problem, because indexing that amount of documents would take a lot of hours, but between us, we agreed on cleaning tsvs of unnecesary content. Finally, we had a meeting with Miriam about Suggestions. 

## Session
### Relevance review with Alberto

*11/05/2022*

#### Participants & Content Deliverers

| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Miriam Ábalo](https://github.com/MiriamLynx) | \

\
&nbsp;

**Key learning points**
1. Cleaning TSVs and indexing documents inside documents
2. Understand how suggestions work 🔮 

****

## Exercise
We reached a key point in the development of our project: with our APIs, documents can be indexed and queries can be done. But it is true that our hits are not as accurate as we would want... 😿 It was clear that some adjustments regarding how we boost the results have to be done. It has to be CLEAR that if we look for Final Fantasy VI, Final Fantasy VI has to be our FIRST result 📝.

In order to achieve what we introduced before, we have to analyze how the relations were between all the files which we needed to index. After that, we started with removing all the adult films from the tsvs, as we don't need them 📝. Then, we continued with removing all the contents published before 1970... It is an unorthodox solution, but we had to clean it in some way...

After that, we started composing mapping for that new structure, taking into account that our principal "entity" was title basics, and then, among all its attributes, it has objects that are from another files, such as akas, principals... 

Finally, we did some research regarding suggestions, that will be implemented next week🤖.

<Statement>

**Author** [Daniel Barrientos](https://github.com/DaniBAIG7)
- Research regarding suggestions
- Research and merge of tsv files
- Repository documentation
- Swagger documentation
- Javadoc

**Author** [Alberto Díez](https://github.com/uo266536)
- Research regarding options for improving the relevancy of our results
- Research regarding options to dockerize the whole API
- Repository documentation
- Swagger documentation
- Javadoc

**Author** [Marcos Tobías](https://github.com/MarcosTobias)
- Research regarding options for improving the relevancy of our results
- Research regarding options to dockerize the whole API
- Repository documentation
- Swagger documentation
- Javadoc