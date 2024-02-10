#!groovy
@Library('roboshop-shared-library') _



//Responsibility to pass what type of application and component

def configMap = [
    application: "nodejsVM",
    component: "catalogue"
]
if( ! env.BRANCH_NAME.equalsIgnoreCase('master')){
    pipelineDecission.decidePipeline(configMap)
}
else{
    echo "This is PRODUCTION, deal with CR process"
}