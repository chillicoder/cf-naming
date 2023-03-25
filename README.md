# cfn-naming

Exercises naming conventions in CloudFormation templates

The intention is to have a standarized way to name resources to prevent duplicates within the same
AWS account.

In this version the structure of the base label is as follows:

* AWS::StackName
* Project
* Environment
    * dev
    * qa
    * stg
    * prod
    * demo

The `Outputs` must be exported with a name build like this:

* AWS::StackName
* `{Name of the Output}`