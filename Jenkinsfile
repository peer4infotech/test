pipeline{
   agent none
   options{
       skipDefaultCheckout()
   }
  //agent none
    stages{
        stage("Build Dev")
        {
            //agent { label "myimage" }
            agent{ label "myimage" }
        //    options{
        //         skipDefaultCheckout()
        //     }
        //     steps{
        //         echo "Hello World"
        //     }
                when{
                    branch 'pipeline_git_2'
                }
                steps{
                    echo "Hello from pipeline_git_2 branch"
                }

        }
        stage("Build Main"){
            agent{ label "myimage" }
            when{
                
                branch 'main'
            }
            steps{
                echo "Hello from Main branch"
            }
        }
    }
}
