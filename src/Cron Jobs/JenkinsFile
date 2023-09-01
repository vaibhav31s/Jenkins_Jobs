    pipeline {
        agent any
        stages {
            stage('Hello') {
                steps {
                    script {
                        for(def link : apiUrls.readLines()){
                            def curlCommand = """
                                echo " " >> logs.txt
                                date >> logs.txt 
                                curl ${link} >> logs.txt
                                echo " " >> logs.txt
                            """
                            def response = sh(script: curlCommand, returnStatus: false)
                        }
                    }
                }
            }
        }
    }
