node{
     stage(scm checkout)
     {
     git credentialsId: 'GIT', url: 'https://github.com/ppuhan/maven-web-project.git'
     }
     stage(test)
     {
     echo testing the source code
     }
     stage(package)
     {
     echo package the source code to binary artifact
     }
     
}
