# Week 7: Relevancy 2. Seeking for the best query :mag_right:
 Going on with the previous session, on Week 7 we started getting deeper knowledge on queries :brain:.

This required hard polishing of our mapping and analyzers, as well as our previous relevancy query. We worked hard to implement good search solutions :pencil: (search magic, woosh :mage:)

Also, we got some feedback on our code and solutions for the IMDb project and we continued our integration with the front path :smirk_cat:

## Session 1
### Relevance II

*04/05/2022*

#### Participants & Content Deliverers

| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Alberto Villamayor](https://github.com/avillamayordevega) | \

\
&nbsp;

**Key learning points**
1. Review of the contents of the previous week
2. Relevance tools in depth
3. Expected results

****

## Session 2
### IMDb Review

*06/05/2022*

 **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Jesús Rebordinos](https://github.com/jesus-rebor) |
| | [Miriam Ábalo](https://github.com/MiriamLynx) |
| | [Alberto Villamayor](https://github.com/avillamayordevega) |

\
&nbsp;

**Key learning points**
1. Check if our solutions were correct
2. Detect some common failures in our code
3. Follow better practices and conventions while coding
4. Use some specific and reccommended tools in our project

****

## Exercise
Although on Search we are kind of a family and we love to work together, we decided to work separately this week. 
This approach encouraged us to compete a bit with each other and try to build different, cool approaches for our different queries that make our APIs feel unique.

<Statement>

**Author** [Daniel Barrientos](https://github.com/DaniBAIG7)
- A query that builds relevancy by penalizing a bit the rating of the movies under the popularity. It also allows to include a year in the query sentence.
- Repository documentation
- Implementation of custom analyzers and tokenizers
- Implementation of custom mapping
- Improvement of code according to our Search mentors' feedback

**Author** [Alberto Díez](https://github.com/uo266536)
- Boosteo películas por encima de series y potencia título principal/título original y número de votos
- A query that boosts films over other kind of contents of the database and boosts both the title match and the number of votes + rating.
- Repository documentation
- Implementation of custom analyzers and tokenizers
- Implementation of custom mapping
- Improvement of code according to our Search mentors' feedback

**Author** [Marcos Tobías](https://github.com/MarcosTobias)
- Potencia por rating más que por numero de votos y películas por encima del resto de contenidos. 
- A query that boosts rating over popularity (number of votes). It also boosts films over other types of content of the database.
- Repository documentation
- Implementation of custom analyzers and tokenizers
- Implementation of custom mapping
- Improvement of code according to our Search mentors' feedback