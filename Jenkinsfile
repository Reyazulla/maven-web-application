node('nodes')
{
    def mavenHome = tool name: "maven3.6.3"
    
stage('CheckoutCode')

{
git branch: 'development', credentialsId: '0d2a42f9-eb31-4c9a-a34c-d3754e0c75d2', url: 'https://github.com/Reyazulla/maven-web-application.git'
}
stage('Build')
{
  sh "${mavenHome}/bin/mvn clean package"
}
    /*
stage('ExecuteSonarQubeReport')
{
  sh "${mavenHome}/bin/mvn sonar:sonar"
}

stage('UploadArtifactIntoNexus')
{
  sh "${mavenHome}/bin/mvn deploy"
}
stage('DeployAppintoTomcatserver')
{
 sshagent(['b4bffd69-6c10-4904-96be-c9f014109ab7']) {
    sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@13.233.141.13:/opt/apache-tomcat-9.0.41/webapps/"
}
}
stage('SendEmailNodification')
{
  mail bcc: 'reyazansar@gmail.com', body: '''build over ....


regards ,
reyzaulla''', cc: 'reyazansar@gmail.com', from: '', replyTo: '', subject: 'build over', to: 'reyazansar@gmail.com'
}
*/
}
