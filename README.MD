### Setup Docker Agent Slave in Jenkins 

*Go to Jenkins under Mangage Jenkins click ok Manage Nodes and Clouds, click on configure cloud*
1. add Name: Docker
2. Docker Host URI?: unix:///var/run/docker.sock
3. Enable checkbox
4. Test Connection


*Add Docker Agent Template*

1. Label: dockeragent
2. Name: DockerAgent
3. DockerImage: jenkins/inbound-agent

**connect method** is important if you are choosing *Attach Docker Container* it means docker and jenkins install same machine
