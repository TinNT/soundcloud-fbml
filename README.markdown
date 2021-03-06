# SoundCloud-FBML

SoundCloud track and playlist embeds can be easily added to a Facebook tab via Facebook's Static FBML application. Here's how you do it:

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

Once you've made it to the Edit page, give your tab a title by editing the **Box Title** field

The **FBML** area beneath the **Box Title** field is where you'll add your SoundCloud embed using the [fb:swf](http://developers.facebook.com/docs/reference/fbml/swf) FBML tag:

     <fb:swf swfsrc='' imgsrc='' height='' width='' quality='best' />

* swfsrc: http://player.soundcloud.com/player.swf?url=url-to-your-track-or-set (Add [parameters](http://wiki.github.com/soundcloud/Widget-JS-API/widget-options) to customize colors, auto_play, and more.)
* imgsrc: URL of the image users must click before it turns into a SoundCloud player (Take a [screenshot](http://github.com/soundcloud/soundcloud-fbml/raw/master/examples/basic.png) of the player and add &auto_play=true above)
* height: The height of the SoundCloud player.
* width: The width of the SoundCloud player.

Here's a working example of the tag using the Band of Horses Infinite Arms set:

     <fb:swf swfsrc='http://player.soundcloud.com/player.swf?url=http://soundcloud.com/bandofhorses/sets/infinite-arms&auto_play=true&color=000000' imgsrc='http://github.com/leemartin/soundcloud-fbml/raw/master/examples/basic.png' height='325' width='425' quality='best' />

Once you've added your code, you can save your work by clicking the `Save Changes` button below.

Finally, return to your page, click the tab with the _Box Title_ you set earlier and make sure everything is in working order.

## Customize It

The Static FBML app let's you render HTML or FBML (Facebook Markup Language) for enhanced Page customization. This allows you to design a nice experience around your SoundCloud player with some basic HTML. [Check out](http://www.facebook.com/bandofhorses?v=app_4949752878) what Band of Horses did with one of our [artwork players](http://soundcloud.com/tour/widgets).

![Custom Tab Screenshot](http://github.com/soundcloud/soundcloud-fbml/raw/master/examples/custom_screenshot.png "Custom Tab Screenshot")

This look was achieved with some [basic HTML](http://github.com/soundcloud/soundcloud-fbml/raw/master/examples/custom.txt).

## Make it Private

If you would prefer to make your player only available to those Facebook users who have 'Liked' your page, simply use the **fb:visible-to-connection** tag in combination with an image or text explaining this. Check out this  [tab app](http://www.facebook.com/pages/SoundCloud-Dev/102523519809552?v=app_4949752878) to see this in action. And here's the [code](http://github.com/soundcloud/soundcloud-fbml/blob/master/examples/locked.txt) to get you started.

## Tips and Tricks

### Set as Default Landing Tab

You can set your SoundCloud tab to be the default landing page for your Facebook page. This is great for album/track premieres.

1. Go to your page
2. Click the **Edit Page** link in the left column
3. Look for the Wall Settings box in the left column
4. Click the _Edit_ link within its block
5. Set the _Default Landing Tab for Everyone Else_ dropdown to your tab (it will show up as your Tab's name)

# Copyright

**SoundCloud-FBML** is Copyright (c) 2010 [Lee Martin](http://Lee.Ma/rtin) and [SoundCloud](http://soundcloud.com), released under the MIT License.