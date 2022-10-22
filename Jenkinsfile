node('built-in')
{
stage('ContinuousDownload_master_vrushabh')
         {
    git 'https://github.com/sunildevops77/maven.git'
        }
stage('Continuousbuild_master_vrushabh')
         {
   sh label: '', script: 'mvn package'
        }
stage('ContinuousDeploy_master_vrushabh')
         {
         deploy adapters: [tomcat9(credentialsId: 'c2dfbe7d-bd18-45e3-80ff-69c626a7204d', path: '', url: 'http://172.31.7.10:8080/')], contextPath: 'vrushenv', war: '**/*.war'
        }
    stage('ContinuousTesting_master_vrushabh')
         {
         sh 'echo "test passed"'
        }
     stage('ContinuousDeploy_master_vrushabh')
         {
         deploy adapters: [tomcat9(credentialsId: '5ea6a75d-f8c1-4497-92ec-5297edb43adf', path: '', url: 'http://172.31.14.195:8080/')], contextPath: 'sarojaenv', war: '**/*.war'
        }
}
