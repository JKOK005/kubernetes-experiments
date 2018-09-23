FROM openjdk:8-jre-alpine 
WORKDIR /setup-scala
ADD test-scala-application/target/scala-2.12/hello-world-assembly-1.0.jar next-dir/    # Compiled jar file is added to /setup-scala/next-dir/ folder
CMD ["java", "-jar", "next-dir/hello-world-assembly-1.0.jar"]