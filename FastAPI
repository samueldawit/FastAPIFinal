from http.client import HTTPException
from fastapi import FastAPI
import os
from pydantic import BaseModel
from typing import Optional, Literal

app = FastAPI()

# Partner Model
class Partner(BaseModel):
    name: str
    partner_level: str
    partner_field: Literal["Gateway","Git","APM","CI/CD","API Monitoring","Storage","API Observeability","Workflows","Collaboration","Open Specification","Incident response","API Visualization","API security","API Automation","API Testing"]
    partner_id: Optional[str]


PARTNER_FILE = "partners"
PARTNER_DATABASE = [
"APIMatic",
"AWS API Gateway",
"Azure API Gateway",
"Azure DevOps",
"BigPanda",
"BitBucket",
"BitBucket Pipelines",
"CircleCI",
"Coralogix",
"Datadog",
"Dropbox",
"Github",
"Github Actions",
"GitLab",
"GitLab CI/CD",
"Jenkins",
"Keen",
"Lightstep",
"Micrsoft Power Automate",
"Microsoft Teams",
"New Relic",
"Open API",
"OpsGenie",
"PagerDuty",
"Splunk",
"Splunk On-Call",
"Slack",
"Statuspage",
"Travis CI",
"Helios",
"Appmap",
"APIsec",
"Workato",
"Speedscale",
"Pynt"
]



#/
@app.get("/")
async def home():
        return{"Message": "Welcome to Postmans new Integration partner API!"}

#/list-partners
@app.get("/list-partners")
async def list_partners():
    return{"partners": PARTNER_DATABASE}

    
#get-partner
@app.get("/APIMatic")
async def APIMatic():
        return {"partner": "APIMatic",
        "partnerlevel":"Strategic",
        "description":"Postmans APIMatic integration converts a Postman collection into an API description format such as Swagger, RAML, or API Blueprint, and then periodically backs up the resulting file on GitHub."
        }

@app.get("/AWS-API-Gateway")
async def AWS_API_Gateway():
        return {"partner": "AWS API Gateway",
        "PartnerLevel":"Strategic",
        "description":"You can upload your API schemas directly to AWS API Gateway from Postman with this integration. It uses version 2 of the AWS API and only supports HTTP APIs with OpenAPI 3.0 schemas. Once the integration is configured, any new changes to your schema in Postman will also appear in your AWS API Gateway."
        }

@app.get ("/Azure-API-Gateway")
async def Azure_API_Gateway():
    return {"partner": "Azure-API-Gateway",
    "PartnerLevel":"Strategic",
    "description":"View deployments for each of your Azure API Management services. You can see the revision history, changelog, and export history. You can also export your API definition from Postman to Azure API Management."
    }

@app.get ("/Azure-DevOps")
async def Azure_DevOps():
    return {"partner": "Azure-DevOps",
    "PartnerLevel":"Strategic",
    "description":"Sync your Postman APIs to Microsoft Azure DevOps, an open-source Git repository manager."
    }

@app.get ("/BitBucket")
async def BitBucket():
    return {"partner": "BitBucket",
    "PartnerLevel":"Strategic",
    "description":"Back up your team's Postman collections with Postman's Bitbucket integration."
    }

@app.get ("/BitBucket-Pipelines")
async def BitBucket_Pipelines():
    return {"partner": "BitBucket-Pipelines",
    "PartnerLevel":"Strategic",
    "description":"Bitbucket Pipelines is a CI/CD service that's integrated with Bitbucket Cloud. View the status of builds or start a new build, all from within Postman."
    }

@app.get ("/CircleCI")
async def CircleCI():
    return {"partner": "CircleCI",
    "PartnerLevel":"Strategic",
    "description":"CircleCI is a cloud-based (CI/CD) platform. You can view the status of builds or start a new build, all from within Postman"
    }

@app.get ("/Coralogix")
async def Coralogix():
    return {"partner": "Coralogix",
    "PartnerLevel":"Strategic",
    "description":"Coralogix is a machine learning-powered log analytics platform that improves the delivery and maintenance process.Configure your Postman Monitors to send metrics to Coralogix, where you can visualize and compare them."
    }

@app.get ("/Datadog")
async def Datadog():
    return {"partner": "Datadog",
    "partnerlevel":"Strategic",
    "description":"Datadog is a monitoring service for cloud-scale applications. Configure your Postman Monitors to send metrics to Datadog, where you can visualize and compare them with other metrics."
    }

@app.get ("/Dropbox")
async def Dropbox():
    return {"partner": "Dropbox",
    "partnerlevel":"Strategic",
    "description":"Back up and synchronize your Postman collections on Dropbox, keeping your Postman collections and other project files in one place."
    }

@app.get ("/Github")
async def Github():
    return {"partner": "Github",
    "partnerlevel":"Strategic",
    "description":"Back up your Postman collections to GitHub, a cloud-based hosting service for Git repositories."
    }

@app.get ("/Github Actions")
async def Github_Actions():
    return {"partner": "Github Actions",
    "partnerlevel":"Strategic",
    "description":"GitHub Actions is a CI/CD service that's integrated with GitHub. After you set up the integration, you can view the status of builds from within Postman."
    }

@app.get ("/GitLab CI/CD")
async def GitLab_CI_CD():
    return {"partner": "GitLab CI/CD",
    "partnerlevel":"Strategic",
    "description":"GitLab CI/CD is integrated with GitLab SaaS and GitLab self-managed. After you set up the integration, you can view the status of builds or start a new build, all from within Postman."
    }

@app.get ("/Jenkins")
async def Jenkins():
    return {"partner": "Jenkins",
    "partnerlevel":"Strategic",
    "description":"Jenkins is an open source automation server that can act as CI/CD hub. you can view the status of builds or start a new build, all from within Postman."
    }

@app.get ("/Keen")
async def Keen():
    return {"partner": "Keen",
    "partnerlevel":"Strategic",
    "description":"You can use Keen IO for API-based computation, Amazon S3 backups, and building visualizations and dashboards for your APIs. Connect your Postman Monitor results to Keen Streams with the Postman to Keen Integration."
    }

@app.get ("/Lightstep")
async def Lightstep():
    return {"partner": "Lightstep",
    "partnerlevel":"Strategic",
    "description":"Lightstep Incident Response is an incident response platform from ServiceNow, which offers the ability to observe, assess, resolve, and escalate alerts and issues in enterprise and DevOps applications."
    }

@app.get ("/Micrsoft-Power-Automate")
async def Micrsoft_Power_Automate():
    return {"partner": "Micrsoft-Power-Automate",
    "partnerlevel":"Strategic",
    "description":"Microsoft Power Automate enables you to automate workflows between your favorite apps and services to get notifications, synchronize files, collect data, and more. It offers over 140 services with predefined flows that you can implement."
    }

@app.get ("/Microsoft-Teams")
async def Microsoft_Teams():
    return {"partner": "Microsoft-Teams",
    "partnerlevel":"Strategic",
    "description":"Microsoft Teams is a chat-based workspace available to all Microsoft Office 365 users. This integration enables you to get updates about your Postman team directly in Microsoft Teams."
    }

@app.get ("/New-Relic")
async def New_Relic():
    return {"partner": "New Relic",
    "partnerlevel":"Strategic",
    "description":"New Relic is an application performance management solution to monitor real-time and trending data for your processes or web apps. Using Postman's New Relic integration, you can send Postman monitor results to New Relic."
    }

@app.get ("/OpenAPI")
async def OpenAPI():
    return {"partner": "OpenAPI",
    "partnerlevel":"Strategic",
    "description":"You can import your existing OpenAPI 3.0 and 3.1 definitions (OpenAPI Specification) into Postman. Postman supports both YAML and JSON formats. You can choose to upload a file, enter a URL, or directly copy your JSON/YAML."
    }

@app.get ("/OpsGenie")
async def OpsGenie():
    return {"partner": "OpsGenie",
    "partnerlevel":"Strategic",
    "description":"Opsgenie is an incident management and alerting tool that enables you to manage alerts. It has several communication features such as SMS, phone calls, and mobile push notifications, and collaboration features such as escalations and schedules."
    }

@app.get ("/PagerDuty")
async def PagerDuty():
    return {"partner": "PagerDuty",
    "partnerlevel":"Strategic",
    "description":"PagerDuty is an incident management solution that integrates with monitoring stacks for alerting, on-call scheduling, and automatic escalation of critical incidents."
    }

@app.get ("/Splunk")
async def Splunk():
    return {"partner": "Splunk",
    "partnerlevel":"Strategic",
    "description":"Splunk is a monitoring service for cloud-scale applications. It combines data from servers, databases, tools, and services to present a unified view of an entire stack. This integration allows you to configure your Postman Monitors to send metrics to Splunk where you can visualize and compare them with other metrics."
    }

@app.get ("/Splunk-On-Call")
async def Splunk_On_Call():
    return {"partner": "Splunk-On-Call",
    "partnerlevel":"Strategic",
    "description":"Splunk On-Call (formerly VictorOps) is a real-time incident management platform that handles incidents as they occur and prepares for the next one."
    }

@app.get ("/Slack")
async def Slack():
    return {"partner": "Slack",
    "partnerlevel":"Strategic",
    "description":"The Postman to Slack integration enables you to send Postman notifications to a Slack channel. You can send the results of a Postman monitor run, notifications received in the Postman notification center, activity in your Team Activity Feed, or uptime monitor notifications."
    }

@app.get ("/Statuspage")
async def Statuspage():
    return {"partner": "Statuspage",
    "partnerlevel":"Strategic",
    "description":"Atlassian Statuspage is an uptime and incident communication tools. You can use Statuspage to create a home page for your customers so they can monitor if subsystems or services within your site are operational, and find out more information on system outages or failures. An example of a Statuspage home page is Postman's status page, located at status.postman.com."
    }

@app.get ("/Travis-CI")
async def Travis_CI():
    return {"partner": "Travis-CI",
    "partnerlevel":"Strategic",
    "description":"Travis CI is continuous integration (CI) platform that software development teams use to automatically build and test code changes. With Travis CI, developers can get immediate feedback on the success of a change."
    }

@app.get ("/Helios")
async def Helios():
    return {"partner": "Helios",
    "partnerlevel":"integration",
    "description":"Helios is an observability, troubleshooting, and testing platform for microservices. Using distributed tracing, developers can pinpoint and analyze issues, reproduce scenarios and then generate tests for APIs, microservices, messaging systems, data pipelines, and databases."
    }

@app.get ("/Helios")
async def Helios():
    return {"partner": "Helios",
    "partnerlevel":"integration",
    "description":"Helios is an observability, troubleshooting, and testing platform for microservices. Using distributed tracing, developers can pinpoint and analyze issues, reproduce scenarios and then generate tests for APIs, microservices, messaging systems, data pipelines, and databases."
    }

@app.get ("/Appmap")
async def Appmap():
    return {"partner": "Appmap",
    "partnerlevel":"integration",
    "description":"AppMap is an open source tool thousands of developers use to visualize their application's runtime behavior. Unlike static analyzers, AppMap records how an application runs and uses that information to find design flaws, security holes, and performance issues."
    }

@app.get ("/APIsec")
async def APIsec():
    return {"partner": "APIsec",
    "partnerlevel":"integration",
    "description":"EthicalCheck from APIsec is a free and instant API penetration testing service. It is offered as self-service, fully automated, and requires no signup. And, it’s user-friendly with an intuitive web UI, an API, and a GitHub action to integrate API security testing in dev workflows."
    }

@app.get ("/Workato")
async def Workato():
    return {"partner": "Workato",
    "partnerlevel":"integration",
    "description":"Workato helps automate business workflows across cloud and on-premises apps. Increase visibility of any API collection by syncing it to your Postman workspace. There, you can make use of the internal and external portal to drive adoption."
    }

@app.get ("/Speedscale")
async def Speedscale():
    return {"partner": "Speedscale",
    "partnerlevel":"integration",
    "description":"Speedscale can export and import traffic in the open source Postman collection format. This lets you use your familiar tools to send test transactions to your app with traffic that was collected by Speedscale."
    }

@app.get ("/Pynt")
async def Pynt():
    return {"partner": "Pynt",
    "partnerlevel":"integration",
    "description":"https://www.youtube.com/watch?v=YWB57GHOPHU&ab_channel=Pynt"
    }

#/partner-by-level{index} /partner-by-index/0
@app.get("/partner-by-index/{index}")
async def partner_by_index(index:int):
    if index <0 or index >= len(PARTNER_DATABASE):
        raise HTTPException(404, f"Index {index} is out of range {len(PARTNER_DATABASE)}.")
    else:
            return{"partners":PARTNER_DATABASE[index]}
