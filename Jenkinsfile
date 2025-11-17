pipeline
{
    agent any
    tools {
       maven "maven-3.9.8"
    }
    stages {
        stage ('git checkout') {
            steps {
                git branch: 'bugfix', url: 'https://github.com/dev-team-co/maven-webapplication-project-kkfunda.git'
            }
        }
            stage ('build') {
                steps {
                    sh "mvn clean package"
                }
            }
    }
}
