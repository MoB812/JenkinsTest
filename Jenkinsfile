node {
    def awsIAMApiImg

    stage('Pull Dockerfile from Repo') {
        /* 
            Checkout/Download Dockerfile from SCM or some other location
            ...need to configure here
         */
        
        /* use this command if configured scm in Jenkins Pipeline */
        checkout scm
    }

    stage('Build Image') {
        /* Build the Docker image from Dockerfile */
        awsIAMApiImg = docker.build(JenkinsTest/)
    }

    stage('Test Image') {
        /* Execute any scripts/commands you want here to test the image */
    }

    stage('Deploy Image') {
        /* 
            Save the image to a container registry service like Amazon ECR.
        */
    }
}
