# DBpedia Chatbot

## Environment Configurations
     chatbot.fb.appSecret = <secret>
     chatbot.fb.verifyToken = <token>
     chatbot.fb.pageAccessToken = <access-token>
     
     logging.level.com.github.messenger4j=<log-level>

### Development Only Configurations
     spring.thymeleaf.cache = false

## Deployment
     mvn clean install
     java $JAVA_OPTS -Dserver.port=$PORT -jar target/*.jar
     spring.devtools.livereload.enabled = true

     node/node node_modules/.bin/webpack --watch
     node/node node_modules/.bin/grunt css