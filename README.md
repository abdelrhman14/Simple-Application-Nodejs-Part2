# Simple-Application-Nodejs-Part2
### Jenkinns CI | CD 
![MicrosoftTeams-image](https://user-images.githubusercontent.com/42601017/199500683-f6022849-3794-49c8-8043-2913806e5e44.png)

1. Cloning this project https://github.com/abdelrhman14/Simple-Application-Nodejs-Part2.git
2. Credentials : withCredentials([usernamePassword(credentialsId: 'dockerhub_key', passwordVariable: 'PASSWORD', usernameVariable: 'USERNAME')])
3. Build Image And Push on DockerHub
    docker build -t nodejs-image33 .
    docker tag nodejs-image33:latest abdelrahman1413/nodejs-image33
    docker push abdelrahman1413/nodejs-image33
![endday1(1)](https://user-images.githubusercontent.com/42601017/199501655-d58e56a7-ce09-491e-9257-73739cf3e05d.png)
4. Deployment
    - NameSpace [application]
    - Deploy app
    - Loadbalancer 
    kubectl create namespace application
    kubectl apply -f deployment.yml -n application
    kubectl apply -f app_loadbalancer.yml -n application
    
    
 ### [Hint] Install Plugins:
    -  Docker
    - Role-based Authorization Strategy
 ###  ### [Hint] Credentials:
    - Docker
    - GitHub
  

    ![End](https://user-images.githubusercontent.com/42601017/199502864-27e6d1e5-9532-4f37-bc08-9e834b6416c1.png)

