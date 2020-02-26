node{
  def mvn_home = tool name: 'Maven', type: 'maven'
}

stage('Checkout from Git'){
git "https://github.com/vignesh05901/Maven_Warfile1"
}

stage('Maven clean and validate'){
sh "${mvn_home}/bin/mvn clean validate"
}

stage('Create a package'){
sh "${mvn_home}/bin/mvn package"
}
