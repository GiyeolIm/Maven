## Apache Maven

Apache Maven is a software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project's build, reporting and documentation from a central piece of information.



## Maven’s Objectives

Maven’s primary goal is to allow a developer to comprehend the complete state of a development effort in the shortest period of time. In order to attain this goal, Maven deals with several areas of concern:

- Making the build process easy
- Providing a uniform build system
- Providing quality project information
- Encouraging better development practices



##### Making the build process easy

* While using Maven doesn’t eliminate the need to know about the underlying mechanisms, Maven does shield developers from many details.



##### Providing a uniform build system

- Maven builds a project using its project object model (POM) and a set of plugins. Once you familiarize yourself with one Maven project, you know how all Maven projects build. This saves time when navigating many projects.



##### Providing quality project information

- Maven provides useful project information that is in part taken from your POM and in part generated from your project’s sources. For example, Maven can provide:
  - Change log created directly from source control
  - Cross referenced sources
  - Mailing lists managed by the project
  - Dependencies used by the project
  - Unit test reports including coverage



## Providing guidelines for best practices development

Maven aims to gather current principles for best practices development and make it easy to guide a project in that direction.

For example, specification, execution, and reporting of unit tests are part of the normal build cycle using Maven. Current unit testing best practices were used as guidelines:

* Keeping test source code in a separate, but parallel source tree
* Using test case naming conventions to locate and execute tests
* Having test cases setup their environment instead of customizing the build for test preparation

Maven also assists in project workflow such as release and issue management.

Maven also suggests some guidelines on how to layout your project’s directory structure. Once you learn the layout, you can easily navigate other projects that use Maven.

While takes an opinionated approach to project layout, some projects may not fit with this structure for historical reasons. While Maven is designed to be flexible to the needs of different projects, it cannot cater to every situation without compromising its objectives.

If your project has an unusual build structure that cannot be reorganized, you may have to forgo some features or the use of Maven altogether.



## Where can I get the latest release?

You can download the release source from our [download page](https://maven.apache.org/download.cgi).

