command : -

sudo docker run -d --name sonarqube -p 9000:9000 sonarqube:latest










✅ Breakdown:
Part	Meaning
sudo	Runs the command as a superuser (needed if your user doesn't have Docker permissions).
docker	The Docker CLI command.
run	Creates and starts a new Docker container.
-d	Detached mode – runs the container in the background.
--name sonarqube	Names the container sonarqube so it's easy to reference later.
-p 9000:9000	Maps port 9000 of your machine to port 9000 inside the container (SonarQube runs on 9000).
sonarqube:latest	Tells Docker to use the latest version of the official SonarQube image from Docker Hub.

📌 What It Does
Downloads the latest SonarQube Docker image (if not already downloaded).

Starts a container running SonarQube.

Makes SonarQube available at http://localhost:9000 or your server's IP on port 9000.

✅ What to Do After
Open your browser:
http://localhost:9000 (or http://<your-EC2-IP>:9000 if remote)

Login using:

Username: admin

Password: admin@123

