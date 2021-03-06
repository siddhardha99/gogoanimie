# Gogoanime-API v.1π§¬
This is a personal project that I am working on π§°
it is a simple api for scrapping πͺ gogoanime.so 

**How to use the API ?**
<br />

π’ step 1
```
Download the repo π’
```

π’ step 2
```
npm install
```
this should install π» all the dependencies required for running this project π

<br />
π’ step 3

```
npm start
```
Now you should get a output similar to this

```
Listening to port 3000
```
π₯³ Yay, our API server is running πββοΈπ¨

π’ step 4 : Now visit
```
http://127.0.0.1:3000/
```
and you should be greeted with
```
π Hello worldπ, Welcome to π¦ GogoAnime API π§¬
```


# API Documentation π

*Running on localhost*

**Available routes**
	
	/Popular/:page_no
	
	/NewSeasons/page_no
	
	/getAnime/anime_id
	
	/getEpisode/episode_id
	
	/search/search_query
	

**GET | Popular Anime πΏ**
```
http://127.0.0.1:3000/Popular/:page
```
 >this will return all the popular anime
```
[
    {
        "name": "anime name",
        "img_url": "url",
        "anime_id": "anime id"
    }
    ...
]
```

**GET | New Seasons π**
```
http://127.0.0.1:3000/NewSeasons/:page
```
 >this will return all anime with new seasons available
```
[
    {
        "name": "anime name",
        "img_url": "url",
        "anime_id": "anime id"
    }
    ...
]
```
**GET | Anime π΅οΈββοΈ**
```
http://127.0.0.1:3000/getAnime/:anime_id
```
 >this will return the anime **name ,thumbnail image ,about  ?** and **episode_id** for all the episodes available for that anime
```
[
	{
	    "name": "anime name",
	    "img_url": "url",
	    "about": "Plot Summary: about the anime",
	    "episode_id": 
		    [
		        "some-anime-episode-1",
		        "some-anime-episode-2",
		        "some-anime-episode-3"
		         ...
		    ]
	}
]
```
**GET  | Anime Episode π½**
```
http://127.0.0.1:3000/getEpisode/:episode_id
```
 >this will return the downloadable  π» link for the episode
```
[
	    {
	        "quality": "watch(360P-mp4)",
	        "ep_link": "episode url"
	    }
	    
	    ...
]
```

**GET  | Search Anime π½**
```
http://127.0.0.1:3000/search/:search-query
```
 >this will return all the anime related to the search
```
[
    	  {
        	"name": "anime name",
        	"img_url": "url",
        	"anime_id": "anime id"
    	  }
	  
	  ...
	  
]	  
```
<br />
<br />

**π’ Troubleshootings**
<br />
This is just a personal project created for study / demonstration purpose and to simplify my working life, it may or may not be a good fit for your project(s).

<br />

**β€οΈ Show your support**
<br />
Please β­ this repository if you like it or this project helped you!
Feel free to open issues or submit pull-requests to help me improving my work.

<br />

**π€ Author**
<br />
Dhanush Suvarna

