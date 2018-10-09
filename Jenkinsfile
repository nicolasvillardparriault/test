node {

    stage("test") {
        docker.image("ubuntu").inside("-u root") {
            echo 'hello World'
            sh 'echo cat /etc/passwd=$(cat /etc/passwd)'
            sh 'id=$(id)'
            sh 'useradd -m -u 1000 toto'
            sh 'su toto'
            sh 'whoami=$(whoami)'
        }
    }

}