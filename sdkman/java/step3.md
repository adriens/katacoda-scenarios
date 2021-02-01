# Install from Java.net

Let's say we want to use Java 8 from Java.net.

First, pick the Java distriubution you want:

```
sdk list java
```{{execute}}

Then install `java 8.0.282-open`:

```
 sdk install java 8.0.282-open
```{{execute}}

... and set if by default by hitting `ENTER`.

Next, test you are now using this latest one :

```
java -version
```{{execute}}

Pay good attention to :

- distributor
- java version

Check all the installed versions and the one you are currently using :

```
sdk list java
```{{execute}}

# Install Java 11 from Java.net

As seen previsously, just :

```
 sdk install java 11.0.10-open
```

... and set if by default by hitting `ENTER`.

Test your java environment now :

```
java -version
```{{execute}}

