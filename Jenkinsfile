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
                            description: 'Run Integration Tests',
                            name: 'RUN_TESTS'),
                    booleanParam(defaultValue: false,
                            description: 'Build athena kong image',
                            name: 'BUILD_KONG_IMAGE'),
                    booleanParam(defaultValue: false,
                            description: 'DO Deployment',
                            name: 'DO_DEPLOYMENT'),
                    booleanParam(defaultValue: false,
                            description: 'Enable plugins',
                            name: 'ENABLE_PLUGINS'),
                    string(defaultValue: 'https://kong-dev-admin.gateway.aws.athenahealth.com',
                            description: 'Kong admin URL',
                            name: 'ADMIN_URL'),
                    string(defaultValue: 'http://gatewaynode.dev.api.athena.io/scopes/verify',
                            description: 'Authorization URL',
                            name: 'AUTH_URL')
                ]
            )
        ]
    );

    // stage('Prepare pipeline') {
    //     pipeline = new cicd.Pipeline();
    //     pipeline.cleanupAndCheckout();
    // }

}
