node {
    stage ('Preperation'){
        echo "Preparation"
        git credentialsId: '76bd5caa-ab6b-4245-a865-09e9c135f985', url: 'git@github.com:praqma-training/jenkins-pipeline-exercise.git'

    }
    stage ('Build'){
        echo "Build"
        sh'pwd'
        sh'./gradlew clean test jar'
    }
    stage ('Result'){
        echo "Result"
        junit '**/build/test-results/test/TEST-*.xml'
        archiveArtifacts 'build/libs/*'
    }
}
