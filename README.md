# JSpy
**JSpy** is a tool that displays the component properties of any java Swing application in the simplest way. To automate Swing applications, You generally need to venture into the application's sources to retrieve the component's properties. That's very time consuming and frustrating or even impossible. Using JSpy all You need to do to get the component's properties is to hover the coursor over the component.
![](https://raw.github.com/stasiek/temp/master/doc/img/jspy_big.png "JSpy Big")

## Dependencies
**JSpy** is operating system independent — it just needs Java 6 or newer.

## Building from sources
We’ll go with IntelliJ for compiling this
First clone the repository

```sh
git clone github.com/nokia/JSpy.git
```

Open cloned JSpy directory in IntelliJ. Go to File\>Project Structure\>Artifact Add a jar artifact, point it to manifest file and set `spyGui.SpyMain` as Main Class
![](https://raw.github.com/stasiek/temp/master/doc/img/project_structure.png "IntelliJ Project Structure")

To compile build the jar Artifact with attached manifest.
![](https://raw.github.com/stasiek/temp/master/doc/img/build_artifacts.png "Build Artifacts")

## Running
To execute jSpy call it from the console:
```sh
java -jar JSpy.jar
```

## Usage
When started go into File \> Execute Command


Execute Command: `javaws C:\path\to\file.jnlp`

To run the application by it's java class remember to add it's jar's path (the path **musn't** contain spaces) to the `CLASSPATH` environment variable.

Execute Command: `java Package.ClassName`
