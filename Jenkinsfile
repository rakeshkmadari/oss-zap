node("BuildServer"){
    checkout scm
    stage("run security scan"){
        sh "sudo docker run --rm -v ${WORKSPACE}:/zap/wrk:rw -t owasp/zap2docker-stable zap-baseline.py -t http://35.227.18.144/ -c config"
    }
}