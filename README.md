# elasticsearch-surefire-test

Tests the running of unit tests with Elasticsearch's test framework

When running multiple unit tests in a Maven project and one of those unit tests extends the org.elasticsearch.test.ESSingleNodeTestCase class, the surefire-plugin will throw an Exception if it has to execute any consecutive tests. This can be reproduced easily by building this project using the "mvn package" command.
