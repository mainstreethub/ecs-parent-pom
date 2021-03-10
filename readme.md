## ecs-parent-pom
This pom adds the ability to easily build a Docker image from the primary
artifact of a maven build.  This pom encapsulates all of the info necessary to
build as well as publish the Docker image into Main Street Hub's private Docker
registry (hosted in ECR).

**Note:** it is assumed that the primary artifact of the maven build is a single
fat jar that contains all of it's dependencies as well as a manifest specifying
a main class.

### Releases

#### 1.5.0
* Upgraded parent POM, `com.mainstreethub:parent-pom`, to 1.6.6

#### 1.4.0
* Upgraded `io.fabric8:docker-maven-plugin` to 0.26.0

#### 1.3.6
* Upgraded parent POM, `com.mainstreethub:parent-pom`, to 1.6.3

#### 1.3.5
* Upgraded docker-maven-plugin to 0.22.1

#### 1.3.2
* Enable `skipExtendedAuth` for `docker-maven-plugin`

#### 1.3.1
* Broken build, do not use.

#### 1.3.0
* Upgraded parent POM, `com.mainstreethub:parent-pom`, to 1.6.0

#### 1.2.0
* Upgraded `io.fabric8:docker-maven-plugin` to 0.20.1

#### 1.1.1
* Updated label `app` to `application`
* Updated label `app_version` to `version`

#### 1.1.0
* Updated base image from docker.io/java to docker.io/openjdk.
* Made base image configurable for image build.
* Added labels to Docker image for application (app) and application version (app_version)
* Upgraded docker-maven-plugin to version 0.18.1
