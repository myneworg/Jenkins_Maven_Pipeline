//node(Linux_Slave) {
//#git url: 'https://github.com/myneworg/Jenkins_Maven_Pipeline.git'
//echo "Linux_Slave"

node ('Linux_Slave') {
    git url: "$GIT_REPO_URL", branch: "$GIT_BRANCH"
    echo env.GIT_COMMIT
    echo env.GIT_BRANCH
    echo env.GIT_REVISION
}
