pipeline{
   agent{ label "myimage" }
   options{
       skipDefaultCheckout()
   }
  //agent none
    stages{
        stage("Build Dev")
        {
            //agent { label "myimage" }
            // agent{ label "myimage" }
        //    options{
        //         skipDefaultCheckout()
        //     }
        //     steps{
        //         echo "Hello World"
        //     }
                when{
                    buildingTag()
                }
                steps{
                    echo "Hello from pipeline_git_2 branch. it is tag build"
                }

        }
        stage("Build Main"){
            // agent{ label "myimage" }
            when{
                
                tag "3.0"
            }
            steps{
                echo "Hello from tag 3.0"
            }
        }
    }
}
