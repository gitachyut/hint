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
          "vendor\\name_of_package\\":"src"
        }
      }
5) keep adding files using ( git add . or git add * ) and git commit n den make git push .. Keep doing it untill the package 
  creation over.
6) for adding webhook and services on github ->
    github -> settings -> webhook and services -> add -> pakagist -> add token  -> done
    ( this will help autoupdate in pakagist on any git commit )
7) For version set --- Github respective repo -> Releases -> Add -> version -> 0.0.1 -> done

Pakagist ---------------- To Install
1)composer require vendor/name_of_package

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

=====================================================================================================

Use Bower n Grunt 

Bower-----------------
1) npm install -g bower
bower init
bower install package-name --save

Grunt-----------------
1)npm install -g grunt-cli (for gloabally)
2)npm init
3)npm install grunt -S (locally inside the project directoy) to save in package.json file
4)make a Gruntfile.js --- eg;
            module.exports = function(grunt) {
            
              grunt.initConfig({
                jshint: {
                  files: ['Gruntfile.js', 'src/**/*.js', 'test/**/*.js'],
                  options: {
                    globals: {
                      jQuery: true
                    }
                  }
                },
                watch: {
                  files: ['<%= jshint.files %>'],
                  tasks: ['jshint']
                }
              });
            
              grunt.loadNpmTasks('grunt-contrib-jshint');
              grunt.loadNpmTasks('grunt-contrib-watch');
            
              grunt.registerTask('default', ['jshint']);
            
            };
5) den run grunt <specific task> command

------for my own pc java n android enviroment --------


++++++++++

export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_92.jdk/Contents/Home
export ANT_HOME=/Users/KrishnaDeka/Library/apache-ant-1.9.7
export ANDROID_HOME=/Users/KrishnaDeka/Library/Android/sdk
export PATH=${PATH}:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools

-----------------


GitHub -----------

1) to revert change -> git checkout -- filename
2) to checkout to previous commit -> git checkout shacode -- file/branch
3) must commit before u switch a branch
4) git reset --hard shacode // 
5) delete untack file -> git clean -f
6) ignore file -> using .gitignore file and git rm --cached filename
7) git checkout -b branch_name
8) to abort a merge confilct ->
    git merge --abort
9) git reset HEAD filename ->to untracked file
    

    
