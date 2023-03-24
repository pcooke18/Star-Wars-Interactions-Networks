<img src="https://media2.giphy.com/media/12Vg35jCqP610Y/giphy.gif" jsaction="load:XAeZkd;" jsname="HiaYvf" class="n3VNCb pT0Scc KAlRDb" role="" aria-label="" alt="Star-wars-icons GIFs - Get the best GIF on GIPHY" data-noaft="1" style="width: 1000px; height: 400px; margin: 40.479px 0px;">

Interactions within the Star Wars Universe

## Overview and Cleaning Steps
This project aims to better understand networks between characters in the Star Wars universe by looking into interactions between characters. The [dataset](https://github.com/evelinag/star-wars-network-data/blob/master/starwars-full-interactions.json) contains information related to 110 characters who appeared in the first 7 films and tracks number of times two characters speak within the same scence. The original data is quite sparse given it only contains information related to the number of interactions, so we added more information from the [Star Wars Databank Website](https://www.starwars.com/databank) in order to add information related to the character's main affiliation, species, and where they spent a majority of their time in the films. 

The Star Wars Function unpacks the JSON data and splits the data into links and nodes tables. The nodes table contains the ID of the character, their name, and the number of scenes they appear in while the links table holds the number of interactions between characters. We then manually added the 3 columns listed above into the nodes table, and then passed the nodes table through the Clean Gephi Nodes file in order to assign the value 'Other' for categories where there was not enough information to form meaningful groups. These data cleaning steps were taken in order to prepare the data for network analysis in the Gephi open source software

## Analysis
We set out to figure out which of the variables we collected from the Star Wars Databank would have the greatest impact on the Star Wars network, and we hypothecized that the Affiliation would have the greatest impact on the number of interactions between characters. We approached answering our research question by visualizing the network, identifying key characters and connections, then seeing which variable was the best at explaining the networks throughout the film series. The photo below visualizes the general shape of the Star Wars universe network that we used for the entirety of our analysis. 
This network uses color to indicate weighted degree, a metric used that takes the weight of all connections for a specific character. This assigns a dark green to characters with a high weighted degree, indicating that they are the most important characters in the Star Wars universe based on the strengh of thier connection's connections.

![Weighted_simple](https://user-images.githubusercontent.com/98417196/226241930-a1d8c259-31ef-4b6b-83b3-acf9bb41ea86.png)

## Conclusion

For those who are fans of Star Wars, it should come as no surprise that characters like Obi Wan and Anakin are some of the  most influential characters, but this information is important to note when analyzing the overall character network. We specifically focused on these influential characters when analyzing the effectivness of each variable in being ablle to determine the number of interactions between characters in the Star Wars universe. Ultimately, we found support for out hypothesis that Affiliations is a better way to understand the interaction network than variables like species or location. Our complete findings can be found in the Final Report document. Thank you for reading and may the force be with you!
