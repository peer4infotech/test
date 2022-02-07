pipeline{
   // agent { label "myimage" }
       agent none
    stages{
        stage("Build")
        {
            agent { label "myimage" }
           options{
                skipDefaultCheckout()
            }
            steps{
                echo "Hello World"
            }


        }
    }
}
