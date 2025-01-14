# ua-jenkins

The ConnectALL Jenkins Universal Adapter is developed as an extension to the universal adapter capability of ConnectALL. This adapter will allow the user to use Jenkins with ConnectALL. Current capabilities and limitations will be defined below.

Please refer to the [ConnectALL Tech Docs](https://techdocs.broadcom.com/us/en/ca-enterprise-software/valueops/connectall/3-6/adapters/universal-adapter.html) for more information.

If you are an existing SaaS customer, please contact Broadcom Support to enable the adapter in your environment. If you are using ConnectALL On-Premise, you may download and install this adapter in your environment. If you are not yet a customer, [please reach out to learn more](https://enterprise-software.broadcom.com/contact-us).

# Setup

## Supported Entities

This Universal Adapter currently supports the following entities:
* Build Results

*Note: This Universal Adapter is provided as-is. It is tested and validated using the entities and configurations as defined. Any additional customizations are not supported and should be made at your own discretion.*

## Connection Details

* **Connection Name:** *Name of Application*
* **Application Type:** Jenkins
* **URL:** Any - this will not be used, but a value is still required.
* **User Name:** Leave Blank
* **Password:** Leave Blank
* **Application Category:** *Pick from dropdown list*
* **Time Zone:** Leave Blank
* **Select Group:** *Set if neccessary*

## Flow Filters

Flow Filters are not used for this adapter.

## Example Automation

When a Jenkins Job is completed, compile the results in a shell script, then push the results to a ConnectALL automation to ValueOps Insights. The shell script used by your pipeline can either be local to Jenkins or it can be called from an external code repsitory.

# Known Limitations

Available fields are limited to what can be captured by variables during the pipeline execution.
