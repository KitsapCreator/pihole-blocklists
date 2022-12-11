## Summary
In the spirit of pihole users and creators, I wanted to create my own blocklists. I decided to share them with the world to help contribute to the overall community. On that note, welcome!

## Disclaimer
The lists contained here are provided as is, with no warranty as to their accuracy. It is your responsibility to whitelist/blacklist as you see fit for your needs and your enviroment. These lists are provided free of charge, are open for use by anyone, and are maintained by myself in my spare time. These lists are collections of domains I have come across or seen in forums or other places, therefore these are not perfectly curated and vetted lists, however I try to do my best to avoid false positives and inaccuracies in all cases.

# Getting Started

## Start Using
All lists are accessible using `https://blocklists.kitsapcreator.com/<file-name-here>.txt`. Just put the file path after the domain.

This domain uses Cloudflare [Pages](https://pages.cloudflare.com/) and [CDN](https://www.cloudflare.com/cdn/) for fast global delivery. Feel free to pull updates as often as you wish; the more the merrier.

## Additional Sources/Mirrors
You can also use [JSDelivr](https://jsdelivr.com) instead if you wish. Use the following to select an individual file: `https://cdn.jsdelivr.net/gh/KitsapCreator/pihole-blocklists/<file-name-here>.txt`.

## Combined Lists
The following is two merged lists - one for all supported social platforms (Facebook, Tiktok, Reddit, etc.) and one for all general lists (Ads, Malware, Scams, etc.).

## Social List
My domain:\
`https://blocklists.kitsapcreator.com/social/social-combined.txt`

JSDelivr:\
`https://cdn.jsdelivr.net/gh/KitsapCreator/pihole-blocklists/social/social-combined.txt`

## General List
My domain:\
`https://blocklists.kitsapcreator.com/social/general-combined.txt`

JSDelivr:\
`https://cdn.jsdelivr.net/gh/KitsapCreator/pihole-blocklists/social/general-combined.txt`

## One and Done
Want one list to rule them all? Look no further.

My domain:\
`https://blocklists.kitsapcreator.com/all-lists.txt`

JSDelivr:\
`https://cdn.jsdelivr.net/gh/KitsapCreator/pihole-blocklists/all-lists.txt`

## Contribute
1. Start by searching lists for the domains you wish to propose additions to avoid duplicates.
2. Fork the repo, make your changes, then create a pull request so changes can be discussed.
* Use these same steps can be used when proposing subtractions.
* Use the Issues tab to report false positives and other problems.
* Before creating an issue, look to see if your problem has already been raised by someone else to prevent duplicate issues.
* If you don't want to mess around with editing files and creating a pull request yourself, simply create an issue with the domain(s) that you propose to add along with what list you propose to put them in.

## Tips and Tricks
* Use forks to regulate list updates if you don't want frequent changes. In this way you control when changes reach your setup.

# Notes
This project is not a place to help you setup, configure, or troubleshoot your pihole or network setup. It is assumed that you know the basics of setting up and using pihole and related technologies associated with it, including how to add blocklists to pihole. If you need help setting up and configuring your pihole, visit the [Official Pi-hole website](https://pi-hole.net/), [forum](https://discourse.pi-hole.net/), [subreddit](https://www.reddit.com/r/pihole/), and [Github Project](https://github.com/pi-hole/pi-hole).

If you have any questions about this project, open an issue and let's have a discussion!
