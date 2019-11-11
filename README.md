# IBM Client Developer Advocacy App Modernization Series

## Simple app to demo HTTPSession replication in WebSphere Liberty on OpenShift

This small Java EE app supports the lab [HTTP Session Replication Lab for the App Modernization Dojo](https://github.com/IBMAppModernization/app-modernization-session-replication-openshift) on OpenShift.

You'll use an Open Source JCache provider to provide the implementation of the JCache support that is included in WebSphere Liberty.

This app can be used with the following JSR 107 providers:
- [Infinispan](https://infinispan.org) - Open Source, subset of [Red Hat Data Grid](https://www.redhat.com/en/technologies/jboss-middleware/data-grid) (comes with [IBM Cloud Pak for Applications](https://www.ibm.com/cloud/cloud-pak-for-applications))
- [Hazelcast](https://github.com/hazelcast/hazelcast) - Open Source - upstream version of Hazelcast's commercial offering

### Building the app

You'll need the following to build the app from source:
- A Java 8 (or later) JDK
- [Maven 3.3 (or later)](https://maven.apache.org/download.cgi)

To build the app from source  run the following command from the top level folder of a clone of this repo :
    ```
    mvn clean package
    ```

This will create the app's *.ear* file in the **target** subfolder.

### Running the app

Refer to the [lab instructions](https://github.com/IBMAppModernization/app-modernization-session-replication-openshift) in the accompanying lab exercise to run the app on OpenShift.
