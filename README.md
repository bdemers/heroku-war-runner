Quick Test idea for Heroku buttons, for Maven Submodules
========================================================

Deploy me!

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/bdemers/heroku-wrapper-test&env\[GROUP_ID\]=com.stormpath.shiro&ARTIFACT_ID=stormpath-shiro-servlet-example)


There is the idea:
Heroku requires an app.json at root of a git repo (not a bad requirement), but we (and other projects) have a lot of examples in 
a Maven sub-module `examples`.  This repo will wrap any Maven `war` project and download the latest release and run it with Jetty.

Button format:

``` markdown
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/bdemers/heroku-wrapper-test&env\[GROUP_ID\]=<maven-groupId-here>&ARTIFACT_ID=<maven-artifactId-here>)
```

Where `<maven-groupId-here>` is your groupId, and `<maven-artifactId-here>` is your artifactId.


