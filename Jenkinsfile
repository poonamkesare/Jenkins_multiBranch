node('built-in') 
{
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build_loans') 
	{
    sh label: '', script: 'mvn package'
	}
    stage('Continuous Deployment_loans') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/sc-pipeline/webapp/target/webapp.war   ubuntu@172.31.42.88:/var/lib/tomcat9/webapps/qaenv.war'
	}
    
}
