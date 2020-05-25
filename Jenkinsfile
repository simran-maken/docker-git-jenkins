pipeline
{
	agent any
	stages
	{
		stage("create docker image")
		{
			agent
			{
				dockerfile true
			}
			steps
			{
				echo "container id: ${Container.id}"
			}
		}
	}
}