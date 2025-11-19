pipeline 
{
    agent any
    tools 
    {
        maven "maven-3.9.8"
    }
    stages 
    {
        stage ("gitcheckout")
        {
            steps {
                git branch: 'development', url: 'https://github.com/dev-team-co/maven-webapplication-project-kkfunda.git'
            }
        }
        stage ("build")
        {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
