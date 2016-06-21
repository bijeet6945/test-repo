node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Get some code from a GitHub repository
   git credentialsId: '1e2e7fc3-e2b5-41e5-b8c1-5794dcc82fc7', url: 'https://github.com/prashantgwaghmare/test-repo.git'

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.           
   def mvnHome = '/home/ubuntu/apache-maven-3.3.9'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   sh "${mvnHome}/bin/mvn clean install"
}
