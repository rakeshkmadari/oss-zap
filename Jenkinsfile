node{
    checkout scm
    stage("run security scan"){
        //sh "sudo docker run --rm -v ${WORKSPACE}:/zap/wrk:rw -t owasp/zap2docker-stable zap-baseline.py -t http://localhost:10000/ -c config"
        //sh "sudo docker run --rm -t owasp/zap2docker-stable zap-baseline.py -t http://spring -u https://github.com/devopsevd/oss-zap/blob/master/config"
        //sh "sudo docker run --net testnet --ip 10.0.0.6 --rm -t owasp/zap2docker-stable zap-baseline.py -t http://10.0.0.5 -u https://github.com/devopsevd/oss-zap/blob/master/config"
        sh "sudo docker run --rm -t owasp/zap2docker-stable zap-baseline.py -t http://tomcat:10000 -u https://github.com/devopsevd/oss-zap/blob/master/config"
    }
}
