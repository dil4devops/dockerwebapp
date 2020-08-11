node {

    checkout scm

    docker.withRegistry('https://hub.docker.com', 'dockerHub') {

        def customImage = docker.build("nodejs/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
