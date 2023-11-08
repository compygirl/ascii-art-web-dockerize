
# ASCII - ART - WEB - DOCKERIZE
* `ayessenb` 
* `roshakba` 



Ascii-art-web-dockerize consists on making your site :

    more appealing, interactive and intuitive.
    more user friendly.
    give more feedback to the user.
    has Dockerfile for creating multiple images and containers


#### Description:


* We used text/template pakage to recieve and send GET/POST requests.
* GET /: Sends HTML response, the main page.
* POST /ascii-art: sends data to Go server (text and a banner). Displays the result in the route /ascii-art after the POST is completed. So going from the home page to another page.
* Linked external css file to make good design 
* Added a Dockerfile which creates two images and container



## Usage/Examples
Cloning storage to your host
```CMD/Terminal 
git clone git@github.com:compygirl/ascii-art-web-dockerize.git
```
Go to the downloaded repository:

```CMD/Terminal 
cd ascii-art-web-dockerize
```
Run a program:
```CMD/Terminal 
docker build --tag web .
docker run -dp 8080:8080 web
```


check the running containers:
```CMD/Terminal 
docker ps
```

check file system:
```CMD/Terminal 
docker exec -it <container's name> sh
ls -l
exit
```


Follow the link on the terminal:
```CMD/Terminal 
Starting server got testing... http://127.0.0.1:8080 
```


Choose your font and write a message to output



## HTTP status codes
* OK (200), if everything went without errors.
* Not Found, if nothing is found, for example templates or banners.
* Bad Request, for incorrect requests.
* Internal Server Error, for unhandled errors.



## Feedback

If you liked our project, we would be grateful if you could add `Star` to the repository.

Alem Student
20.06.2023.