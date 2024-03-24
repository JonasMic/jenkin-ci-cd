/*
pipeline{

    agent any
    tools{
        maven "maven"
    }
    stages{

        stage("SCM checkout"){
            steps{
                checkout scmGit(branches: [[name: '*//*
main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/JonasMic/jenkin-ci-cd.git']])
            }
        }

        stage("Build Process"){
            steps{
                script{
                     bat 'mvn clean install'
                }
            }
        }

         */
/* stage("Deploy to container"){
            steps{
                deploy adapters: [tomcat9(credentialsId: 'tomcat.pwd', path: '', url: 'http://localhost:8080/')], contextPath: 'jenkinsCiCd', war: '**  */
/* *//*
 */
/*.war'
            }
        } *//*




    }

     post{
            always{
                emailext attachLog: true, body: '''<html>
    <body>
        <p>Build Status: ${BUILD_STATUS}</p>
        <p>Build Number: ${BUILD_NUMBER}</p>
        <p>Check the <a href="${BUILD_URL}">console output</a>.</p>
    </body>
</html>''', mimeType: 'text/html', replyTo: 'faycontrag@gmail.com', subject: 'Pipleline_Status: ${BUILD_NUMBER}', to: 'faycontrag@gmail.com'
            }
        }
}

//SCM checkout
//build
//deploy WAR
// EMAIL */
