# shortcuts-turnout

## A Siri Shortcuts automation to handle link opening in fitting apps.

At the moment I'm not that sure how to publish it because it needs to be signed by Apple. I am not sure if uploading the signed Shortcut would be the ultimate foot gun.

## Roadmap

- settle on an updater
- deciding wether to crosshost on routinehub.co
- have it at least handle Twitter, Mastodon, Apollo and Reddit
- make it modular so community can plug into it

## modularity concept

- handle updater and split up url
- let it run other shortcut
- that shortcut gets a part of the url and checks if it can handle that service
- if not the next shortcut is run
- if it can, shortcut will manipulate url and passes it back to main shortcut to open url

In theory, this will assure that, if named correctly, one could add services without ever needing to modify the original Shortcut because that one simply runs other Shurtcuts and receives ther output.
