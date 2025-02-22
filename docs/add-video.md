# Adding A Youtube Video

To add a YouTube video you will need to do the following two things:

### Add YouTube Video ID

The first thing is to add the YouTube video ID to the metadata for the page. The video ID is the part that comes after "v=" in the url. For example:

`https://www.youtube.com/watch?v=_g46WiGPhFs`

In the above url the video ID is `_g46WiGPhFs`. We will take that and place it in the metadata like you see below: 

```
---
layout: post
authors: 
    - dtaivpp
comments: true
title: "Look Ma, It's a YouTube Embed!"

contributingToOpenSource: _g46WiGPhFs
---
```

Small note here you can name the video ID whatever you want. I have chosen to name it contributingToOpenSource as that is the name of the video I am linking. That can help you to ensure the right video ID is being placed in the correct spot.

### Inserting the video to the Blog

Finally, we will add the video to the correct section of the blog. We can do that with the below snippet: 

```
{% include youtube-player.html id=page.contributingToOpenSource %}
```

Here you can see we used the `contributingToOpenSource` name that we defined above with the video ID is used to specify which video goes in this section. Now you should be able to see your videos within the page! 
