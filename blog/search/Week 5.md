# Week 5: Indexing, but faster :runner:
Even with the batch requests from the previous week, we are not comtempt with the indexing time we achieved. We wanted it to be even faster. Thats why this week we tried different implementations, and in the end we had a meeting with Alberto who concluded that our solutions were, let's say, "non-optimal".

## Session
### Indexing review pt.2 with Alberto

*12/04/2022*

#### Participants & Content Deliverers

| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Jesús Rebordinos](https://github.com/jesus-rebor) | [Alberto Villamayor](https://github.com/avillamayordevega) | \

\
&nbsp;

**Key learning points**
1. Understanding why our improvements were lacking
2. Obtaining the best batch size for indexing operations

****

## Exercise
Alberto explained to us why our individual solutions for making indexing faster were not optimal, or in some cases even worse or just wrong. He also gave us some comments regarding our code, and finally he showed us some tests he had done regarding the optimal batch size. He concluded that 20k requests per batch was the optimal configuration, and that probably some changes from elastic 6 to 7 was what it caused this increment in indexing time that we were experiencing.

We reverted our implementation with this new batch size and moved on, marking the indexing part as done.

Nonetheless, we still had a lot of aspects to work on, so we kept improving our documentation, mapping and file reading.

On wednesday we had the Risk Prevention Session, and enjoyed Thursday and Friday off because of Easter holidays.

&nbsp;

<Statement>

**Author** [Daniel Barrientos](https://github.com/DaniBAIG7)
- Reverting indexing to optimal implementation
- Attend Risk Prevention Session
- Repository documentation
- Swagger documentation
- Enjoy Easter :moyai:

**Author** [Alberto Díez](https://github.com/uo266536)
- Reverting indexing to optimal implementation
- Attend Risk Prevention Session
- Repository documentation
- Swagger documentation
- Enjoy Easter :moyai:

**Author** [Marcos Tobías](https://github.com/MarcosTobias)
- Reverting indexing to optimal implementation
- Attend Risk Prevention Session
- Repository documentation
- Swagger documentation
- Enjoy Easter :moyai:

