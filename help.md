# Docker on windosw issue - docker-compose bind mount docker.sock not a valid Windows path
Set env variable COMPOSE_CONVERT_WINDOWS_PATHS=1
https://github.com/docker/for-win/issues/1829

# Windows Powershell to stop all running containers:
docker ps -a -q | ForEach { docker stop $_ }


# AWS SQS and SNS
https://www.bountysource.com/teams/spring-cloud/issues?tracker_ids=7680837
# Localstack Commands
https://lobster1234.github.io/2017/04/05/working-with-localstack-command-line/
# Referenced github links for spring cloud aws
https://github.com/spring-cloud-samples/aws-refapp/blob/master/src/main/java/org/springframework/cloud/aws/sample/sqs/SqsController.java

# Stack for i-fxxxxxx does not exist AWS Cloud Starter
https://stackoverflow.com/questions/45818092/spring-boot-startup-error-for-aws-application-there-is-not-ec2-meta-data-avail
https://github.com/spring-cloud/spring-cloud-aws/issues/121

# SNS subscription
http://cloud.spring.io/spring-cloud-aws/spring-cloud-aws.html#_annotation_driven_http_notification_endpoint
https://stackoverflow.com/questions/36040800/spring-aws-cloud-sns-http-end-point-confirm-subscription-not-working
https://github.com/spring-cloud/spring-cloud-aws/blob/147420f4d86806b921d4d7533813d11d73692fb5/spring-cloud-aws-messaging/src/main/java/org/springframework/cloud/aws/messaging/config/annotation/SnsWebConfiguration.java

# Read file from S3  using lambda 
https://stackoverflow.com/questions/30651502/how-to-get-contents-of-a-text-file-from-aws-s3-using-a-lambda-function

# Subscribing to S3 Event through Cloudformation
https://stackoverflow.com/questions/38752985/create-a-lambda-notification-in-an-s3-bucket-with-cloudformation?rq=1

# Invoking Lambda from SNS
https://stackoverflow.com/questions/39689228/why-is-sns-not-triggering-my-lambda
https://aws.amazon.com/blogs/mobile/invoking-aws-lambda-functions-via-amazon-sns/

# aws lambda with spring boot
https://github.com/awslabs/aws-serverless-java-container/wiki/Quick-start---Spring-Boot
Handler class not FoundException
https://stackoverflow.com/questions/36081908/using-spring-boot-cloud-with-amazon-aws-lambda-does-not-inject-values
# Project that helped aws lambda with spring boot Handler class not FoundException
https://github.com/mengjiann/aws-lambda-s3/blob/master/pom.xml 

# git discard all changes and pull from upstream
git reset --hard origin/master
git pull origin master


# find process running on port and kill process on Windows
netstat -ano | findstr :<yourPortNumber>
taskkill /PID <typeyourPIDhere> /F

https://docs.spring.io/spring/docs/current/spring-framework-reference/integration.html#jms

# Lombok
If you use STS. You must have Lombok installed in your Eclipse by running lombok-xyz.jar
Please Try the Following the Steps:
Include pom in Maven .
Exit/Shutdown STS
Find lombok Jar in ~/.m2/repository/org/projectlombok/lombok/version.x
From Command Prompt/Shell java -jar lombok-1.x.y.jar 

# SSL issues
http://magicmonster.com/kb/prg/java/ssl/pkix_path_building_failed.html
http://www.javasavvy.com/import-ssl-certificate-into-java-keystore/

# sqslistener-with-threadpoolexecutor
https://stackoverflow.com/questions/50070384/sqslistener-with-threadpoolexecutor


# MYSQL running on Windows
https://stackoverflow.com/questions/13752424/how-to-connect-from-windows-command-prompt-to-mysql-command-line

# Rules of threadpoolExecutor Poolsize
http://www.bigsoft.co.uk/blog/2009/11/27/rules-of-a-threadpoolexecutor-pool-size
# JMS Patterns
https://docs.oracle.com/cd/E13171_01/alsb/docs25/interopjms/MsgIDPatternforJMS.html

# PowerMock

https://stackoverflow.com/questions/20754432/powermock-mockito-not-working


# Custom scopes in spring:
https://stackoverflow.com/questions/50477894/spring-custom-scope-lifecycle-bean-termination
http://iryndin.net/post/spring_destroy_prototype_beans/
https://www.javadevjournal.com/spring/spring-custom-scope/

# Spring Cache with EHCache
https://stackoverflow.com/questions/26927044/how-to-load-data-from-database-to-ehcache-when-the-application-starts
https://javaglobin.wordpress.com/2013/11/13/declarative-caching-with-spring/
http://www.ehcache.org/blog/2016/05/18/ehcache3_jsr107_spring.html
https://stackoverflow.com/questions/52518312/cacheable-doesnt-intercept-the-method-cache-is-always-empty

# Completable Future
https://www.nurkiewicz.com/2015/11/which-thread-executes.html
https://medium.com/@senanayake.kalpa/fantastic-completablefuture-allof-and-how-to-handle-errors-27e8a97144a0
https://www.nurkiewicz.com/2014/11/executorservice-10-tips-and-tricks.html

# 5 things you didn't know about ...Multithreaded Java programming
https://www.ibm.com/developerworks/library/j-5things15/index.html


# AWS study material
https://www.quora.com/How-did-you-prepare-for-AWS-Certified-Solutions-Architect-Associate-Level-certification#

# pause listening messages in jMS listener
https://stackoverflow.com/questions/625725/how-to-temporarily-disable-a-message-listener

# JmsTemplate using CachingConnectionFactory, async sends
http://chriswongdevblog.blogspot.com/2013/01/jmstemplate-is-not-evil.html =Cache
# JMS tuning
https://bsnyderblog.blogspot.com/2010/02/using-spring-jmstemplate-to-send-jms.html
https://bsnyderblog.blogspot.com/2010/05/tuning-jms-message-consumption-in.html
https://bsnyderblog.blogspot.com/2010/05/tuning-jms-message-consumption-in.html


# Tuning RestTemplate
https://tech.asimio.net/2016/12/27/Troubleshooting-Spring-RestTemplate-Requests-Timeout.html

# JMS hystrix
https://github.com/soudmaijer/spring-jms-hystrix



# aws document DB connection
https://braytonstafford.com/2018/03/27/importing-aws-rds-pem-certificate-to-java-keystore/
https://stackoverflow.com/questions/54230901/attaching-aws-documentdb-to-spring-boot-application


# Shopping cart
https://o7planning.org/en/10683/create-a-shopping-cart-web-application-with-spring-boot-hibernate#a14223762
Insert image into H2 DB
https://stackoverflow.com/questions/38353487/insert-blob-from-a-file-into-a-sql-script-to-embed-h2-database

# Thymleaf
https://stackoverflow.com/questions/26632529/how-to-set-servletcontext-property-for-a-bean-in-spring-xml-metadata-configurati
https://stackoverflow.com/questions/38057341/failed-to-instantiate-org-thymeleaf-templateresolver-servletcontexttemplatereso


https://stackoverflow.com/questions/48089021/spring-test-cannot-get-spring-configuration-beans

# Lambda SSL issues
https://medium.com/i-me-myself-naveen/java-ssl-within-aws-lambda-39f87c1c03f2

# Calling SSL enabled RESTful service from JAVA
https://www.youtube.com/watch?v=arxCYazXJ_g

# SKIP SSL CERTIFICATE VERIFICATION IN SPRING REST TEMPLATE
https://blog.codeleak.pl/2016/02/skip-ssl-certificate-verification-in.html


# Maven assembly - zipiing classes
https://github.com/aws/aws-lambda-java-libs/issues/2#issuecomment-314539625

# Spring boot and aws parameter store
https://source.coveo.com/2018/08/03/spring-boot-and-aws-parameter-store/

# Testing async methods with Mockito
https://fernandocejas.com/2014/04/08/unit-testing-asynchronous-methods-with-mockito/

# Testing Rest API with Request Parameters
https://stackoverflow.com/questions/14124110/spring-mvc-testframework-fails-with-http-response-406
# solution which worked
https://stackoverflow.com/questions/17972428/mock-mvc-add-request-parameter-to-test
https://stackoverflow.com/questions/24044553/spring-controller-integration-test-fails-to-parse-response-and-fails-the-test-wi

# spring-mvc-webapp-schedule-java-sdk-http-connection-reaper-failed-to-stop
https://stackoverflow.com/questions/18069042/spring-mvc-webapp-schedule-java-sdk-http-connection-reaper-failed-to-stop

# KMS Service
https://github.com/devender/envelope-encryption-aws/tree/master/src/main/java/com/gdr/aws/kms 

# Spring Transactional Isolation Propogation
https://stackoverflow.com/questions/8490852/spring-transactional-isolation-propagation


# AWS Athena
https://docs.aws.amazon.com/code-samples/latest/catalog/java-athena-src-main-java-aws-example-athena-ListQueryExecutionsExample.java.html
# AWS Glue
https://medium.com/searce/convert-csv-json-files-to-apache-parquet-using-aws-glue-a760d177b45f


# Spring MVC Showcase
https://github.com/spring-projects/spring-mvc-showcase

# Spring mvc tests
https://github.com/pkainulainen/spring-mvc-test-examples/blob/master/controllers-unittest/pom.xml

# MongoLookup Spring data
https://stackoverflow.com/questions/45860117/how-to-use-aggregation-query-with-mongoitemreader-in-spring-batch

# Send data secure with sftp and spring batch
https://blog.codecentric.de/en/2011/09/send-data-secure-with-sftp-and-spring-batch/

# Trace ID in Sleuth
https://github.com/spring-cloud/spring-cloud-sleuth/issues/206

# Config Client pull behavior
https://github.com/codecentric/spring-boot-admin/issues/667

# Encryption Decryption
https://proandroiddev.com/security-best-practices-symmetric-encryption-with-aes-in-java-7616beaaade9
https://proandroiddev.com/security-best-practices-symmetric-encryption-with-aes-in-java-and-android-part-2-b3b80e99ad36

# Key Management Service Guide
https://info.townsendsecurity.com/definitive-guide-to-encryption-key-management-fundamentals
