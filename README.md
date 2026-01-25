# GitHub Sandbox
This is an API sandbox for the [GitHub API](https://developers.github.com/), using an OpenAPI specification with examples, Microcks and Bruno as the sandbox interface, and this GitHub repository as the vehicle for delivering a localized sandbox.

## Capability-Driven
This sandbox is capability-driven, using an early [prototype of the Naftiko capability schema as the manifest](capability-github-sandbox.yml). The manifest provides the mapping to the OpenAPI source for the sandbox and guides the evolution of the sandbox, aligning with business outcomes—something we will keep iterating upon.

## OpenAPI
This sandbox uses OpenAPI as the definition, providing [a complete definition of all available paths for the GitHub API](openapi/github-openapi.yml). This OpenAPI uses examples and Microcks extensions to mock the requests and responses for each API operation, something we will iterate and expand upon with richer examples as we move forward.

## Microcks
This sandbox uses Microcks to deliver the mock API. [You just install Microcks, with the Docker extension being the easiest](https://microcks.io/documentation/guides/installation/docker-desktop-extension/), import any of the OpenAPIs and you have a mocked API for the entire GitHub API, available via REST and MCP APIs--providing a multi-protocol sandbox.

## Bruno
This sandbox [uses Bruno as the client](https://www.usebruno.com/), leveraging Bruno Collections pre-generated from the OpenAPI and a Bruno environment that uses the localhost and port of Microcks to work with the mocked API. You just have to install Microcks, then open the collection provided in this repository, select the available environment, and begin calling the GitHub API via the sandbox.

# GitHub Organizations API

## Summary
This is a summary of this sandbox, breaking down the available paths, operations, and other relevant detail regarding the scope of this sandbox, designed to support development and testing against the GitHub API.

numberOfPaths: 104
numberOfOperations: 179
numberOfReadOperations: 85
numberOfWriteOperations: 94
numberOfSchemas: 127
numberOfResponses: 15
numberOfParameters: 60
numberOfExamples: 82
numberOfRequestBodies: 0
numberOfHeaders: 1

## Resources
These are the resources available via the GitHub API, which are made available via this sandbox API, which are applied as tags to each operation in the OpenAPI.

Access, Actions, Actions Cache, Actions Oidc, Actions Permissions, Actions Runners, Actions Secrets, Actions Variables, Active, Advanced, Alerts, All, Allowed, Announcement, Announcement Banners, Applications, Archive, Assigned, Audit, Audit Log, Authenticated, Banner, Between, Billing, Cache, Check, Child, Child Teams, Claims, Code, Code Scanning Alerts, Collaborators, Comments, Committers, Configuration, Conflicting, Connection, Convert, Custom, Custom Repository Roles, Customizations, Default, Deliveries, Dependabot, Dependabot Alerts, Dependabot Secrets, Disablement, Discussion Comments, Discussions, Docker, Docker Migration, Download, During, Enabled, Enablement, Enforcement, Events, External, External Groups, Feature, Fine-grained, Groups, Hook, Hooks, Installations, Issues, Keys, Labels, Log, Manager, Member, Members, Membership, Memberships, Migrations, Name, Openid Connect, Organization Events, Organization Installations, Organization Issues, Organization Members, Organization Migrations, Organization Projects, Organization Repositories, Organization Webhooks, Organizations, Outside, Outside Collaborators, Owned, Package, Package Versions, Packages, Permissions, Ping, Pre-receive, Pre-receive Hooks, Project, Projects, Public, Re-deliver, Reactions, Registration, Removal, Repositories, Repository Permissions, Restore, Role, Roles, Runner Groups, Runners, Scanning, Secret Scanning Alerts, Secrets, Security Features, Security Managers, Selected, Self-hosted, Start, Status, Subject, Team Discussions, Team Members, Team Projects, Team Repositories, Teams, Templates, Tokens, Unlock, Update, Usage, Users, Variables, Versions, Webhooks, Workflows

# GitHub Projects API

## Summary
This is a summary of this sandbox, breaking down the available paths, operations, and other relevant detail regarding the scope of this sandbox, designed to support development and testing against the GitHub API.

numberOfPaths: 10
numberOfOperations: 19
numberOfReadOperations: 7
numberOfWriteOperations: 12
numberOfSchemas: 9
numberOfResponses: 7
numberOfParameters: 6
numberOfExamples: 6
numberOfRequestBodies: 0
numberOfHeaders: 1

## Resources
These are the resources available via the GitHub API, which are made available via this sandbox API, which are applied as tags to each operation in the OpenAPI.

  - Cards
  - Collaborators
  - Columns
  - Permissions
  - Projects
  - Repositories
  - Users

# GitHub Repos API

## Summary
This is a summary of this sandbox, breaking down the available paths, operations, and other relevant detail regarding the scope of this sandbox, designed to support development and testing against the GitHub API.

numberOfPaths: 111
numberOfOperations: 160
numberOfReadOperations: 88
numberOfWriteOperations: 72
numberOfSchemas: 127
numberOfResponses: 15
numberOfParameters: 38
numberOfExamples: 97
numberOfRequestBodies: 0
numberOfHeaders: 1

## Resources
These are the resources available via the GitHub API, which are made available via this sandbox API, which are applied as tags to each operation in the OpenAPI.

App Installations, Archives, Assignees, Branch Policies, Check Runs, Check Suites, Codeowners, Commit Comments, Commit Statuses, Commits, Contents, Contributors, Dependency Graph, Deploy Keys, Deployment Statuses, Deployments, Environment Secrets, Environment Variables, Environments, Events, Forks, Git Blobs, Git Lfs, Git Refs, Git Tags, Git Trees, Labels, Languages, Licenses, Merges, Milestones, Notifications, Pages, Pages Builds, Reactions, Readme, Release Assets, Releases, Replicas, Repositories, Repository Events, Search, Secret Scanning, Stargazers, Statistics, Teams, Templates, Topics, Transfers, Vulnerability Alerts, Watchers

# GitHub Search API

## Summary
This is a summary of this sandbox, breaking down the available paths, operations, and other relevant detail regarding the scope of this sandbox, designed to support development and testing against the GitHub API.

numberOfPaths: 7
numberOfOperations: 7
numberOfReadOperations: 7
numberOfWriteOperations: 0
numberOfSchemas: 23
numberOfResponses: 5
numberOfParameters: 3
numberOfExamples: 7
numberOfRequestBodies: 0
numberOfHeaders: 0

## Resources
These are the resources available via the GitHub API, which are made available via this sandbox API, which are applied as tags to each operation in the OpenAPI.

Code, Commits, Issues, Labels, Repositories, Topics, Users

# GitHub Users API

## Summary
This is a summary of this sandbox, breaking down the available paths, operations, and other relevant detail regarding the scope of this sandbox, designed to support development and testing against the GitHub API.

numberOfPaths: 77
numberOfOperations: 108
numberOfReadOperations: 63
numberOfWriteOperations: 45
numberOfSchemas: 53
numberOfResponses: 10
numberOfParameters: 26
numberOfExamples: 51
numberOfRequestBodies: 0
numberOfHeaders: 1

## Resources
These are the resources available via the GitHub API, which are made available via this sandbox API, which are applied as tags to each operation in the OpenAPI.

Accessrestriction, Authorization, Branchprotection, Email, Enterpriseadmin, Event, Follower, Gist, Gpgkey, Hovercard, Installation, Issue, Ldapmapping, Organization, Organizationmembership, Package, Repository, Search, Siteadmin, Socialaccount, Sshkey, Sshsigningkey, Starredrepository, Statistics, Subscription, User, Usersuspension

## Backstage
We provide a Backstage software catalog entity for the GitHub API Sandbox, allowing this sandbox to be registered with any catalog, making it discoverable by team and across an organization--allowing anyone to fork and deploy locally within the enterprise.

## Support
Please provide any questions or feedback via GitHub issues, or just email kinlane@naftiko.io with feedback. The goal is to keep iterating upon this sandbox using existing OpenAPI, Microcks, and Bruno features, offering value out of the box via this forkable third-party GitHub API sandbox.


