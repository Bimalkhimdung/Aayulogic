pipeline{
    agent any
    stages{
        stage("Checking for Jnekins File .."){
         steps{
            script{
                def filepath = './script.sh'

                if(fileExits(filepath)){
                    sh " chmod +x $filepath"

                    sh "./$filepath"
                }
                else{
                    echo"file doesnot exits"
                }

            }
        }
    }
    }

}