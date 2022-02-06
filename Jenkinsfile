pipeline{
    agent 
    stages{
        stage("Build")
        {
            agent { label "myimage" }
           /* options{
                skipDefaultCheckout()
            }*/
            steps{
                echo "Hello World"
            }


        }
    }
}