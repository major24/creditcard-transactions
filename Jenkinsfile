node {
	stage ('Checkout git repo') {
		git branch: 'master', url: 'https://github.com/major24/creditcard-transactions.git'
	}
	
	stage ('Build and publish') {
		dotnet restore
		dotnet publish -c Production -o publish
	}

}