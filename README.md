# maven-resolver-test

## Directions

After cloning, run `apache-maven-3.8.7/bin/mvn dependency:resolve; apache-maven-3.9.0-SNAPSHOT/bin/mvn dependency:resolve`  (will take a while to complete)

After that, your local repository should be fully populated and you can run subsequent tests with the `--offline` flag

Compare the performance of:

1. `apache-maven-3.8.7/bin/mvn dependency:resolve --offline`
2. `apache-maven-3.9.0-SNAPSHOT/bin/mvn dependency:resolve --offline`
3. `apache-maven-3.9.0-SNAPSHOT/bin/mvn dependency:resolve --offline -Daether.dependencyCollector.impl=bf`
