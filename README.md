# node-movie-scrape
Simple Node.js scraper for IMDb
## Installation

###Install npm (node package manager)
```
  curl http://npmjs.org/install.sh | sh
```

###Install the dependencies
The folders need to be in the same directory as the server.js file.
```
  [sudo] npm install express
  [sudo] npm install request
  [sudo] npm install cheerio
  [sudo] npm install q
```

## Usage

###To run it 

``` js
  node server.js
```

###Search for a movie
To search for a movie, you put the movie's name and year in the URL request.
``` js
  http://localhost:8081/scrape?title=matrix&year=1999
```  
###Result
This returns a JSON object that contains selected information about the movie.
``` js
  {
    "Title":"The Matrix",
    "Year":"1999",
    "imdbRating":"8.7",
    "Director":"Andy Wachowski, Lana Wachowski",
    "Actors":"Keanu Reeves, Laurence Fishburne, Carrie-Anne Moss",
    "Plot":"A computer hacker learns from mysterious rebels about the true nature of his reality and his role in the war against its controllers.",
    "Poster":"http://ia.media-imdb.com/images/M/MV5BMTkxNDYxOTA4M15BMl5BanBnXkFtZTgwNTk0NzQxMTE@._V1_SX214_AL_.jpg",
    "Metascore":"73",
    "imdbVotes":"970,378",
    "imdbID":"tt0133093"
  }
```  
##License
This project uses the [MIT license](http://opensource.org/licenses/MIT).
