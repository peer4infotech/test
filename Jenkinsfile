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
                    tag "release-to-*"
                }
                steps{
                    echo "Hello from pipeline_git_2 branch. it is tag 4.0 build"
                }

        }
    }
}
