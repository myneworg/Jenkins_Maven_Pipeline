node(Windowsslave) {
stage 'checkout'
git url: 'https://github.com/myneworg/Jenkins_Maven_Pipeline.git'

stage 'build'
def mvnhome = tool 'M3'
sh "${mvnhome}/bin/mvn clean package"
}
