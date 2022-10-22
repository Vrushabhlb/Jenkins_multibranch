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


}
