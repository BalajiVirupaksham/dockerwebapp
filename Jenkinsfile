node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'mydockerhub') {

        def customImage = docker.build("balajivirup-image/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
