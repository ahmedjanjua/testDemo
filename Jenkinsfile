pipeline 
{
  agent any
  stages 
  {
    stage('Build') 
    {
      steps 
      {
        echo 'Building..'
        // Here you can define commands for your build
      }
    }
    stage('Test') 
    {
      steps 
      {
        echo 'Testing..'
        // Here you can define commands for your tests
      }
    }
    stage('Deploy') 
    {  
      steps 
      {
        echo 'Deploying....'
        // Here you can define commands for your deployment
      }
    }
  }
  post
  {
    //conditions here will be executed after build
    always
    {
      //always run despite build failed
      echo "Post build condition running'
      failure
      {
        //only if build is failed
        echo 'Post action if build failed
      }
    }
  } 
}
