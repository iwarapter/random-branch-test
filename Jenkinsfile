pipeline {
    agent any
    triggers { 
      upstream(upstreamProjects: 'lattice-triggah', threshold: hudson.model.Result.SUCCESS) 
    }
    stages {
        stage('Example') {
            steps {
                echo env.BRANCH_NAME
            }
        }
    }
}
