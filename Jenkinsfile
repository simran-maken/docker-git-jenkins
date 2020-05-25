pipeline
{
	agent any
	options
	{
		buildDiscarder(logRotator(numToKeepStr: '5'))
	}
	stages
	{
		stage("create docker image")
		{
			steps
			{
				script
				{
					sh "docker image pull simranmaken/python:version3"
				}
			}
		}
		stage("Image name")
		{
			steps
			{
				echo "image name: ${Image.imagename}"
			}
		}
	}
}