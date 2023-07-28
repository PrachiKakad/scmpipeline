pipeline{
	agent{ 
	        label "built-in"
	     }
        stages{

		stage( "seq-1"){
                                steps{
                                      sleep 10
                                      echo "seq step-1"
                         	      }
				}
          
		stage( "seq-2"){
                                steps{
                                      sleep 10
                                      echo "seq step-2"
                         	      }
				}

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

		stage( "seq-3"){
                                steps{
                                      sleep 10
                                      echo "seq step-3"
                         	      }
				}

		stage( "seq-4"){
                                steps{
                                      sleep 10
                                      echo "seq step-4"
                         	      }
				}
          
          

                  }
          }  
