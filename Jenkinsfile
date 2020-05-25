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
					im = docker.image("simranmaken/python:version3").pull()
				}
			}
		}
		stage("Image name")
		{
			steps
			{
				echo "image name: ${Image.imageName}"
			}
		}
	}
}