title: Using qDslrDashboard with the Sony a6000
tags:
- photography
- sony-a6000
---

Most of my posts are going to be something technology related but I _do_ happen
to have other interests. For a while now, I've had a Sony a6000 that I've been
very happy with. I'm very much an amateur at photography but I find it fun and I
like the images I get of my family more than the ones I can get from my iPhone.
So I've been slowly trying to level up my photography skills. I'm definitely not
over 9000 yet, but maybe one day I'll get there.

This Christmas, I finally got a tripod and it has gotten me interested in trying
to do some timelapse photography. Sony has a timelapse app but I wanted to see
what other options were out there. After a bit of Googling, I came across
[DslrDashboard](http://dslrdashboard.info). Confusingly, the apps have been
renamed to qDslrDashboard, but there is an app for just about every platform.

Since I own two iDevices, I went ahead and threw down the $10 it cost for the
iOS app. At first, I was hoping to find a free option to do timelapse, but I
definitely feel better giving a developer my ten dollars insted of just throwing
it at Sony. Since I didn't have my iPad right on hand, I started trying things
out with my iPhone. It took me a while to figure out how to get the app to work
with my phone, and honestly, I'm still not 100% sure how to get the thing to
work consistently every time. Here's what it took me to get my camera and my
iPhone running the qDslrDashboard app running.

* Go to https://www.playmemoriescameraapps.com/portal/
* Create an account (PlayStation Network acount, ugh.)
* Go to `Menu -> Applications`
{% asset_img application-list.jpg application list on the a6000 %}
* Select `PlayMemories Camera Apps`
{% asset_img playmemories-camera-apps.jpg application select PlayMemories
    Camera Apps on the a6000 %}
* Find Smart Remote Control app
* Install it

I still feel pretty gross about having to create a PlayStation Network account,
but there you go, all the steps to get the Smart Remote Control updated.

## Getting qDslrDashboard and the a6000 working together

Connect your device to the Wifi network created by the camera.

Once you do that, you can tap the sony button. The first time I tried, I had to
tap it a couple times and then it finally connected. At first I had though I had
wasted the 10 dollars on the qdslrdashboard ios app, but it finally worked.


So far, I barely know how to work it, but I was able to get it to take a
timelapse after fiddling with it for a bit.

**How to convert the images to a gif**

Show how to use imagemagick to convert to a gif

First, I usually resize my images

```bash
for file in *.jpg do;
  mogrify -resize 3840x2160^ -gravity center -crop 3840x2160+0+0 +repage
done
```

**How to make a movie out of the images**

Show how to use ffmpeg to make a movie from the images
