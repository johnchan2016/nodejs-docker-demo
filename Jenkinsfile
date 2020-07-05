node {
    checkout scm

    docker.withRegistry("https://registry.hub.docker.com", 'dockerHubCredentials') {

        def customImage = docker.build("myhk2009/sample-microservices")
        customImage.push("${VERSION}");
    }
}