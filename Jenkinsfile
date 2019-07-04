pipeline {
        agent any
                stage('STAGE 1')
                      steps {
                            script {
                                    env.EXECUTE="True"
                                   }
                      steps {
                            sh ' echo "Updating Second Stage" '
                            }
                      }
                satge('STAGE 2')
                      steps {
                            script {
                                     sh echo ${EXECUTE}
                       when{
                                     equas expected: true, actual STAGE 2
                            }

                                    }
                         }

         }



