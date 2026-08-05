@Library('mylibrary')_


pipeline
{
    agent any
    stages
    {
        stage('Download_Master')
        {
            steps
            {
                script
                {
                    cicd.gitDownload("maven")
                }
            }
        }
        stage('Build_Master')
        {
            steps
            {
                script
                {
                    cicd.buildArtifact()
                }
            }
        }
        stage('Deployment_Master')
        {
            steps
            {
                script
                {
                    cicd.deployTomcat("DeclarativePipelinewithSharedLibraries","172.31.31.19","myapp")
                }
            }
        }
        stage('Testing_Master')
        {
            steps
            {
                script
                {
                    cicd.gitDownload("FunctionalTesting")
                    cicd.executeSelenium("DeclarativePipelinewithSharedLibraries")
                }
            }
        }
        stage('Delivery_Master')
        {
            steps
            {

	    script

                script

                {
                    cicd.deployTomcat("DeclarativePipelinewithSharedLibraries","172.31.25.180","myprodappp)                }
            }
        }
    }
}

=======
>>>>>>> 4a96ceeb3828c174be6679d2b7294fb956fad43d
