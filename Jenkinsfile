pipeline
{
  agent any
  stages
  {
    stage("build")
    {
      steps
      {
        echo "[step] building......"
        bat="dotnet restore /src/helloworld/helloword.csproj"
        bat="dotnet clean /src/helloworld/helloword.csproj"
        bat="dotnet build /src/helloworld/helloword.csproj"
        archiveArtifacts artifacts: "src/helloword/bin/**"
      }
    }
    stage("test")
    {
      steps
      {
        echo "[step] testing..."
      }
    }
    stage("depoly")
    {
      steps
      {
        echo "[step] deploying..."
      }
    }
  }
}

post
{
  failure
  {
    echo "the build has failed"
  }
}
