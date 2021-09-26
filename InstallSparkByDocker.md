## Step 1: Generate dockerfile
```
vim dockerfile
```
## Step 2: Build docker image
```
docker build -t jupyter/pyspark-notebook .
```
## Step 3: Run container
```
docker run -it --rm -p 8888:8888 jupyter/pyspark-notebook
```
or 
```
docker run -it --rm -p 8888:8888 -v /Users/shuhsi/github:/home/jovyan/work jupyter/pyspark-notebook
```
## Step 4: Connect to Jupyter Notebook
```
# Copy/paste this URL into your browser (if the first)
http://localhost:8888/?token=e144d004f6652ae6406a78adf894621e62fdeb1fc57d02e8
```
Replace the localhost by the public DNS of this EC2