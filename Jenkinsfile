pipeline
{
  agent any
  stages
  {
    stage("build")
    {
      echo "[step] building...."
      bat="dotnet restore /src/helloworld/helloword.csproj"
      bat="dotnet clean /src/helloworld/helloword.csproj"
      bat="dotnet build /src/helloworld/helloword.csproj"
    }
    stages
  {
    stage("test")
    {
      steps
      {
        echo "[step] testing..."
      }
    }
stages
  {
    stage("deploy")
    {
      steps
      {
        echo "[step] deploying..."
      }
    }
  }
}
