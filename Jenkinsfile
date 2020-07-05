node {
    environment {
        VERSION_NUMBER = '1.2.1'
    }

    checkout scm

    docker.withRegistry("https://registry.hub.docker.com", 'dockerHubCredentials') {

        def customImage = docker.build("myhk2009/sample-microservices")

        /* Push the container to the custom Registry */
        //customImage.push("latest") 
        customImage.push('1.2.2')    
    }
}