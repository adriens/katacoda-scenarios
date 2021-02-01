# SDKMAN Management tasks

# Upgrade Java, Kotlin, maven

To see what is currently out of date for a Candidate on your system: 

```
sdk upgrade
```{{execute}}


# Update SDKMAN

Installs a new version of SDKMAN! if available :

```
sdk selfupdate
```{{execute}}

# Broadcast Messages

Get the latest SDK release notifications on the command line: 

```
sdk broadcast
```{{execute}}

# Get updates

Periodically SDKMAN! requires a refresh to become aware of new (or removed) candidates. When candidate metadata has potentially grown stale, a warning is displayed with instruction on how to update. By simply running the following command, the candidate cache will be refreshed and new candidates will become available for installation: 

```
sdk update
```{{execute}}