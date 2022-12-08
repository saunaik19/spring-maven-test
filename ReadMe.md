# Read Me First

I am trying this to explore remote & local repositories in Maven
snapshot repository
release repository
mix of both

below is command to run nexus sonatype on docker

To run sonatype nexus on docker run this
`docker run -d -p 4081:4081 --name nexus -e MAX_HEAP=614m sonatype/nexus`


default user name is admin & password is admin123
1) Create 3 repos
maven-group as a proxy

Create maven-snapshot & maven-releases repos

make sure to create volume for your image & point to it

`mvn --s .\settings.xml clean install > maven_output.txt`

If you use  spring-maven-test 


| **Version**                           | **Repository**      |
|-----------------------------------|-----------------|
| <version>0.0.1-SNAPSHOT</version> | maven-snapshots |
| <version>1.0</version>            | maven-releases  |

