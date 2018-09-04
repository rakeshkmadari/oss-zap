node{
    checkout scm
    stage("run security scan"){
     /* sh "sudo docker run --network=bundlev2_prodnetwork --rm -t owasp/zap2docker-stable zap-baseline.py -t https://samplep2000474034trial.hanatrial.ondemand.com/explore-ui5/ -u https://github.com/shree47/oss-zap/blob/master/config"*/
     sh "sudo docker run -t owasp/zap2docker-stable zap-baseline.py -t https://samplep2000474034trial.hanatrial.ondemand.com/explore-ui5/ -u https://github.com/shree47/oss-zap/blob/master/config"       
    }
}
