properties([pipelineTriggers([pollSCM('* * * * *')])])
node {
    stage("clone"){
       checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/avielb/moshe.git']]]) 
    }
    stage("show files"){
        sh "ls -l"
    }
}
