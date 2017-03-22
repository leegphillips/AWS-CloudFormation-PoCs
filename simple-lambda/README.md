#build
mvn package

#upload lambda
aws s3 \target\aws-java-simple-http-endpoint-dev.jar cp s3://lambda-functions/aws-java-simple-http-endpoint-dev.jar
