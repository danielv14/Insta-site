Insta-site web applications
-------------------------------------
This is a simplified version of the Insta-site that only shows the gallery and the slideshow.

Configuration
=====================================
If you want to use the web applications on your own site it is recommended that you take a look at [The Instagram developer site](http://instagram.com/developer/ "Instagram developer") and follow the inscructions there to set up your own client and get your own client id. You then change the client id in search.js and slideshow.js like this:

```
feed = new InstagramFeed({
                clientId: 'my-client-id' (change to your own id)
```

If you want to configure the slideshow to display pictures connected to another tag you simply modify the file slideshow.js in the javascript folder like this:

```
feed = new InstagramFeed({
                get: 'tagged',
                tagName: 'vsco' (change vsco to whatever you like)
```
You can change the limit of pictures to fetch both in the files slideshow.js and search.js like this:

```
feed = new InstagramFeed({
                limit: '30' (can be changed from 1-60)
```