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

stage('Perform Regression Testing'){
steps{
sh 'newman run /home/mustafa/Music/newmen/WORLD-TIME-ZONE.postman_collection.json'
}
}

}
}