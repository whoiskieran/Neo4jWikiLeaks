I have created a graph of the 2010 WikiLeaks Cablegate cables. There are 251,287 diplomatic cables in this graph.
This graph is relatively unsophisticated at the moment however I am planning to use NLP (Natural Language Processing) to process the text of the cables and create a more sophisticated graph
The files can be downloaded from github GitHub - whoiskieran/Neo4jWikiLeaks 3
The text of the cables are not included.

Graph Details

Node Types:
1. Cables 
2. Locations 
3. Tags 

Relationships
Cable [IS_TO] -> Locations
Cable [IS_FROM] -> Locations
Cable [IS_TAGGED_WITH] -> Tag
Cable [IS_MENTIONED_IN] -> Cable

To create the graph do the following (these instructions apply to Neo4j Desktop for Windows):

1. Create a blank Neo4j database 
2. Download the import folder from github 
3. Unzip cable_nodes.zip 
4. Move the files into the Import folder of the newly created database. 
5. Launch the terminal from Neo4j desktop. 
6. Put the bin folder in the path 
7. Move to the import folder. 
8. Run the import.bat file. 
