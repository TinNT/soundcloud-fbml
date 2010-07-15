# SoundCloud-FBML

SoundCloud track and playlist embeds can be easily added to a Facebook tab via Facebook's Static FBML application. This technique was made popular by Band of Horses [here](http://www.facebook.com/bandofhorses?v=app_4949752878). Here's how you do it:

## Add Static FBML & Navigate to Edit Page

### Add Static FBML

1. [Go here](http://www.facebook.com/apps/application.php?id=4949752878)
2. Click the **Add to my Page** link in the left column and a window will pop up
3. Click the `Add to Page` button next to the page you'd like to add it to
4. Click `Close` in the bottom right of the window
5. Go to your Page
6. Click on the `+` tab that is located after `Wall` `Info` (and other tabs)
7. This will bring up the _Add a new tab_ selector, search for **FBML** and click Static FBML
8. You have added a Static FBML tab!

### Navigate to Static FBML Edit Page

1. Go to your page
2. Click the **Edit Page** link in the left column
3. Scroll down until you find the FBML application box in the left column
4. Click the *Edit* link within its block

## Edit Static FBML

Give your tab a title by editing the **Box Title** field

The **FBML** area beneath the **Box Title** field is where you'll add your SoundCloud embed using the **fb:swf** FBML tag:

     <fb:swf swfsrc='http://player.soundcloud.com/player.swf?url=[http://soundcloud.com/bandofhorses/sets/infinite-arms][url]&auto_play=true&player_type=artwork&color=000000'
     imgsrc='http://stream.bandofhorses.com/images/facebook_play.jpg' 
     height='425'
     width='425'
     swfbgcolor='000000' 
     quality='high' />

[url]: # "url"