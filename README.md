**What's in this fork?**


This fork adds a new example called `responsive` (see branch `example/responsive`). This example implement a mobile first / responsive UI with mute button and switch camera functionalities. A glitch demo is available [here](https://twilio-video-js-responsive.glitch.me/).

Mobile: 

![screenshot_20190920-130122_2](https://user-images.githubusercontent.com/54728384/65326641-db7eff80-dba9-11e9-92b1-78dd3e01133f.jpg)

Desktop: 

![desktop_screenshot](https://user-images.githubusercontent.com/54728384/65326604-c73b0280-dba9-11e9-8cc8-d91b814fdb8a.jpg)


**IMPORTANT:** Please upgrade to the latest version of twilio-video.js to avoid upcoming breaking changes in Firefox 68.
See [this advisory](https://support.twilio.com/hc/en-us/articles/360024434554-Twilio-Video-JavaScript-SDK-Breaking-Changes-in-Firefox-68-July-9-2019-) for details.

# Twilio Video Quickstart for JavaScript

[![OS X/Linus Build Status](https://secure.travis-ci.org/twilio/video-quickstart-js.png?branch=master)](http://travis-ci.org/twilio/video-quickstart-js) [![Windows Build status](https://ci.appveyor.com/api/projects/status/3u69uy9c0lsap3dr?svg=true
)](https://ci.appveyor.com/project/markandrus/video-quickstart-js)

This application should give you a ready-made starting point for writing your
own video apps with Twilio Video. Before we begin, we need to collect
all the config values we need to run the application:

* Account SID: Your primary Twilio account identifier - find this [in the console here](https://www.twilio.com/console).
* API Key: Used to authenticate - [generate one here](https://www.twilio.com/console/runtime/api-keys).
* API Secret: Used to authenticate - [just like the above, you'll get one here](https://www.twilio.com/console/runtime/api-keys).

## A Note on API Keys

When you generate an API key pair at the URLs above, your API Secret will only
be shown once - make sure to save this in a secure location, 
or possibly your `~/.bash_profile`.

## Setting Up The Application

Create a configuration file for your application:
```bash
cp .env.template .env
```

Edit `.env` with the configuration parameters we gathered from above.

Next, we need to install our dependencies from npm:
```bash
npm install
```

Now we should be all set! Run the application:
```bash
npm start
```

Your application should now be running at [http://localhost:3000](http://localhost:3000). Just enter
the name of the room you want to join and click on 'Join Room'. Then,
open another tab and join the same room. Now, you should see your own
video in both the tabs!

![screenshot of chat app](https://s3.amazonaws.com/com.twilio.prod.twilio-docs/images/video2.original.png)

## Examples

The project contains some use-case examples for the Twilio Video JS SDK. After running the application
by following the instructions above, go to [http://localhost:3000/examples](http://localhost:3000/examples)
to try them out.
