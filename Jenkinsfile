
pipeline{
	 agent{
              label{
                     label "built-in"
                     customWorkspace "/mnt/prachi11"
                   }
            }

	 stages{
               stage("stage-1"){
                               steps{
                                    sleep 10
                                    echo "welcome step 1"
			            }
				}

               stage("stage-2"){

                         agent{
                             label{
                                   label "slave-B"
                                   customWorkspace "/mnt/sonali"
                                   }
                               }
                               
                          steps{
                                    sleep 10
                                    echo "welcome step 2"
			            }
		}

               stage("Test"){
			  steps{
                                build "pipe1"
                               echo "hello this is first declarative script"
                   }
		} 
		}
}  
