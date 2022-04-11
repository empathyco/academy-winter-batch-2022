# Unlocking Elasticsearch #
During Week 2, we started learning how Elasticsearch works. It has not been very difficult for us as we have previous experience. I do not want to rise our egos that much, but this background gave us the ability to soak up like sponges.
## First steps ##
You must understand that our past approaches with search engines or databases were with relational databases, and it is a somewhat difficult for our brains to get to really appreciate the big difference between what we have been using and this.
Elastic stores a mapping from some content to documents, just the other way around as relational databases that use a forward index.
I have to mention that it also does not have any kind of constraint regarding indexing the data you give to Elastic, as long as it is a .json file. 
## Getting deeper... ##
After this brief explanation, we were introduced to how queries are used in Elastic.
Pretty simple, you ask what you want to find, and Elastic returns what it thinks you were looking for. But without a problem: if you are not as specific as you have to regarding some filters/analyzers, you could end up being annoyed as hell, so it is very important to **specify** .
## Let's implement! ##
This was without any doubt the toughest point of the week so far. Elastic migrated their old API to a new one lacking documentation and we have to figure out how the things were done using infused knowledge. But downgrading the version of the API it was not the solution, because some methods required for us to start indexing documents were missing and I promise that we had chronic migraines for two days because of this.
At the end, and after many hours, many litres of coffee and many hours spent navigating through the javadoc of the API, our code started to do things and it was a feeling similar as when the prisoner of the myth of cave escaped and visualized the sun. 
