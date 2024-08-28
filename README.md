# 🎵 music application

## 📄 Description

This Java project is a simple application for managing music and podcasts, with features for playing and enjoying audio, as well as classifying and listing user preferences. The project is organized into different classes to represent audios, songs, and podcasts, and includes functionalities for interacting with the audios.

## 🗂️ Project Structure

### 🎧 `Audio` Class
The `Audio` class is the base class for representing audio, whether it is a song or a podcast. It has the following attributes and methods:

#### Attributes:
- **`title` (String)**: Title of the audio.
- **`totalReproductions` (int)**: Total number of audio reproductions.
- **`totalLikes` (int)**: Total number of likes for the audio.
- **`classification` (int)**: Audio classification.

#### Methods:
- **`getTitle()`**: Returns the title of the audio.
- **`setTitle(String title)`**: Sets the title of the audio.
- **`getTotalReproductions()`**: Returns the total number of audio reproductions.
- **`getTotalLikes()`**: Returns the total number of likes for the audio.
- **`getClassification()`**: Returns the audio classification.
- **`like()`**: Increases the total number of likes.
- **`reproduce()`**: Increments the total number of reproductions.

### 🌟 `MyFavorites` Class
The `MyFavorites` class is responsible for adding audios to the user's list of preferences and displaying messages based on the classification of the audios.

#### Method:
- **`include(Audio audio)`**: Checks the audio rating and prints a message indicating whether the audio is a major success or is liked by many.

### 🎵 `Music` Class
The `Music` class extends the `Audio` class and adds attributes specific to songs.

#### Attributes:
- **`album` (String)**: Song album.
- **`singer` (String)**: Singer of the song.
- **`genre` (String)**: Musical genre.

#### Methods:
- **`getAlbum()`**: Returns the song album.
- **`setAlbum(String album)`**: Sets the song's album.
- **`getSinger()`**: Returns the singer of the song.
- **`setSinger(String singer)`**: Sets the singer of the song.
- **`getGenre()`**: Returns the musical genre.
- **`setGenre(String genre)`**: Sets the musical genre.
- **`getTotalReproductions()`**: Overrides the method to return a ranking based on total reproductions (10 if more than 2000 reproductions, otherwise 8).

### 🎙️ `Podcast` Class
The `Podcast` class also extends the `Audio` class and adds attributes specific to podcasts.

#### Attributes:
- **`presenter` (String)**: Podcast presenter.
- **`description` (String)**: Description of the podcast.

#### Methods:
- **`getPresenter()`**: Returns the podcast presenter.
- **`setPresenter(String presenter)`**: Sets the podcast presenter.
- **`getDescription()`**: Returns the description of the podcast.
- **`setDescription(String description)`**: Sets the description of the podcast.
- **`getClassification()`**: Overrides the method to return a rating based on total likes (10 if more than 500 likes, otherwise 8).

### 🏠 `Main` Class
The `Main` class contains the main method that initializes and interacts with the `Music`, `Podcast`, and `MyFavorites` objects.

#### Method:
- **`public static void main(String[] args)`**: This method creates `Music` and `Podcast`

## Autor

Kaio Vitor - [GitHub](https://github.com/Kaio-0708)
