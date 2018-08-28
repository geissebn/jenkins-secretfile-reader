# jenkins secret file reader

This simple ``Jenkinsfile`` makes it possible to read a *secret* file from Jenkins

Just create a pipline job with the content given, start a build and add the ID of the secret file as build parameter.

Et voilà: Its content is 'cat'ed into the build log.
