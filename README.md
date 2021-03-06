![KDR Banner](https://github.com/JackMD/KDR/blob/master/meta/KDR.png)
# KDR

### A KDR, Kill Death Ratio  plugin for your Minecraft Bedrock Server. Allows you to keep track of players kills, deaths and kill to death ratio.

### Features
 - Keep track of players kills.
 - This plugin is an update to JackMD's KDR
 - Keep track of players deaths.
 - Keep track of players kill to death ratio.
 - Two storage ways are supported:
        - Yaml
 - Simple and neat api for developers.

### How to setup?
 - Put the plugin in your plugins folder.
 - Start and then stop the server.
 - Edit the `confiig.yml` to suit your needs.
 - Restart and enjoy...
 
### API

KDR provides a simple way api for the developers.<br />

First of all you need to get the `KDR` Instance. 
```php
KDR::getInstance();
```

- To get the kill count of a player:
```php
KDR::getInstance()->getProvider()->getPlayerKillPoints($player);
```

- To get the death count of a player:
```php
KDR::getInstance()->getProvider()->getPlayerDeathPoints($player);
```

- To get the kill to death ratio of a player:
```php
KDR::getInstance()->getProvider()->getKillToDeathRatio($player);
```

And thats about it. Let me know if I missed out on something.
