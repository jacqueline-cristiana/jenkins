- docker pull jenkins/jenkins:lts
- docker run --name myjenkins -p 8080:8080 -p 50000:50000 -v /var/jenkins_home jenkins/jenkins:lts
- docker logs <container-name> -> password for jenkins

docker stop container_id
cd jenkins
docker rm container_id
docker rmi jenkins/jenkins:lts
cd ..
docker built -t jenkins/jenkins:lts .