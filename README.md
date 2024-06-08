# OSINT namecheckers list

A list of tools to search accounts by username with pros and cons.

## Table of Contents
- [Scripts](#scripts)
- [APIs](#apis)
- [OSINT Online Tools](#osint-online-tools)
- [Branding Tools](#branding-tools)
- [Toolkits](#toolkits)
- [Useful Links](#useful-links)

### Scripts

#### [Sherlock](https://github.com/sherlock-project/sherlock)
* hunts down social media accounts by username across around 400 social networks
* has web-cli deployments 👍
* batch search 👍
* tor & proxy support 👍
* alexa top ranking 👍
* adding custom sites & rules
* csv reports
* false positives

#### [Maigret](https://github.com/soxoj/maigret)
* sherlock fork, all its pros and cons so
* 3100+ sites 👍
* profile pages parsing and extracting personal info, links to other profiles, etc. 👍
* recursive search by new usernames found 👍
* searching by countries and categories by tags 👍
* very few false positives 👍
* censorship and captcha detection

#### [social-analyzer](https://github.com/qeeqbox/social-analyzer)
* 1000+ sites 👍
* web interface 👍
* multilayers detections (OCR, normal, advanced & special) 👍
* metadata extraction

#### [WhatsMyName](https://github.com/webbreacher/whatsmyname)
* username enumeration on around 600 various websites
* adding custom sites & rules

#### [DetectDee](https://github.com/piaolin/DetectDee)
* hunt down social media accounts by username, email or phone across social networks
* 372 sites
* screenshots 👍

#### [nexfil](https://github.com/thewhiteh4t/nexfil)
* 350 sites
* fast, lookup can complete under 20 seconds

#### [Snoop](https://github.com/snooppr/snoop)
* sherlock fork, all its pros and cons so
* 271 sites in demo version, around 4200+ sites in full paid version
* country ranking & filtering 👍
* html and csv reports
* difficult to install and use 🚫

#### [thorndyke](https://github.com/rly0nheart/thorndyke)
* Lightweight username enumeration tool
* checks the availability of a specified username on over 200 websites
* no longer supported 🚫

#### [sagemode](https://github.com/senran101604/sagemode)
* simple and effective OSINT username search tool
* around 150 sites

#### [Userrecon](https://github.com/wishihab/userrecon)
* finds usernames across over 75 social networks 
* original repository is unavailable
* no longer supported 🚫

#### [NicknameFinder](https://github.com/restanse/NicknameFinder)
* 45 sites in database

#### [Gideon](https://github.com/YouVBeenHacked/gideon)
* 44 sites in database

#### [Arina-OSINT](https://github.com/AlexC-ux/Arina-OSINT)
* 42 sites in database

#### [netizenship](https://github.com/rahulrajpl/netizenship)
* 38 sites in database

#### [Search4](https://github.com/0xknown/Search4)
* 35 sites in database
* small and fast

#### [Socialscan](https://github.com/iojw/socialscan)
* checks for **email** and username usage on 12 platforms 
* uses api, not a direct userpage link 👍

#### [sherlock-go](https://github.com/mesuutt/sherlock)
* faster and minimal implementation of sherlock written in Go
* no longer maintained

#### [Investigo](https://github.com/tdh8316/Investigo)
* can take screenshots with headless chromium 👍
* uses sherlock database

#### [recon-ng](https://github.com/lanmaster53/recon-ng/)
* have a profiler module using WhatsMyName database

#### [SocialPath](https://github.com/woj-ciech/SocialPath)
* track users across 10 popular social media platforms
* extract details info from 4 platforms
* web interface

#### [tookie-osint](https://github.com/Alfredredbird/tookie-osint)
* hunts down social media accounts
* 261 sites in the database
* has a WebUI
* has some false positives (≈20%)
* difficult to install and use 🚫

### APIs

#### [Social Scanner](https://rapidapi.com/hailbytes-hailbytes-default/api/social-scanner/)
* 996 social networks with links to each profile in JSON
* implementation of social-analyzer

### OSINT Online Tools

Websites to search accounts from your browser. Usually there are advertising and logging of requests.

#### [WhatsMyName](https://whatsmyname.app/)
* username enumeration on around 250 various websites
* web-gui for searching for [WhatsMyName](https://github.com/webbreacher/whatsmyname) data
* rich filtering by category

#### [Usersearch](https://usersearch.org/)
* 120 popular websites, 100+ generic forums , 6 dating sites and crypto forums

#### [analyzeid username checker](https://analyzeid.com/username/)
* more than 80 social sites
* gather information on the taken username and get a summary of who the person is 👍

#### [iDCrawl](https://www.idcrawl.com/username)
* 12 sites

#### [suIP.biz](https://suip.biz/ru/?act=sherlock)
* yet another sherlock online

#### [Usersherlock](http://usersherlock.com/)
*website is down*

## Branding tools

The main goal of branding tools is to search for the availability of usernames on social platforms and sites, not to search for users.
These tools are used by marketers to brand securing and promotion.
One of the features of such tools is a domain name search similar to a search by username.

#### [Knowem](https://knowem.com/) (updated Checkusernames)
* searches over 550 popular social networks, over 150 domain names
* 15 categories of social networks
* trademarks checks

#### [Namecheckup](http://namecheckup.com/)
* checks social media username availability over 270+ social networks and sites and check 45 TLDs

#### [InstantUsername](https://instantusername.com/)
* checks username availability for more than 100 social media sites
* [open source](https://github.com/instant-username-search) 👍

#### [Checkusernames](https://checkusernames.com/)
* checks the use of your brand or username on 160 Social Networks

#### [CHECKUSER.org](https://checkuser.org)
* checks popular domains and 52 social media sites

#### [Namechk](https://namechk.com/)
* finds an available username over 96 sites and 36 domain names

#### [Namecheckr](https://www.namecheckr.com/)
* checks domain & social username availability across 38 networks and 17 TLDs

#### [Checkerapi](https://app.swaggerhub.com/apis/checker/api)
* checks 6 services for username availability
* [open source](https://github.com/checker/api) 👍


## Toolkits

- [One-plus OSINT Toolkit](https://one-plus.github.io/EmailUsername)

- [Aware-online](https://www.aware-online.com/en/osint-tools/username-search-tool/)

- [Lullar](https://com.lullar.com/)

## Useful links

* [OSINT Handbook September 2020 (see "Username Check")](https://i-intelligence.eu/uploads/public-documents/OSINT_Handbook_2020.pdf)
* [Nixintel's OSINT Resource List (see "Usernames & People Searches"](https://start.me/p/rx6Qj8/nixintel-s-osint-resource-list)
* [What’s wrong with namecheckers?](https://soxoj.medium.com/whats-wrong-with-namecheckers-981e5cba600e)
