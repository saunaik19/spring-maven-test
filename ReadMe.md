# Read Me First

I am trying this to explore remote & local repositories in Maven
snapshot repository
release repository
mix of both

below is command to run nexus sonatype on docker

To run sonatype nexus on docker run this
`docker run -d -p 4081:4081 --name nexus -e MAX_HEAP=614m sonatype/nexus`

Default user name is admin & password is admin123


**Create 3 repos**
1) Create maven-group as a proxy repo
2) Create maven-snapshot repo
3) Create maven-releases repo

make sure to create volume for your image & point to it


TO run maven command use below command
`mvn --s .\settings.xml clean install > maven_output.txt`

If you use  spring-maven-test 


| **Version**                           | **Repository**      |
|-----------------------------------|-----------------|
| <version>0.0.1-SNAPSHOT</version> | maven-snapshots |
| <version>1.0</version>            | maven-releases  |

