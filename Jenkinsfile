pipeline {
        agent any
                stages {
                        stage('One') {
                                steps {
                                        env.EXECUTE="True"
                                }

                                steps {
                                        sh ' echo "Updating Second Stage" '
                                }
                        }


                        stage('Two') {
                                steps {
                                        sh echo ${EXECUTE}
                                }

                                when{
                                        equas expected: true, actual STAGE 2
                                }
                        } 

                        stage('Three') {
                                steps {
                                        sh 'echo "Step Three" '
                                }
                        }
                }
}
