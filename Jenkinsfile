#!/usr/bin/env groovy
import groovy.json.JsonSlurper;


node() {
    def pipeline;
    
    //colors
    def ANSI_RESET = "\u001B[0m"
    def ANSI_RED = "\u001B[31m"
    def ANSI_GREEN = "\u001B[32m"
    def ANSI_BLUE = "\u001B[34m"
    def branchName = env.BRANCH_NAME;
    def snapshotVersion = "0.1.0";

    properties(
        [
            parameters(
                [
                    booleanParam(defaultValue: false,
                            description: 'Update the defaut service level configurations with service specific ones',
                            name: 'UPDATE_SERVICE_OUTLIERS'),                   
                    string(defaultValue: 'https://kong-dev-admin.gateway.aws.athenahealth.com',
                            description: 'Kong admin URL',
                            name: 'ADMIN_URL'),
                    
                ]
            )
        ]
    );

    // stage('Prepare pipeline') {
    //     pipeline = new cicd.Pipeline();
    //     pipeline.cleanupAndCheckout();
    // }
    
    if(env.UPDATE_SERVICE_OUTLIERS == 'true') {
       
        def myfile = readFile("./file.txt")
        
        echo "${myfile}"
       
    
    }

}
