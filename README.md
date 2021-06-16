You will need a Millicast account for the example.

You can create account here https://millicast.com/

1.This player includes a mute image overlay.

2.Offline reconnect for network disconnect.

3 Viewer count.

4.Message overlay.



1. In your Millicast portal(+) Create a new stream label
Select the API Tab.
You will need the following to test the player.
AccountId and Streamname

You can test the player right here.

DEMO:

https://rnkvogel.github.io/Millicast-Player/

Note secure token is not needed if youdid not enable it.

Place the folder on your website 

https://YOUR_WEB_SITE/player/?id=ANY_NAME

Customize the player as desired.

If you secured your stream requiring a token.
https://reqbin.com/curl


curl -H "Authorization: Bearer YOUR_API_CODE_FROM_PORTAL_ACCOUNT_TAB" \
      -H "Content-Type: application/json" \
     https://api.millicast.com/api/subscribe_token/ \
     -d '{"subscribeRequiresAuth": true, "label": "STREAM_LABEL", "streams": [{"streamName": "STREAM_NAME"}]}'

Set up responsive iframe
<div class="container">
  <iframe class="responsive-iframe" src="YOURSITE.COM/playerpath.></iframe>
</div>
