## 1 Node Assignment

### Task 1: Create docker image:
  ```
  $ docker build .
  ```
 Resultant Iamge Id: `8f1eb8d97a36`

### Task 1.1 Create docker image with custom name and tag
  ```
  $ docker build -t nodeappimage:v101
  ```

### Task 2: Run docker container
  ```
  $ docker run -p 8000:3000 8f1eb8d97a36
  ```
### Task 3: Stop docker container
  ```
  $ docker stop 8f1eb8d97a36
  ```

### Task 4: Recreate docker container with custom name
  ```
  $ docker run -p 8000:3000 --name nodeapp 8f1eb8d97a36
  ```

### Task 5: Delete stopped container
  ```
  $ docker rm nodeapp
  ```

### Task 5.1: Delete unused images
  ```
  $ docker rmi nodeappimage
  ```

### Task 6: Delete docker container when stopped
  ```
  $ docker run -p 8000:3000 -d --name nodeapp --rm 8f1eb8d97a36 
  ```
## 2 Python Assignment

### Task 1: Create docker image:
  ```
  $ docker build .
  ```
 Resultant Iamge Id: `ee56aea18773`

### Task 1.1 Create docker image with custom name and tag
  ```
  $ docker build -t pythonappimage:v202
  ```

### Task 2: Run docker container
  ```
  $ docker run -it ee56aea18773
  ```
### Task 3: Stop docker container
  ```
  $ docker stop ee56aea18773
  ```
### Task 4: Recreate docker container with custom name
  ```
  $ docker run -p 8000:3000 --it pythonapp ee56aea18773
  ```

### Task 5: Delete stopped container
  ```
  $ docker rm nodeapp
  ```

### Task 5.1: Delete unused images
  ```
  $ docker rmi pythonappimage
  ```

### Task 6: Delete docker container when stopped
  ```
  $ docker run -p 8000:3000 --it pythonapp --rm ee56aea18773
  ```
