node {
input 'Ready to go?'
git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'

def mvnHome = tool 'M3'
input 'Ready to go?'
sh "${mvnHome}/bin/mvn clean package"
}
