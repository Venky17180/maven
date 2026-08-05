@Library('mylibrary') _
pipeline
{
    agent any
    stages
    {
        stage('download')
        {
            steps
            {
                script
                {
                    cicd.gitdownload("maven")
                }
            }
        }
        stage('build')
        {
            steps
            {
                script
                {
                    cicd.buildArtifact()
                }
            }
        }
   }}
