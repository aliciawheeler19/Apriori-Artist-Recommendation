# Apriori-Artist-Recommendation

This a recommendation system powered by the Apriori Machine Learning Alogrithm. The recommendatino system is accessed through a GUI that allows users to type an artist name and be returned a list of artists that relate to the given artist. The Apriori Model was learned on a Spotify playlist dataset that contains 17024 playlists with each having between 3 to 10 unqiue artists in each playlist. 

To begin running the model, the user needs to download the [datasets](https://drive.google.com/drive/folders/1nVcBvJIye0hD2Qzzpku5_gc2unJLhCxZ?usp=sharing) which can be found in this shared Google Folder. 

There are two options for starting the Recommendation System and loading the data:
1) If user wants to use the original Spotify dataset they can begin loading the data from chunk labeled Spotify Dataset. Once loaded the user will need to go through the Data Cleaning chunk of code which will clean the original dataset. 
2) If the user wants to immediatly use the cleaned dataset, then they can load the data under the chunk labeled Dataset Analysis. We have provided the csv of the cleaned Spotify data and it can be loaded through that code.

Once the data has been loaded the user can explore the data through the Data Anlysis protion of the code or jump straight into building the model. To begin building the model the user needs to go to the The Apriori Algorithm Implementation and first begin running the code in the Data Setup section. Here the data will be reaggrated into unique playlists with a list of unique artists found in the playlist. The dataframe is also filtered to just contain playlilsts that have between 3 to 10 unique artists. Following the data is transformation, the item sets are changed into tuples of strings of unqiue artist names in a list. 

With the prepared data, the code chunks in the Model section can be run. Here the data is run through the Apriori Algorithm and itemsets and rules are created. When the model finishes running it is possible to run all the rules or filter the rules by a specific artist. In our code our example is we filter the rules for just "Kanye West", but this can be changed for any artists. Once the model is ready, the user can test the model to make sure it is running as expected.

Finally, the user can run the GUI code under the section header GUI Implementation and from there the user can begin seeing how the model works. While the code is running, the user is prompted to pass in an artist name. This name will be run through the models rules that were previously created and then the GUI will return a list of artists that associate to the passed artist name. 
