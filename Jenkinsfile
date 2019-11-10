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
        // below is the call for the return value

        def value = "Vamshi"
        def finput = samplereturn(value)
        echo "${finput}"
    }
    
    stage('Delivery')
    {
        echo "Delivery"
        // below we are calling the function
        returnfunction()
    }    
   
}

 // below is the method/function implementation outside of the node space
    def returnfunction()
    {
        def value = "Calling the function";
        echo "this is how: ${value}" 
    }

    // Below is the node function to return a value

    def samplereturn(String value)
    {
        def input = "connection the values for Jenkins file: ${value} ";
        return input
    }

