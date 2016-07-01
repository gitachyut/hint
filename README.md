# hint
Pakagist ---------------- To Create
1)initialize the github repo .
2)clone repo to desktop.
3)initialize composer -> composer init
4)make composer.json
    -> vendor/name_of_package
    -> set the name_of_package as github repo name
    -> den make  src directory inside name_of_package dir
    -> composer.json file config for autoload
    "autoload":
      {
        "psr-4":{
          "vendor\\name_of_package\\":"scr"
        }
      }
5) keep adding files using ( git add . or git add * ) and git commit n den make git push .. Keep doing it untill the package 
  creation over.
6) for adding webhook and services on github ->
    github -> settings -> webhook and services -> add -> pakagist -> add token  -> done
    ( this will help autoupdate in pakagist on any git commit )
7) For version set --- Github respective repo -> Releases -> Add -> version -> 0.0.1 -> done

Pakagist ---------------- To Install
1) composer composer require vendor/name_of_package

================================================================================================================

NPM -------------------- To Create
1)Make the directory named as the Node package (akd-js)
2)nmp init 
3)make the package.json
4)add codes
5)npm adduser
6)npm publish
NPM -------------------- To install
1)nmp install akd-js
NPM -------------------- To use
1)var md = require('akd-js');
NPM -------------------- To Uninstall
1)npm uninstall
NPM -------------------- To version chnage
1)change the version number on package.json file and den npm publish


  
    
