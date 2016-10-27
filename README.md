Stormpath War Jetty Runner for Heroku
=====================================

Deploy A Maven based war artifact to Heroku.  This project is intended to enable simple way to bootstrap an example application to Heroku.
The pom.xml will download a war artifact and run that war with Jetty.

Example:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/bdemers/heroku-war-runner&env\[GROUP_ID\]=com.stormpath.shiro&env\[ARTIFACT_ID\]=stormpath-shiro-servlet-example)


Heroku requires an app.json at root of a git repo (not a bad requirement), but we (and other projects) have a lot of examples in 
a Maven sub-module typically named `examples`.  This repo will wrap any Maven `war` project and download the latest release and run it with Jetty.

Button format:

``` markdown
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/bdemers/heroku-war-runner&env\[GROUP_ID\]=<maven-groupId-here>&env\[ARTIFACT_ID\]=<maven-artifactId-here>)
```

Where `<maven-groupId-here>` is your groupId, and `<maven-artifactId-here>` is your artifactId.

Supported URL parameters:

| Parameter | Default Value | Description |
| --------- | ------------- | ----------- |
| `env[GROUP_ID]` | N/A | War artifact's group ID |
| `env[ARTIFACT_ID]` | N/A | War artifact's ID |
| `evn[VERSION]` | [0.0.0,) | War artifact's version |