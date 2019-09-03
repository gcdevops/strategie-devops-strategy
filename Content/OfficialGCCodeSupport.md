# Official GC/Code Support

## Purpose

To recommend the adoption of a decentralized version control system for all IT personnel in order to enable wider collaboration within the Government of Canada as well as support advanced and modern DevOps capabilities.

## Context

The latest updates to the [Directive on Management of IT](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=15249) have clearly identified 3 main requirement changes related to source code management in the GoC:

1. If a custom-built application is the appropriate option, **by default any source code written by the government must be released** in an open format via Government of Canada websites and services designated by the Treasury Board of Canada Secretariat [(C.2.3.8.3)](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=15249#claC.2.3.8.3);
2. All source code must be released under an appropriate **open source software licence** [(C.2.3.8.4)](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=15249#claC.2.3.8.4);
3. Share code **publicly** when appropriate, and when not, share **within** the Government of Canada [(C.2.3.9.5)](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=15249#claC.2.3.9.5).

The use of source code version control is indeed a foundational tool for software development but each department currently manages its own source code independently. More so, there are even instances where multiple methods and solutions are in place to manage source code versioning within a single organization.

However, as IT infrastructure, environments and processes become more complex and abstract, new tools and roles are emerging. Information Technology world leaders and best practices promote the use of automation and development tools throughout the lifecycle of an application, not only through the coding phase.
In order to properly leverage this modern approach, a decentralized version control system with collaborative capabilities is vital.

Many opportunities present themselves for individual departments (reference the [ESDC Development Community's GC Code Recommendation article](https://github.com/esdc-edsc/Welcome/blob/master/Recommendations/GCcode.md)), though for the Government of Canada as a whole as well.
With initiatives such as the OneGov movement and the GCTools from TBS, having a collaborative tool with powerful automation features available would deliver great benefits to our development communities, who are increasingly responsible for ensuring the delivery of modern services to Canadians.
By providing a common place to develop and share development projects and solutions, there is an exceptional opportunity to reuse the same platform across departments in most cases.
Presently, many redundancies exist within departments as they each host and support local instances of varying source control solutions.

## Existing literature

1. ESDC's Developer Community has written an [article](https://github.com/esdc-edsc/Welcome/blob/master/Recommendations/GCcode.md) providing guidelines on how to manage ESDC's projects in GC/Code.
2. A [wiki page](https://wiki.gccollab.ca/GCcode/ConceptCase) was written supporting the move toward a government-wide standardized source control solution and makes a case for GC/Code. The proposed initiative from the article is an integration of GC/Code within the GCTools suite.
3. The Government of Canada Open Source Advisory Board started writing a [business case](https://github.com/canada-ca/OS-Advisory_Conseil-SO/blob/master/en/Working_Group_Tools/gc-source-code-repo.md) for a Source Code Platform to enable central hosting and sharing of source code.

## Current State

GC/Code is an instance of [GitLab Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/), free open source software (FOSS) under the MIT licence, hosted by Shared Services Canada (SSC).
GC/Code is currently unofficially supported by SSC with a "best effort" policy. It runs on production servers and has backups and receives semi-regular updates. GC/Code is currently only available within the GoC Intranet, which blocks the solution from access to 3rd party add-ons and some native features. A number of departments are already storing a large amount of source code on GC/Code.

### GC/Code Stats

As of May 2019, GC/Code has a record of ≈3600 projects and ≈3000 users (350+ being from ESDC) from 50 GC organizations, with more than 17k issues and 8k merge requests having been created.

<!-- 
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
 -->

## Business case

To bring [GC/Code](https://gccode.ssc-spc.gc.ca) as an officially supported source control solution for the Government of Canada's developer community.

### Benefits to ESDC Business Lines

#### IITB

* Strengthen relationship between IT and business through a centralized collaboration platform
* Improve the quality and security of code with automated testing (e.g. static code analysis to detect hard coded passwords)
* Accelerate the rate of application development and deployments through a modern tool (in constant evolution)
* Easily find and reuse source code from other projects, including from other departments
* Receive notifications and send actions from instant messaging platform (e.g. Slack)
* Obtain metrics/statistics for reporting and continuous improvement
* Edit files without leaving the browser

#### Existing Development Projects (e.g. Old Age Security)

* Reduce costs of version control systems
* Off-load maintenance responsibilities to centralized GC resources
* Enable static code analysis to promote better security and development practises, through detection of:
  * Hard-coded passwords
  * Non-parametized SQL queries
  * Dependencies with known security vulnerabilities
  * Bad coding practice (unused variables [clutered namespaces])
  * Lack of automated testing code coverage
  * Inefficient code
* Benefit from a common development platform:
  * Leverage functionalities covering the full development lifecycle from a single tool (code, issues/tasks, tests, etc.), in particular the automation of builds, tests, and deployments.
  * Facilitate adoption/training by staff
  * Centralize conversations (instead of using emails)
* Enhance planning of features development through a single view
* Track time spent on project tasks
* Ensure accountability through logging of changes and incidents
* Publish webpages related to project (with official GC look and feel as an option)
* Improve code quality and collaboration by developing in the open, thereby reducing overall risk

### Additional Features

With the current (as is) configuration of GC/Code, additional features could be enabled to increase the viability of the tool:

* **[Pages](https://about.gitlab.com/product/pages/)** – To host documents and guides on the software in development, and even static websites including ones with GoC official theme.
* **[Internal Runners](https://docs.gitlab.com/runner/)** – For deployment directly to SSC infrastructure to manage production and development environments.

With the tool exposed to the internet, even more features could be leveraged:

* **[Cloud Runners](https://docs.gitlab.com/runner/)** – For deployment to cloud infrastructure to manage production and development environments.
* **[3rd Party Integrations](https://docs.gitlab.com/ce/integration/)** – To add a variety of services to projects.
* **[Repository mirroring](https://docs.gitlab.com/ce/workflow/repository_mirroring.html)** – For multi-government and citizen collaboration.

With funding for the [GitLab Enterprise Edition (EE)](https://gitlab.com/gitlab-org/gitlab-ee), even more [advanced features](https://about.gitlab.com/pricing/self-managed/feature-comparison/) could be made available.

### Why GC/Code and not GitHub?

There are arguments to support the adoption of GitHub over GC/Code. Mainly:

* **Leveraging GitHub's infrastructure**  
The GC will not be able to compete with GitHub's resources and its ability to stay current, so it would be best to use GitHub from the get go and benefit from its sustainability capability.
* **Work in complete openness**  
GitHub allows GC employees to work in complete openness with the rest of the world, turning repositories private only when needed.

However, this proposal counters these arguments to the favour of GC/Code for the following reasons:

* **Increase comfort level to openness**  
Some GC employees and IT Security personnel are reluctant to use GitHub due to security risks (e.g.: [accidentally adding sensitive information like API keys in the repos](https://www.theregister.co.uk/2018/02/07/uber_quit_github_for_custom_code_after_2016_data_breach/)).
Using GC/Code is expected to augment the GC developer's community best practices around source control and, as such, increase assurance around management and IT Security personnel for open source project meant to be released to the public.
* **Vendor lock-in risk management**  
GitHub roadmap is determined based on industry funding, not by the GC's interests. Having our own internal instance running on open source software reduces vendor lock-in by allowing GitHub repositories a second home.
* **Potential Cost Savings**  
Although a more fulsome cost evaluation should be performed when this proposal is adopted, it is believed that maintaining an internal instance would result in cost savings due to the requirement to host private repositories at the GC level.
* **Contribute to [GitLab Community Edition (CE)](https://gitlab.com/gitlab-org/gitlab-ce/)**  
Having a hosted version of GitLab allows the GC to contribute more directly to the GitLab open source project.

## Recommendation

We recommend that GC/Code becomes the official internal version control platform for the GC and that ESDC contributes toward this goal (e.g. funding through MOU) as it directly benefits from the platform.

We anticipate that the following work will be needed:

1. Commence discussions with SSC CIO ADDA (Application Development and Database Administration) team responsible for the current service;
2. Determine and plan evolution of the service (e.g. business model, service levels, hosting environment, additional features);
3. Present to relevant committees;
4. Set funding agreement(s) with ESDC and other departments as required;
5. Implement technical changes and formalize a support team within SSC; and
6. Rebrand the platform accordingly.

## Supporting members

| Department | Name | Title |
|--- |--- |--- |
| ESDC | Jayson McIntosh | Acting Manager / Technical Advisor |
| ESDC | Remy Bernard | Manager (on interchange) |
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
| SSC | Jeff Barnes | Senior Advisor |
| DFO | Daniel Ricard | Senior Biologist |
| DFO | David Fishman | Data Manager |
| DFO | Pablo Vergara | Data Manager |
| CEDQ | Sebastien Metivier | Team Lead - Integration |
| NRCan | Todd McDonald | Senior Programmer |
| TBS | Guillaume Charest | Advisor, Open Source Software |
| ESDC | Terry Doerksen  | Programmer Analyst |
| ESDC | Calvin Rodo | Senior Advisor - Application Development
| DFO | Diana McHugh | Stock Assessment Biologist |
| ESDC | Josée Paquette | Programmer Analyst |
| ESDC | Gabriel Cossette | Senior Advisor |
| ESDC | Martin Mondor | Director of Strategy, Architecture and Business Relationships |
| ESDC | Michael Murphy | Director of Project Portfolio Management |
