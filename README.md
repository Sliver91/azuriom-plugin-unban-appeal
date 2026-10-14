# Unban Appeal

[Lire en français](README.fr.md) · **Limeris.fr by Sliver91** · [limeris.fr](https://limeris.fr) · [Discord](https://discord.gg/4kV8pgC3Ck)

An [Azuriom](https://azuriom.com) plugin: an appeal form tied to the player's sanction, with a discussion thread between the player and the staff.

![Appeal page with the discussion thread](docs/appeal.jpg)

> **Showcase only.** This repository presents the plugin: it does not contain the plugin files. **Coming soon** on the Azuriom Market. Follow the news on [Discord](https://discord.gg/4kV8pgC3Ck).

## Screenshots

| | |
|---|---|
| ![Appeal home page](docs/home.jpg) **Appeal home page**: how it works, your appeals | ![New appeal form](docs/form.jpg) **New appeal** for an in-game or Discord sanction |
| ![Website ban form](docs/site-ban.jpg) **Website ban**: appeal without logging in | ![Light mode](docs/appeal-light.jpg) **Light mode**, follows the installed theme |
| ![Admin list](docs/admin-appeals.jpg) **Admin: appeal list** filtered by status | ![Admin appeal](docs/admin-appeal.jpg) **Admin: appeal** with internal notes and decision |
| ![Admin settings](docs/admin-settings.jpg) **Admin: settings** | ![On a phone](docs/mobile.jpg) **On a phone** |

<sub>Screenshots taken with the free Haze Limeris theme.</sub>

## What players see

- **Two paths**, depending on the sanction:
  - **Website ban**: the player cannot log in anymore. They send their appeal with the username and email address of their account, and the appeal is linked to the Azuriom ban.
  - **Sanction in game or on Discord** (ban, mute, other): the player is logged in and describes their sanction.
- **One appeal per sanction**, and only one appeal at a time.
- **A discussion thread** with the staff, on the page of the appeal.
- **Progress** in three steps: appeal sent, review by the staff, decision.
- **A private tracking link** to keep: it lets the player follow the appeal without being logged in.
- **A waiting time before a new appeal** after a refusal, shown with the date.

The page uses the font, colors and light or dark mode of the installed theme, whatever it is.

## What the staff sees

- The list of appeals, filtered by status, with the ones waiting for an answer on top.
- For each appeal: the player's explanation, the sanction, the discussion thread and the other appeals of the same player.
- **Reply to the player** or **internal note** the player never sees.
- **Accept** or **refuse**, with a message. Accepting can lift the website ban at the same time. A refusal can be final.
- **Discord notification** for each new appeal, player reply and decision.

## Requirements

- Azuriom 1.2 or newer.
- No other plugin is needed.
- Works with every game supported by Azuriom.


## Settings

Everything is in **Unban appeals > Settings**.

### Page

- **Page title** and **sentence under the title**.
- **Reminder shown above the forms**: optional. For example what a good appeal contains, or what gets an appeal refused.

### Appeal rules

- **Waiting time before a new appeal**: in days, after a refusal (14 by default). 0: no waiting. In any case, one appeal at a time.
- **Minimum length of the explanation**: in characters (50 by default), to avoid one-line appeals.
- **Sanctions players can contest**: website ban, game ban, game mute, Discord sanction, other sanction. Uncheck the ones that do not apply to your server.

### Discord notification

1. In Discord, open **Channel settings > Integrations > Webhooks**, create a webhook and copy its address.
2. Paste it in **Webhook address**.
3. Optional: enter the identifier of the **role to mention** on each new appeal (right click on the role > Copy ID, with developer mode on).
4. Choose whether player replies in the thread are sent too. New appeals and decisions always are.

## Handling an appeal

Open **Unban appeals > Appeals**, then an appeal.

1. **Start the review** tells the player their appeal is being read. Replying to the player does it automatically.
2. **Reply** in the thread to ask a question. Turn on **Internal note** to leave a word for the rest of the staff, invisible to the player.
3. **Accept** or **Refuse**, with an optional message shown to the player.
   - For a website ban, the **Lift the website ban when accepting** box takes care of it.
   - For a sanction in game or on Discord, lift it yourself where it was given.
   - **Final refusal** prevents any new appeal for this sanction.
4. **Reopen the appeal** cancels a decision.

A logged-in player gets a notification on the website for each reply and for the decision.

## Website bans, in detail

This path uses the Azuriom bans (**Users > Bans**). A banned account cannot log in anymore, so:

- the player proves the account is theirs with its username and email address. The email is neither shown nor stored in the appeal;
- the error message is the same whether the username, the email or the ban is wrong, so nothing is revealed about accounts;
- the number of attempts is limited;
- the tracking page is reached through a secret link the player must keep. It is not indexed by search engines.

## Who can manage the plugin

Administrators, and any role you give the **Handle unban appeals** permission in **Users > Roles**.



## Support

A question, a bug, an idea: join the [Discord](https://discord.gg/4kV8pgC3Ck).

## Translations

English and French are included.

---

Unban Appeal · **Limeris.fr by Sliver91**
