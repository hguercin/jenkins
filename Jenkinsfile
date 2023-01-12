node {
    stage('clone') {
        git credentialsId: '736c4c49-ab6c-45a0-8a6d-ad48867c3738', url: 'https://github.com/hguercin/jenkins.git'
    }
    stage('build') {
        sh label: 'script', script: 'javac Main.java'
    }
    stage('run') {
        sh label: 'script', script: 'java Main'
    }
    stage('repertoire') {
        sh label: 'script', script: 'ls -ltr'
    }
}
