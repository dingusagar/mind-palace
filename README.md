# mind-palace

mind-palace is a tool for storing information as a knowledge graph as you read something online. 

Initial Idea : 
Use case 1 : 
Let's say you are reading a pdf ebook and keep highlighting the interesting points using the pdf highlighter. 
You finished reading the book. After few weeks, when you want to refresh / refer back something from the book, you have to go through the highlights in a sequential manner. 
Basically it's not well organized. 

This tool takes all the highlighted texts along with the section/chapter header info and stores it as an interactive knowledge graph like this. 

![image](https://github.com/dingusagar/mind-palace/assets/12700858/b965eefe-bdbe-4ff3-82dd-14ea2474427e)

Some feature ideas and how to implement them : 
1. The conversion from highlights to a useful knowledge graph should be completely automated. There shouldn't be any manual steps in between. This is the goal. 
2. Graph contains nodes and edges. nodes are concepts and edges connect different concepts. How do we take a highlighted text and convert it into a node ? We can probably do text summarization, and topic modeling on the highlighted text and the surrounding texts, get the key concept, and make it a node in the graph.
3. How different nodes are connected in the graph automatically? This needs some thought. But a simple approach to start with can be to make use of the pdf headers and sub headers to connect links between concepts.
4. In the knowledge graph visualizer, we should be able to do nice searches. This search should not just match with the node names, but also the actual highlighted texts and surrounding texts maybe. Search can be powered using semantic search using either sentence transformers.

Rollout Plans: 
-  The first version can be a POC, a simple python application that takes a pdf as input and extracts the highlights, and builds the knowledge graph.
-  In the actual release, we can roll this out as a web application or Chrome extension. 


