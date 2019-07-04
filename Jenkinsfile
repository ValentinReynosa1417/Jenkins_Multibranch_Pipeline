pipeline {
        agent any
        stages {
                stage('Stage first') {
                        steps {
                                script {
                                        echo "Building"
                                        env.EXECUTE = 'true'
                                }
                        }
                }

 

                stage('Stage second') {
                        when {
                                expression {
                                        env.EXECUTE == 'true'
                                }
                        }

 

                        steps {
                                script {
                                        echo "Updating second stage"
                                        echo "${env.EXECUTE}"
                                }
                        }
                }

 

                stage('Stage third') {
                        when {
                                expression {
                                        env.EXECUTE == 'false'
                                }
                        }
                        steps {
                                script {
                                        echo "Deploying yes"
                                }
                        }

 

                }
        }
}
