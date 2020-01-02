pipeline
{
agent any 
stages{
stage('Build Application'){
steps{
sh 'mvn clean install'
}
}

stage('Deploy Application To Mulesoft CloudHub'){
steps{
sh 'mvn package deploy -DmuleDeploy'
}
}

}
}