## Summary 

ESDC's Developer Community has promoted GCCode as their preferred solution for a standardized source control.  
http://www.gcpedia.gc.ca/wiki/ESDC_Development_Community_-_GC_Code_Recommendation

The main set back of the tool is that it is unofficially supported, though given its benefits, ESDCs IT Strategy recommends that it should become the officially supported standard for all of the Government of Canada 

## Background 

The use of source control is a foundational tool for development. As IT infrastructure and processes become ever more complex, new tools and roles are emerging. Information Technology world leaders and best practices promote the use of automation and development tools throughout the lifecycle of an application. In order to properly leverage this modern approach, a shared source control instance is vital. Many opportunities present themselves for individual departments (reference the ESDC Development Community's GC Code Recommendation article), though for the Government of Canada as a whole as well. With initiatives such as the OneGov movement from TBS, having a collaborative tool with powerful automation features available, will deliver great benefits to our development communities, who are increasingly responsible for ensuring the delivery of modern useable tools to Canadians. 

## Situation 

GCCode is a instance of [GitLab Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/), free open source software (FOSS) under the MIT licence, hosted by Shared Services Canada (SSC). GCCode is currently supported by SSC with a "when time permits" policy. It runs on production servers and has backups and recives simi-regular updates. GCCode is currently only avalibe within the GoC Intranet, which does block the solution from access 3rd party add-ons and some native features. A number of departments are already storing a large amount of source code on GCCode as their main source control solution. 

### Improved Feature Support

With the current (as is) configuration of GCCode, there are a few features that could be supported to increase the viablity of the tool.

* **[Pages](https://about.gitlab.com/product/pages/)** could be used for hosting documents and guides on the software in development.
* **Shared [Runners](https://docs.gitlab.com/runner/)** could be capable of deploying directly into SSC infastructure to manage production and development enviornments.

With the tool exposed to the internet, there are a few other features that could be used.

* **[Runners](https://docs.gitlab.com/runner/)** could be capable of deploying to cloud infastructure to manage production and development enviornments.
* **3rd Party [Integrations](https://docs.gitlab.com/ce/integration/)** could be added to projects for a verity of services.
* **[Repository mirroring](https://docs.gitlab.com/ce/workflow/repository_mirroring.html)** could be enabled for multi-government and citizen collaberation.

With funding for the [GitLab Enterpise Eddition (EE)](https://gitlab.com/gitlab-org/gitlab-ee), even more features could be avaliable. The [feature list](https://about.gitlab.com/pricing/self-managed/feature-comparison/) details the improvements avaliable.

## Support

| Department  	| Name  		| Title 			 	|
|---		|---			|---					|
| ESDC  	| Jayson McIntosh  	| Acting Manager / Technical Advisor  	|
| ESDC		| Remy Bernard		| Manager (on interchange)		|
| ESDC | Shaun Laughland | Programmer Analyst |
