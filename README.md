 pipeline {
         agent any
         stages {
         stage(Build){
         steps{
         echo "build the application"
        }
      }
       stages {
       stage("test"){
       steps{
       echo "test the application"
      }
    }
    stages {
    stage("deploy"){
    steps{
    echo "deploy the application"
    }
  }
}
}
}
}
