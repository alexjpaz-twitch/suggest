# suggest

1. Get your channel name from your twitch.tv name

2. Create a discord webhook using the following guide

https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks

3. (Optional) Generate an OAuth token

4. Replace the variables in the URL below with your variables

https://github.com/alexjpaz-twitch/suggest?channel=CHANNEL_NAME&webhook=WEBHOOK_URL

5. Add the resulting URL as a hidden browser source in OBS

## Generating OAuth Token (Optional)

If you want your chatbot to respond when a user makes a suggestion you will need to create a token. Once you create a token you will need to add the `token` parameter to the URL.

1. Navtivate to https://dev.twitch.tv/console/apps/create

2. Enter a name for the application (e.g. MyUserNameRomShuffler)

3. Enter `https://twitchapps.com/tokengen/` for the *OAuth Redirect URLs* field

4. Click *create*

5. Click *manage* next to your newly created application

6. Copy the value in the *clientID* field 

7. Navigate to https://twitchapps.com/tokengen/

8. Enter your *clientID* from step 6

9. Enter the following scopes string in to the scopes field

```
channel:manage:redemptions channel:read:redemptions user:read:email chat:edit chat:read
```
