node{
   checkout scm
   def image = docker.image("node:16-buster-slim")
   image.inside{
      stage("Build"){
         sh "npm install"
      }
      stage("test"){
         sh "./jenkins/scripts/test.sh"
      }
   }
}
