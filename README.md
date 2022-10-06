# Reindex-Check -- Always test in non-production first. 

# Update Groovy logic to have your sql server name and jira database name

# Jenkins Agent needs to have a directory created /home/jenkins with a file called web-team-config.properties

         web-team-config.properties needs to have the following format
                jira-reindexer-username=<JIRA ADMIN USER>
                jira-reindexer-password=<JIRA ADMIN USER PASSWORD
                rqmdb-username=<SQL User>
                rqmdb-password=<SQL User>
      
# Jenkins Master need the following installed
          https://plugins.jenkins.io/matrix-project
          https://plugins.jenkins.io/config-file-provider
          https://plugins.jenkins.io/mailer
          
          
    
# Jenkins Master Configuration Matrix Setup
           Update labels to the label for your agents and update the nodes for all the nodes in your DC cluster (Does work on JIRA server)
          ![image](https://user-images.githubusercontent.com/115188099/194411336-02890d20-a032-48d9-ae64-d8551c7e26c5.png)
          
# Jenkins Master Configuration Files Setup
           Location and name of the web-team-config.properties
          ![image](https://user-images.githubusercontent.com/115188099/194410829-74d57168-f54c-428f-9303-0a4b0980edb8.png)
          
          
