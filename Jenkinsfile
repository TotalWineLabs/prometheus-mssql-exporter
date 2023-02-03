common.killOldDeployments()
version = 'v1.0.1'
stagingBaseNode {
    stage('Build') {
        gitCheckout { }
        cloud.loginStaging()
        dockerImage.buildPush('.', 'mssql-exporter', "${version}")
    }
}