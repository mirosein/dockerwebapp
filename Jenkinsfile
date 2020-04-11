node {
    checkout scm

    docker.withRegistry('https://github.com/mirosein/dockerwebapp.git', 'dockerhub') {

        def customImage = docker.build("mirosein/node-web-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
