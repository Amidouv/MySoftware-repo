nes (9 sloc)  302 Bytes
   
properties([pipelineTriggers([pollSCM('* * * * *')])])
node {
    stage("clone"){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Amidouv/MySoftware-repo.git']]])
    }
    stage("show files"){
        bat "dir"
    }
}
