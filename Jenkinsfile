pipeline
{

    agent any
parameters {
        string(name: 'BRANCH_NAME', defaultValue: 'master', description: 'Git branch to build')
    
    }

    stages
    {
        stage("checkout")
        {
              steps{
                echo " Cloning branch: ${params.BRANCH_NAME}"
                git branch: "${params.BRANCH_NAME}", url: 'https://github.com/sresrinivas/cicdpipeline.git'
              }
        }
    }
}
