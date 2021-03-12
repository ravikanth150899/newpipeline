pipeline
{
	agent any
	stages
	{
		stage('build')
		{
			steps
			{
				sh 'mvn clean install'
			}
		}
		stage('deploy')
		{
			steps
			{
				sh 'mv target/*.war javademoex.war'
				sh 'sudo cp javademoex.war /var/lib/tomcat9/webapps'
			}
		}
		}
}
