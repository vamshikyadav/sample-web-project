//Below is the sample Jenkins file for the build of the sample application

def workspace;
def name;

node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/vamshikyadav/sample-web-project.git']]])
        workspace
    }
    
    stage('Static Code Analysis')
    {
        name = "Vamshi Krishna Yadav"
        echo "Static Code Analysis ${name}"
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
        // below we are calling the function
        returnfunction()
    }
    
    // below is the method/function
    def returnfunction()
    {
        def value = "Calling the function"
        echo "this is how: ${value}" 
    }
}

