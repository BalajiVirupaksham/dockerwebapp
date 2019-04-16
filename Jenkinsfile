node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'mydockerhub') {

        def customImage = docker.build("balajivirup-image:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
