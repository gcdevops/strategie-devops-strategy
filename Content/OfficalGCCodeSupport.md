## Purpose
To bring [GCCode](https://gccode.ssc-spc.gc.ca) as an officially supported source control solution within the Government of Canada's developer community.

## Existing literature

1. ESDC's Developer Community has [written an article](http://www.gcpedia.gc.ca/wiki/ESDC_Development_Community_-_GC_Code_Recommendation) promoting GCCode as their preferred solution for a standardized source control. The main set back of the tool is that it is unofficially supported, though given its benefits, ESDCs IT Strategy recommends that it should become the officially supported standard for all of the Government of Canada 

2. [A wiki article](https://wiki.gccollab.ca/GCcode/ConceptCase) was written supporting the move towards a government wide standardized source control solution and makes a case for GCCode. The proposed initiative from the article is an integration of GCcode within the GCTools suite

## Background 

The use of source control is a foundational tool for development. As IT infrastructure and processes become ever more complex, new tools and roles are emerging. Information Technology world leaders and best practices promote the use of automation and development tools throughout the lifecycle of an application. In order to properly leverage this modern approach, a shared source control instance is vital. Many opportunities present themselves for individual departments (reference the [ESDC Development Community's GC Code Recommendation article](http://www.gcpedia.gc.ca/wiki/ESDC_Development_Community_-_GC_Code_Recommendation)), though for the Government of Canada as a whole as well. With initiatives such as the OneGov movement from TBS, having a collaborative tool with powerful automation features available, will deliver great benefits to our development communities, who are increasingly responsible for ensuring the delivery of modern useable tools to Canadians. By providing a common place to develop and share development projects and solutions, there is an opportunity to reuse the same platform across departments in most cases. Presently many redundancies exist within departments as they each host and support local instances of varying source control solutions. 


## Situation 

GCCode is an instance of [GitLab Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/), free open source software (FOSS) under the MIT license, hosted by Shared Services Canada (SSC). GCCode is currently supported by SSC with a "when time permits" policy. It runs on production servers and has backups and receives semi-regular updates. GCCode is currently only available within the GoC Intranet, which does block the solution from access 3rd party add-ons and some native features. A number of departments are already storing a large amount of source code on GCCode as their main source control solution. 

### GCCode Stats

**As of May 29th, 2019** GCCode has a record of:
<!-- not all stats may be needed for this, but listing them all for now -->
* 3,614 projects
* 2,998 users
* 2,996 active users
* 507 groups
* 317 forks
* 741 milestones
* 17,280 issues
* 8,778 merge requests
* 155,596 notes
* 394 snippets
* 300 SSH Keys
* 50 distinct email domains (aka GC Organizations)


## Business case 

### Improved Feature Support

With the current (as is) configuration of GCCode, there are a few features that could be supported to increase the viability of the tool.

* **[Pages](https://about.gitlab.com/product/pages/)** could be used for hosting documents and guides on the software in development.
* **Shared [Runners](https://docs.gitlab.com/runner/)** could be capable of deploying directly into SSC infrastructure to manage production and development environments.

With the tool exposed to the internet, there are a few other features that could be used.

* **[Runners](https://docs.gitlab.com/runner/)** could be capable of deploying to cloud infrastructure to manage production and development environments.
* **3rd Party [Integrations](https://docs.gitlab.com/ce/integration/)** could be added to projects for a verity of services.
* **[Repository mirroring](https://docs.gitlab.com/ce/workflow/repository_mirroring.html)** could be enabled for multi-government and citizen collaboration.

With funding for the [GitLab Enterprise Edition (EE)](https://gitlab.com/gitlab-org/gitlab-ee), even more features could be available. The [feature list](https://about.gitlab.com/pricing/self-managed/feature-comparison/) details the improvements available.

### Why GCCode and not GitHub?
There are arguments to support the adoption of GitHub over GCCode. Mainly:

* **Leveraging the GitHub's infrastructure**. The GC will not be able to compete with GitHub's resources and its ability to stay current, so it would be best to use GitHub from the get go and inherit its sustainability capability.
* **Work in complete openness**. GitHub allows GC employees to work in complete openness with the rest of the world. Turning repositories private only when needed.

However, this proposal counters these arguments to the favour of GCCode for the following reasons:
* **Contribute to [GitLab Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/)**. Having a hosted version of GitLab allows the GC to contribute more directly to the GitLab open source project. 
* **Increase comfort level to openness**. Some GC employees and IT Security personnel are currently reluctant to use GitHub due to security risks (e.g. [accidently adding sensitive information like API keys in the repos](https://www.theregister.co.uk/2018/02/07/uber_quit_github_for_custom_code_after_2016_data_breach/)). Using GCCode is expected to augment the GC developer's community best practices around source control and, as such, increase assurance around management and IT Security personnel for open source project meant to be released to the public.
* **Vendor lock in risk management**. GitHub roadmap is determined based on industry funding, not by the GC's interests. Having it's own GitLab instance reduces vendor lock in by allowing GitHub repositories a second home.


## Potential Funding Options

SSC and PSPC-Digital Services Branch are two Departments mandated with providing these types of services to other Government Departments, however both SSC and PSPC-DSB exist within a cost recovery funding model. In order to move forward on this recommendation, it is likely that we will need to identify Departments interested in providing resources to support this recommendation. Below are some potential options:

- Each department which leverages GCCode provides one employee who is responsible one day a week to contribute towards the maintenance and constant improvement of the GitLab instance 

- A flat fee per user per department is charged to those departments using the service

## Supporting members

| Department  	| Name  		| Title 			 	|
|---		|---			|---					|
| ESDC  	| Jayson McIntosh  	| Acting Manager / Technical Advisor  	|
| ESDC		| Remy Bernard		| Manager (on interchange)		|
| ESDC | Shaun Laughland | Programmer Analyst |
| ESDC | Eric Wu | Technical Advisor |
| PSPC | Brittany Hurley | Technical Advisor |
| ESDC | François Brillant | Director |
| SSC | Mathieu Fortin | Director, Partner Enterprise Architecture Liaison |
| IRCC | Luc Schulz | Business Solutions |
| TBS | Roy Saavedra | Research Analyst |
| TC | Vivian Nobrega | Technical Advisor |
| CRA | Nikhil Sebastian | A/IT Specialist |
| PSPC | Steve Trotman | Programmer Analyst |
| TC | Stephen Bakalian | Programmer Analyst |
| PSC | Md Alam | Middleware Operations |
| DFO | Daniel Ricard | Senior Biologist |
| SSC | Jeff Barnes | Senior Advisor |
| DFO | David Fishman | Data Manager |
| CEDQ | Sebastien Metivier | Team Lead - Integration |
| NRCan | Todd McDonald | Senior Programmer |
| TBS | Guillaume Charest | Advisor, Open Source Software |
| ESDC		| Terry Doerksen		| Programmer Analyst		|
| ESDC | Calvin Rodo | Senior Advisor - Application Development
