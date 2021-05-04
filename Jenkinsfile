node('docker'){
    def customImage //variable to define the built image
   
    stage('Checkout SCM'){
        checkout scm
        }
       
    stage('Docker build'){
        customImage = docker.build("myimage:${env.BUILD_ID}") //build the image in the docker file using the tag as "myImage:build_number"
        }
       
    stage('Docker push'){
