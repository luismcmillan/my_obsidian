- [[Shell]]
```Shell
#!/bin/bash

if lsof -i:10002 > /dev/null 
then
    echo "Port 10002 ist belegt."
    java -jar ~/Documents/Java-projects/reporting_problem/Reporting_app/target/Reporting_app-1.0-SNAPSHOT.jar
else
    osascript -e 'tell application "Terminal" to do script "java -jar ~/Documents/Java-projects/reporting_problem/Reporting_app/target/Reporting_app-1.0-SNAPSHOT.jar; exec bash"'
    aws-config workload dev dc && source ~/.aws/current_profile
    acd dev-dsdcom-reporting-postgres
    
fi
```