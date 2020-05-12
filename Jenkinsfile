//Where you want to run the job
//node('jenkins-slave')
//node('jenkins-slave')
//Master
//JPipeline is a domain specific language (DSL)
//Irrespective of the env we can run the script either windows or linux
def workspace;
node
{
    //Subset of tasks | actions - Build, Static code analysis, Code Coverage, Code Review, Packaging, Delivery

    stage('Checkout')
    {
        def var_1
        workspace=pwd()
        echo workspace
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '0d791dfd-e21e-43f5-93df-306ed465fb64', url: 'git@github.com:edaraanand/apachej1.git']]])
    }

    stage('Code Analysis')
    {
        echo "Static Code Analysis"
        sh "sudo ls -ltr /home/Anand"
    }
    stage('Build')
    {
        echo "Build"
        sh "sudo ls -ltr /home/Anand"
    }
    stage('Unit Testing')
    {
        echo "Unit Testing"
        sh "sudo ls -ltr /home/Anand"
    }
    stage('Delivery')
    {
        echo "Delivery"
        sh "sudo ls -ltr /home/Anand"
    }
}
