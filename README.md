# jenkins<br/>	  
sudo apt-get update<br/>	
sudo add-apt-repository ppa:openjdk-r/ppa<br/>
sudo apt install -y openjdk-11-jre-headless<br/>
wget -qO - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add - <br/>	
sudo apt-get upgrade<br/>	   
echo deb https://pkg.jenkins.io/debian-stable binary/ | sudo tee /etc/apt/sources.list.d/jenkins.list<br/>	
sudo apt-get update<br/>
sudo apt-get -y install jenkins<br/>
sudo cat /var/lib/jenkins/secrets/initialAdminPassword<br/>
sudo nano /etc/sudoers<br/>
sudo reboot<br/>
jenkins ALL=(ALL) NOPASSWD:ALL<br/>
