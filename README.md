## Interactions Within the Star Wars Universe

#### Overview and Cleaning Steps
This project aims to better understand networks between characters in the Star Wars universe by looking into interactions between characters. The [dataset](https://github.com/evelinag/star-wars-network-data/blob/master/starwars-full-interactions.json) contains information related to 110 characters who appeared in the first 7 films and tracks number of times two characters speak within the same scence. The original data is quite sparse given it only contains information related to the number of interactions, so we added more information from the [Star Wars Databank Website](https://www.starwars.com/databank) in order to add information related to the character's main affiliation, species, and where they spent a majority of their time in the films. 

The Star Wars Function unpacks the JSON data and splits the data into links and nodes tables. The nodes table contains the ID of the character, their name, and the number of scenes they appear in while the links table holds the number of interactions between characters. We then manually added the 3 columns listed above into the nodes table, and then passed the nodes table through the Clean Gephi Nodes file in order to assign the value 'Other' for categories where there was not enough information to form meaningful groups. These data cleaning steps were taken in order to prepare the data for network analysis in the Gephi open source software

#### Analysis
The photo below visualizes the general shape of the Star Wars universe network. This simple graphic assigns color to weighted degree, which is a metric used that takes the weight of all connections for a specific character by looking at the strength of connections of all the other characters they are directly associated with, where the dark colors signify an important character in the films. 

![Weighted_simple](https://user-images.githubusercontent.com/98417196/226241930-a1d8c259-31ef-4b6b-83b3-acf9bb41ea86.png)

We used the features gathered from the Star Wars Databank website to group characters based on different features, and used visual cues to determine which feature was the best at explaining the interactions between characters across these films. Our findings can be found in the Final Report document. Thank you for reading and may the force be with you!
