node('docker') {

    stage 'Checkout'
        checkout scm
    stage 'Build & UnitTest'
        sh "docker build -t accountownerapp:B${BUILD_NUMBER} -f Dockerfile ."
        sh "docker build -t accountownerapp:test-B${BUILD_NUMBER} -f Dockerfile.Integration ."
 
}
