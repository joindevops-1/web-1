#!groovy
@Library('roboshop-shared-library') _

// responsibility to pass what type of application and component is this to pipeline deicssion

def configMap = [
    application: "staticVM",
    component: "web"
]
if( ! env.BRANCH_NAME.equalsIgnoreCase('main')){
    pipelineDecission.decidePipleine(configMap)
}
else{
    echo "This is PRODUCTION, deal with CR process"
}