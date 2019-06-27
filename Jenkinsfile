pipeline {
    agent any {
    options {
       skip stage after unstable()
      }
    stages{
       stage('Build'){
            steps {
               sh 'make'
}
}
      stage('Test'){
             steps {
                sh 'make check'
                junit 'report/* */*.xml'
}
}
      stege('Deploy'){
           steps {
              sh 'make publish'

}
}

}
}
}
}

