node ('master') {
  def project = 'hcalab'
  def appName = 'gceme'
  def feSvcName = "${appName}-frontend"
  def imageTag = "gcr.io/${project}/${appName}:${env.BRANCH_NAME}.${env.BUILD_NUMBER}"

    stage "install"
    checkout scm
    sh "./docker/startup.sh"
    ls | grep docker | xargs cd
    
}