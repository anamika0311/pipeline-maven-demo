node {
   // Mark the code checkout 'stage'....
   //Changes are made 6/9/17 5:21 pm
   stage 'Checkout'

   // Checkout code from repository
   checkout scm

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.
   //def mvnHome = tool 'M3'
   def mvnHome= "D:\\apache-maven-3.1.1"
   env.JAVA_HOME = tool 'Java 1.7.0_101'

   // Mark the code build 'stage'....
   stage 'Build'
   input 'Ready to go?'
   // Run the maven build
   bat "${mvnHome}\\bin\\mvn verify"
}
