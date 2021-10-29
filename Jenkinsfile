pipeline {
    agent any
    
    stages{
        script{
    try{
        stage('checkout Source dev Repo'){
            when{
                branch 'dev'
            }
        steps{
            sh 'mkdir tar'
            dir( "tar"){
            
            sh 'git clone https://prajwalyb:Gitpass1234@github.com/prajwalyb/maven4.git'
        
            //sh 'pwd'
            sh 'git remote -v'
            
        
            sh 'git remote add upstream https://anurajbhandari5:Anuraj123456789@github.com/anurajbhandari5/microservice.git'
            
            sh 'git remote -v'
           sh 'git fetch upstream'
           
            sh 'git checkout dev'
            //sh 'git merge upstream/master'
            sh 'git pull upstream dev'
           
           
            sh  'git push https://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@github.com/prajwalyb/maven4.git '
            
} 
       
            
            }            
        
        } 
        stage('checkout Source master Repo'){
            when{
                branch 'master'
            }
        steps{
            sh 'mkdir tar'
            dir( "tar"){
            
            sh 'git clone https://prajwalyb:Gitpass1234@github.com/prajwalyb/maven4.git'
        
            //sh 'pwd'
            sh 'git remote -v'
            
        
            sh 'git remote add upstream https://anurajbhandari5:Anuraj123456789@github.com/anurajbhandari5/microservice.git'
            
            sh 'git remote -v'
           sh 'git fetch upstream'
           
            sh 'git checkout master'
            //sh 'git merge upstream/master'
            sh 'git pull upstream master'
           
           
            sh  'git push https://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@github.com/prajwalyb/maven4.git '
            
} 
       
        }
        }
    }
    }
        catch(all){
        sh 'git remote remove upstream'
        

       sh 'rm -rf *'
            
            }            
        
        } 
}
