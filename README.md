[//]: #@corifeus-header
  
[![NPM](https://nodei.co/npm/p3x-redis-ui.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/p3x-redis-ui/)

  [![Build Status](https://travis-ci.org/patrikx3/redis-ui.svg?branch=master)](https://travis-ci.org/patrikx3/redis-ui) 
[![Uptime Robot ratio (30 days)](https://img.shields.io/uptimerobot/ratio/m780749701-41bcade28c1ea8154eda7cca.svg)](https://uptimerobot.patrikx3.com/)

 


 
# 📡 P3X Redis UI that uses Socket.IO, AngularJs Material and IORedis with statistics, console - terminal, tree, dark mode, internationalization, multiple connections, web and desktop by Electron. v2018.12.18-8  

This is an open-source project. Star this repository, if you like it, or even donate! Thank you so much! :)

I run my own server with dynamic IP address, so, it may happen, that the server can not be reachable for about max 15 minutes, due to nature of the dynamic DNS. The server may also be unreachable, when I backup the SSD with Clonzilla (very rarely) or an electrical issue (but this should not happen again). When the server is down, please hang on for 15-30 minutes and the server will be back up.

All my domains (patrikx3.com and corifeus.com) could have errors, since I am developing in my free time. However, it is usually stable.

**Bugs are evident™ - MATRIX️**

### Node Version Requirement 
``` 
>=10.13.0 
```  
   
### Built on Node 
``` 
v11.4.0
```   
   
The ```async``` and ```await``` keywords are required.

Install NodeJs:    
https://nodejs.org/en/download/package-manager/    



# Description  

                        
[//]: #@corifeus-header:end

`p3x-redis-ui` is a new Redis GUI which can serve as a backend server or as a desktop application.
Some of the features are coming below.

👷 **The full complete version was created in 20 days in September of 2018.** 

## Development

It creates a package that allows you to compose `p3x-redis-ui-server` and `p3x-redis-ui-material` into one:

[Server on GitHub](https://github.com/patrikx3/redis-ui-server)  
[Client on GitHub](https://github.com/patrikx3/redis-ui-material)

By default, only English is created, but given all strings are from a `JS` file, it is very quick to spawn another language eg. German, French, Spanish etc ...

[English strings, easy to translate](https://github.com/patrikx3/redis-ui-material/blob/master/src/strings/en/strings.js)

This solution is not using REST at all, but instead uses Socket.IO 🤣, which is weird, but I like it, it is supposed to be more responsive, as there is no big overhead in the HTTP protocol.

### Reference for Socket.IO speed
http://blog.arungupta.me/rest-vs-websocket-comparison-benchmarks/

## Releases
https://github.com/patrikx3/redis-ui/releases  

## On ElectronJs  
(The GitHub versions are always instant to see than from ElectronJs Apps - delayed.)  
https://electronjs.org/apps/p3x-redis-ui  
    
## The test version
https://p3x.redis.patrikx3.com

![Redis themed - Statistics](https://cdn.corifeus.com/git/redis-ui/artifacts/preview-images/preview-1.png)

![Dark themed - JSON preview](https://cdn.corifeus.com/git/redis-ui/artifacts/preview-images/preview-2.png)

![Light theme - Settings](https://cdn.corifeus.com/git/redis-ui/artifacts/preview-images/preview-3.png)

## Features 

* Works as a backend

* Works as a desktop via Electron
  * I have 
    * Linux
    * Windows
    * macOS
      * I do not have the money to buy a macOS machine and build an Electron installer, but it would be very easy to do
* The error handling took careful (as much I can find errors)
* Starts with no settings without config, or setup your own config
* Able to create, test, save, delete multiple connections or a readonly connections setup, for shared usage
* Able to use the console and interact with Redis
* Online you are able to choose the tree separator, for example :, /, -, space etc... or even empty separator
* It is based on Redis-Commander and phpRedisAdmin
* You can select the database via console or the drop down, where the checked database is not empty, so you can always know which is filled
* Save button to save the db
* There is a performance penalty for this application, given it uses AngularJS `ng-repeat` for the tree component. The best is if your application uses nested keys (something:nested:good), then the tree will be fast, but, for example, Nextcloud uses about 500 keys inline and it can take 5 seconds to generate the tree.
  * Another solution is that instead of the : separator for your app, you can use the / separator. Then it will be much more responsive, see the settings tree separator 
  * A second solution is to use paging, the default paging is 50 keys
* Full statistics pages, can be useful
* This is just a New Kind on the Block in the Redis world, so, of course, there are advantages and disadvantages in the other Redis GUIs
* Dark - Dracula / light themes
* Search
  * Client side mode searching in keys - small key set
  * Server side mode searching in keys - large key set
  * Search mode
    * the search keys starts with a string key
    * the search keys includes a string in the key


# Start up with Electron

Please check out the releases section.


# Start up with a server or via a browser and NodeJs/NPM
[Start up with a server readme](artifacts/readme/start-up-server.md)

# Some description about the config file
[Some description about the config file readme](p3xrs.json)

# TODO
[The to do readme](todo.md) 

# Change log
[The change log readme](changelog.md) 


[//]: #@corifeus-footer

---

[**P3X-REDIS-UI**](https://pages.corifeus.com/redis-ui) Build v2018.12.18-8 

[![Like Corifeus @ Facebook](https://img.shields.io/badge/LIKE-Corifeus-3b5998.svg)](https://www.facebook.com/corifeus.software) [![Donate for Corifeus / P3X](https://img.shields.io/badge/Donate-Corifeus-003087.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=QZVM4V6HVZJW6)  [![Contact Corifeus / P3X](https://img.shields.io/badge/Contact-P3X-ff9900.svg)](https://www.patrikx3.com/en/front/contact) 


## P3X Sponsors

[IntelliJ - The most intelligent Java IDE](https://www.jetbrains.com)
  
[![JetBrains](https://cdn.corifeus.com/assets/svg/jetbrains-logo.svg)](https://www.jetbrains.com/) [![NoSQLBooster](https://cdn.corifeus.com/assets/png/nosqlbooster-70x70.png)](https://www.nosqlbooster.com/)

[The Smartest IDE for MongoDB](https://www.nosqlbooster.com)
  
  
 

[//]: #@corifeus-footer:end