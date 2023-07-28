pipeline{
	agent{ 
	        label "built-in"
	     }
        stages{
                stage("parallel-stages"){ 
                       parallel{
                           stage ("parallel-1"){
                                 steps{
                      		       sleep 10
                                       echo "hello all"
                                      }
                                   }
                           stage ("parallel-2"){
                                  steps{
                                        sleep 10
                                        echo "second hii"
                                       }
                                    }
                           stage ("parallel-3"){
                                   steps{
                                           sleep 10
                                           echo"thirs hii"
                                          }
                                     }
                                 }
                             }
                  }
          } 
