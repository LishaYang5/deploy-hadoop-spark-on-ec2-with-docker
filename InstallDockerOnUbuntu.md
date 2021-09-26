## Step 1:
```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```
## Step 2:
```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```
## Step 3:
```
sudo apt-get update
```
## Step 4:
```
sudo apt-get install -y docker-ce
```
## Step 5:
```
sudo usermod -aG docker ${USER}
```
## Step 6: Restart EC2
```
sudo reboot
```