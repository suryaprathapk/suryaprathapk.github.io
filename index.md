---
layout: default
title: Home
nav_order: 1
description: "ModelN End of Life Tracking Portal"
permalink: /
---

# Model N - End of Life Tracking Portal
{: .fs-9 }

This portal helps track release, support and end of life time lines for the software and libraries in use at Model N.
{: .fs-6 .fw-300 }

---
## Getting started
Click on any software listed on the left  or search for it in the search bar above.

If any of the data mentioned is missing or wrong, please click on the contribute button on the top right corner to report an issue in github to alert the this portal owner. 

This solution can be used in three ways.

### Portal View

Hit on the list of software listed in the list on the left to see the release, support and EOL time lines of the respective software.

A GREEN colored block indicates the software is still in support (Not all libraries have a definitive support date listed, but we have filled in as much as we can get thru manual overriding)

A YELLOW colored block indicates the software is about to reach EOL/ end of active support/ end of security support in the next 180 days. This gives a visual heads up to be prepared and move to latest supported versions

A RED colored block indicates the software has already crossed the EOL/ end of active support/ security support date and our releases has to move away from using these ASAP.

### API for Back end 

We have an API back end inference hosted on AWS API Gateway here : [API LINK](https://t0kdlpsinj.execute-api.us-east-1.amazonaws.com/dev/)

Please reach out to **Bhavani Sankavaram / Surya Kambham** for Access key and secret key information.

A GET Method can be used to get the list of all software.
A POST Method with list of software to get the EOL date in the response

This API can be utilized as part of release workflow & Git CI/CD. 

All it needs is a JSON call with requirements.json file with all the software/libaray used in that product development.

### e-Mail Alerts (WIP)
In the list on the left hand side , there is a menu item called "ModelN Products", all our product's underlying software and libraries are present here

An additional functionality to e-mail product stakeholders periodically with with status of the libraries is in pipeline.


## Ownership
 WHo would own the portal PMO Group/ COPS / any other group ?? 

Knowledge of GitHub is mandatory, merging, handling pull requests, tracking and closing issues reported by our users.

### Maintenance
New software can be added periodically with just new *.md files created for each software (This step is manual for now)

We have evaluated scraping and dumping the dates into the portal, after careful evaluation that part if kept on hold since it is not worth the effort and cost involved.

Changes to Additional software can be suggested using the contribute button in the top right corner (Please provide your comments, and suggested changes and a link to back up the proposed change )



## About the project

This portal is built using Just the Docs Jekyll theme, which is the official theme endorsed by GitHub, built in Ruby.

### License

Just the Docs is distributed by an [MIT license](https://github.com/just-the-docs/just-the-docs/tree/main/LICENSE.txt)