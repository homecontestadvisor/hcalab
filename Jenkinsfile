node ('master') {
  def project = 'hcalab'
  def appName = 'gceme'
  def feSvcName = "${appName}-frontend"
  def imageTag = "gcr.io/${project}/${appName}:${env.BRANCH_NAME}.${env.BUILD_NUMBER}"

    stage "install"
    sh "pwd"
    sh "./docker/startup.sh"
    sh "cd docker"
    sh "ls -a"
}