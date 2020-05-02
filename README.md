### What is a stack ?

Set of metadata, artifacts and example code needed to develop an application. 
The scope of AppStaK goes beyond the traditional software stack and covers development 
and GitOps activities.

#### What information does a stack have ?

A stack contains the following information with respect to an application 
that is associated with a stack:

* How to turn the application into a container(s)
* How to run the application
* How to run tests
* How to debug the application
* How to deploy the application
* Pipeline(s)
* Sample application(s)


#### How does one define a stack ?

A stack author defines a stack by specifying the following information in a devfile YAML file.

* Metadata for setting up a container-based developer workspace for developing an app with the 
specific stack.
* Commands for compiling the app in a container in the developer workspace. 
Example, `mvn package`.
* Commands for running the app in a container in the developer workspace. 
Example, `java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App` 
* Guidance for building an image from the app's source code.
* Guidance for deploying the above image as a container on Kubernetes.