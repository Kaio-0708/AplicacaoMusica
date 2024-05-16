This Java project is a simple application for managing music and podcasts, with features for playing and enjoying audio, as well as classifying and listing user preferences. The project is organized into different classes to represent audios, songs and podcasts, and includes functionalities for interacting with the audios.

Audio Class
<br>
The Audio class is the base class for representing audio, be it a song or a podcast. It has the following attributes and methods:
<br>
Attributes:
<br>
title (String): Title of the audio.
totalReproductions (int): Total audio reproductions.
totalLikes (int): Total audio likes.
classification (int): Audio classification.
<br>
Methods:
<br>
getTitle(): Returns the title of the audio.
setTitulo(String titulo): Sets the title of the audio.
getTotalReproducoes(): Returns the total number of audio reproductions.
getTotalLike(): Returns the total number of likes for the audio.
getClassification(): Returns the audio classification.
like(): Increases the total number of likes.
reproduce(): Increments the total number of reproductions.



MyFavorites Class
<br>
The MinhasFavorites class is responsible for including audios in the user's list of preferences and displaying messages based on the classification of the audios.
<br>
Method:
includes(Audio audio): Checks the audio rating and prints a message indicating whether the audio is an absolute success or whether it is being liked by many.



Music Class
<br>
The Music class extends the Audio class and adds attributes specific to songs.
<br>
Attributes:
album (String): Song album.
singer (String): Singer of the song.
genre (String): Musical genre.
<br>
Methods:
getAlbum(): Returns the song album.
setAlbum(String album): Sets the song's album.
getSinger(): Returns the singer of the song.
setSinger(String singer): Sets the singer of the song.
getGenero(): Returns the musical genre.
setGenero(String genre): Defines the musical genre.
getTotalReproducoes(): Overrides the method to return a ranking based on total reproductions (10 if more than 2000 reproductions, otherwise 8).



Podcast Class
<br>
The Podcast class also extends the Audio class and adds attributes specific to podcasts.
<br>
Attributes:
presenter (String): Podcast presenter.
description (String): Description of the podcast.
<br>
Methods:
getPresenter(): Returns the podcast presenter.
setPresenter(String presenter): Sets the podcast presenter.
getDescricao(): Returns the description of the podcast.
setDescricao(String description): Sets the description of the podcast.
getClassification(): Overrides the method to return a rating based on total likes (10 if more than 500 likes, otherwise 8).



Main Class
<br>
The Main class contains the main method that initializes and interacts with the Music, Podcast and MyFavorites objects.
<br>
Method:
public static void main(String[] args): This method creates Music and Podcast instances, sets their attributes, simulates plays and likes, and adds the audios to the preference list to display the appropriate messages.
