common.killOldDeployments()
version = '1.0.0'
stagingBaseNode {
    stage('Build') {
        gitCheckout { }
        cloud.loginStaging()
        dockerImage.buildPush('.', 'mssql-exporter', "${version}")
    }
}