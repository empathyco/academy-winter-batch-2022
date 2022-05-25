# WEEK 7
Creating a next queries & related tag bot for Empathy.co metrics.

## Bot
### Creating a NQ and RT bot

*25-04-2022*

<!-- (Do not change the line below!!!) -->
| **Path Owner** | **Content Deliverer** | 
| --- | --- | 
| [Eva Gonzalez](https://github.com/evag-empathy) | [Edgar Herrero](https://github.com/edgarRSV4) | \ 

\
&nbsp; <!-- (Do not change this and above line PLEASE!!!) -->
**Key learning points** <!-- (Do not change this line!!!) -->
1. Bot
2. Next queries
3. Related tags
4. Tagging API

**** <!-- (Delete this comment and just leave the 4 *) -->

## Exercise
For an url given, create a bot with python that launches requests to Tagging API.

Goals:
- Read a .json file from a Python script
- For all the combinations found in the file, launch a tagging /query
request - must be with the same sessionId
- Once all those have been iterated once, reiterate changing the
sessionId
- Data will be available 24 h after you triggered the requests