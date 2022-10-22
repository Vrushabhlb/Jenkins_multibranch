node('master')

{

stage('ContinuousDownload_master_edit')

         {

    git 'https://github.com/sunildevops77/maven.git'

        }

stage('Continuousbuild_master_edit')

         {

   sh label: '', script: 'mvn package'
        }


}
