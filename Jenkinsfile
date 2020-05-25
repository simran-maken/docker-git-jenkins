pipeline
{
	agent any
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