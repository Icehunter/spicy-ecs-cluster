#!/usr/bin/env groovy

@Library(["spicy-automation@development"]) _

spicyECSCluster(
    pipelineProperties: [pipelineTriggers([cron('0 10 * * 1-4')])],
    devAccount: accounts.get().SPICY_US_EAST_1_DEV,
    sandboxAccount: accounts.get().SPICY_US_EAST_1_SANDBOX,
    stagingAccount: accounts.get().SPICY_US_EAST_1_STAGING,
    prodAccount: accounts.get().SPICY_US_EAST_1_PROD,
    stackName: "spicy-ecs"
)
