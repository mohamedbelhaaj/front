pipeline {

    agent { node { label 'prod' } }
    
    stages {


        stage('Build image front2/sysinfo ') {
            
            steps { 
            dir ('projet-front') {
                 sh ' sudo docker build -t front2/sysinfo  . && sudo docker run -d -it -p 80:80/tcp --name sysinfo front2/sysinfo:latest'
               
                         }
                      

			   
     
            }
        }
}


   
   
}