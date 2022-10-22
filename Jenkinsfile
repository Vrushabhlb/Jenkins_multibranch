node('master')

{

stage('ContinuousDownload_child')

         {

    git 'https://github.com/sunildevops77/maven.git'

        }

stage('Continuousbuild_child')

         {

   sh label: '', script: 'mvn package'
        }


}
