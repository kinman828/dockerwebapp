node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("stevelaw/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
