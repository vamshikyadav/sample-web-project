//Below is the sample Jenkins file for the build of the sample application

def workspace;

node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/vamshikyadav/sample-web-project.git']]])
        workspace
    }
    
    stage('Static Code Analysis')
    {
        echo "Static Code Analysis"
    }
    stage('Build')
    {
        echo "Build"
    }
    stage('Unit Test')
    {
        echo "Unit Test"
    }
    
    stage('Delivery')
    {
        echo "Delivery"
    }
    
}

