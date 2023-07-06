# get-going-with-gradle
[Gradle](https://gradle.org/) is a build automation tool written in [Groovy](https://groovy-lang.org/). It's very concise and lightning fast, as there is no XML configuration (unlike [Maven](https://maven.apache.org/))
Gradle makes building and running applications very easy and there is no need for people using your projects to have Gradle installed. Gradle wrapper comes bundled with the project.

## Key concepts of Gradle
**build.gradle** is the Gradle build script file, which is equivalent to Maven's `pom.xml` and it normally lives at the top level of your project. It consists of all the details about plugins, build metadata, repositories, and dependencies.

**tasks** define a unit of work that is invoked from the command line when we send commands like `./gradlew build`. Tasks have dependencies on other tasks, which leads to the creation of _task graph_.
We can also create our own tasks.

**wrapper** is the script used to invoke Gradle and run tasks. It contains the specific version of Gradle for your project.
No local Gradle installation is required for anyone building your project.

---

## How Gradle works with Java
Gradle _Java plugin_ provides us with all the tasks that are required for our Java project. Some tasks included in the Java plugin:
- Compiling classes: `./gradlew compileJava`
- Managing resources: `./gradlew processResources`
- Package into jar file: `./gradlew jar`
- Easily run tests: `./gradlew test`

---
## Source
[Get Going with Gradle | Gradle Hero](https://gradlehero.com/courses/get-going-with-gradle/)
