## Welcome
Welcome to Sovereign Fronts, an open-source and completely free real-time grand strategy game! Sovereign Fronts aims to get rid of the annoying microtransactions that plague many known real-time browser-based grand-strategy games, as well as making it a more customizable experience by featuring integrated modding.

## Current State
In its current state, Sovereign Fronts is NOT ready to use.

## Q&A
### Why did you make Sovereign Fronts?
I'm bad at writing Q&As, and accidentally already answered that above, TLDR: I don't like P2W.
### What is planned?
Currently, the following ideas have landed on the "things I wish to manifest into reality" list:
- Open source game server software that anyone can download and host with minimal system requirements
- Stable client that for all mainstream operating systems & devices
- Auth servers, free account creation
- Stable mod API
### How will the mod API work?
The current plan is to make mods a basic part of the server. To ensure that the API is extensive enough, the main game will be just a skeleton while the main game units and mechanics are going to be written as a mod called `core`!
### Why do you use bun for everything?
Bun is pretty darn fast
### Will you rewrite the server in Rust?
no.
### Will you update the codebase to use Typescript?
Possibly at some point, although this is not one of my main goals in the current moment.
### Can one contribute?
Yes! Anyone is welcome to contributing following the issues template. I myself am not a particularly good programmer, so I welcome any improvements.
### How long do you plan to keep development?
One thing I wish to avoid, at least on paper, is constantly updating the server software, leaving no room for a stable moddable version. This happens a lot in other games, causing modders to stay on a specific old version, understandably refusing to update the mod for every single api change a game updates to. Therefore I only plan to update so many times until I deem that the server is good enough to use and that the mod api is extensive enough.
### Why are you planning to implement an auth system?
Ultimately, without any account system, whitelists and blacklists would only work so long nobody shares the server ip. So in order to enforce bans on fully public servers, a simple auth system tied to accounts (that will be free, forever) makes this somewhat more enforceable.<br>And while accounts being free makes doesn't stop a banned player from coming back with another account it does make it harder and discourages it. And this also gives me the opportunity to write a simple `ip-ban` mod to use as an example in the documentation :)
### Will you ever use the auth server to ban servers globally?
**No.** While I encourage everyone to follow the **Server Usage Guidelines (SUG)** and the **End User License Agreement (EULA)**, the open-source nature of Sovereign Fronts means I will not and can't use the authentication server to ban servers globally. Moderation is the responsibility of individual server hosts, and players are free to decide which servers they join. Therefore auth servers will only be used to ban timed out users, or players suspected of hacking.
### Can I turn off authentication?
By disabling the `auth` in the server config you can disable player authentication on join, in case of authentication server outages.
