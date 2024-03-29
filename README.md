# Summary

In the spirit of pihole users and creators, I was inspired to create my own blocklists, and decided to share them with the world to help contribute to the community. Feel free to copy these lists and use them in your own list project, or however you wish, no need to credit me! All I care about is that this project helps somebody (see the [license](/LICENSE)).

# Disclaimer

The lists contained here are provided as is, with no warranty as to their accuracy. It is your responsibility to whitelist/blacklist as you see fit for your needs and your enviroment. These lists are provided free of charge, are open for use by anyone, and are maintained by myself in my spare time.

These lists are collections of domains I have come across in my time on the interwebs or seen in forums or other places, therefore these are not perfectly curated and vetted lists, however I try to do my best to avoid false positives and inaccuracies in all cases. I also do my best to credit sources as applicable. Credits, if any, will be listed in the commit messages of relevant commits.

# How it works

All lists are hosted at my domain `blocklists.kitsapcreator.com`. This domain uses Cloudflare [R2](https://www.cloudflare.com/products/r2/) (S3-compatible object storage) and [CDN](https://www.cloudflare.com/cdn/) for fast global delivery.

Updates are synced to R2 via a Github Action that uses [rclone](https://rclone.org/) to upload new file versions. Feel free to duplicate what I've put together here if you need a similar Github Action.

Feel free to ping the lists as often as you wish; the more the merrier.

# Start Using

All lists are accessible using `https://blocklists.kitsapcreator.com/<file-name-here>.txt`. Just put the file path after the domain.

## Standard Lists

### General

- https://blocklists.kitsapcreator.com/general.txt

### Ads

- https://blocklists.kitsapcreator.com/ads.txt

### Adult Content

- https://blocklists.kitsapcreator.com/adult.txt

### Malware/Malicious

- https://blocklists.kitsapcreator.com/malware-malicious.txt

### Scams/Spam

- https://blocklists.kitsapcreator.com/scam-spam.txt

## Social Lists - Facebook/Meta and related properties

### Facebook:

- https://blocklists.kitsapcreator.com/social/facebook/facebook.txt

### Facebook Messenger

- https://blocklists.kitsapcreator.com/social/facebook/messenger.txt

### Instagram

- https://blocklists.kitsapcreator.com/social/facebook/instagram.txt

### Whatsapp

- https://blocklists.kitsapcreator.com/social/facebook/whatsapp.txt

## Social Lists - Other properties

### Reddit

- https://blocklists.kitsapcreator.com/social/reddit.txt

### Snapchat

- https://blocklists.kitsapcreator.com/social/snapchat.txt

### Tiktok

- https://blocklists.kitsapcreator.com/social/tiktok.txt

### Twitter/X

- https://blocklists.kitsapcreator.com/social/twitter.txt

## Game Scams (Discord scams, etc)

- https://blocklists.kitsapcreator.com/gaming/game-scams.txt

## Microsoft Exchange autodiscover flaw

Learn more about this in the [readme](autodiscover/readme.md).

- https://blocklists.kitsapcreator.com/autodiscover/autodiscover-tlds.txt

## Combined Lists

### Block all General items

_Combines Ads, Adult, Autodiscover Flaw, Malware/Malicious, Game Scams, and Scams/Spam_

- https://blocklists.kitsapcreator.com/general-combined.txt

### Block all supported social media

_Combines Facebook, Reddit, Snapchat, Tiktok, and Twitter/X_

- https://blocklists.kitsapcreator.com/social-combined.txt

## One and Done

Want one list to rule them all? Look no further. This file has ALL domains from every list in this repo. Handle with care!

- https://blocklists.kitsapcreator.com/all-lists.txt

# Contribute

1. Start by searching lists for the domains you wish to propose additions to avoid duplicates.
2. Fork the repo, make your changes, then create a pull request so changes can be discussed.

- Use these same steps can be used when proposing subtractions.
- Use the Issues tab to report false positives and other problems.
- Before creating an issue, look to see if your problem has already been raised by someone else to prevent duplicate issues.
- If you don't want to edit files and create a pull request yourself, simply create an issue with the domain(s) that you propose to add along with what list you propose to put them in.

# Tips and Tricks

- Use forks to regulate list updates if you don't want frequent changes. In this way you control when changes reach your setup.
- Consider using indvidual lists instead of the combined lists if you want more control over what is blocked.

# Notes

This project is not a place to help you setup, configure, or troubleshoot your pihole or network setup. It is assumed that you know the basics of setting up and using pihole and related technologies associated with it, including how to add blocklists to pihole. If you need help setting up and configuring your pihole, visit the [Official Pi-hole website](https://pi-hole.net/), [forum](https://discourse.pi-hole.net/), [subreddit](https://www.reddit.com/r/pihole/), and [Github Project](https://github.com/pi-hole/pi-hole).

If you have any questions about this project, open an issue and let's have a discussion!
