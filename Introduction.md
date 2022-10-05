# What is Gitea?
* Gitea is a painless self-hosted Git service. It is similar to GitHub, Bitbucket, and GitLab. Gitea is a fork of Gogs. See the Gitea Announcement blog post to read about the justification for a fork.  
* The goal of this project is to provide the easiest, fastest, and most painless way of setting up a self-hosted Git service. With Go, this can be done platform-independently across all platforms which Go supports, including Linux, macOS, and Windows, on x86, amd64, ARM and PowerPC architectures. You can try it out using the online demo.

## Feature
* User Dashboard
    * Context switcher (organization or current user)
    * Activity timeline
        * Commits
        * Issues
        * Pull requests
        * Repository creation
    * Searchable repository list
    * List of organizations
    * A list of mirror repositories
* Issues dashboard
    * Context switcher (organization or current user)
    * Filter by
        * Open
        * Closed
        * Your repositories
        * Assigned issues
        * Your issues
        * Repository
    * Sort by
        * Oldest
        * Last updated
        * Number of comments
* Pull request dashboard
    * Same as issue dashboard
* Repository types
    * Mirror
    * Normal
    * Migrated
* Notifications (email and web)
    * Read
    * Unread
    * Pin
* Explore page
    * Users
    * Repos
    * Organizations
    * Search
* Custom templates
* Override public files (logo, css, etc)
* CSRF and XSS protection
* HTTPS support
* Set allowed upload sizes and types
* Logging
* Configuration
    * Databases
        * MySQL (>=5.7)
        * PostgreSQL (>=10)
        * SQLite3
        * MSSQL (>=2008R2 SP3)
        * TiDB (MySQL protocol)
    * Configuration file
        * app.ini
    * Admin panel
        * Statistics
        * Actions
            * Delete inactive accounts
            * Delete cached repository archives
            * Delete repositories records which are missing their files
            * Run garbage collection on repositories
            * Rewrite SSH keys
            * Resync hooks
            * Recreate repositories which are missing
        * Server status
        * User management
        * Organization management
        * Repository management
        * Authentication sources
        * Configuration viewer
        * System notices
        * Monitoring
    * Environment variables
    * Command line options
* Multi-language support (21 languages)
* Mermaid diagrams in Markdown
* Math syntax in Markdown
* Mail service
* Reverse proxy support
* Users
    * Profile
    * Settings
* Repositories
    * Clone with SSH/HTTP/HTTPS
    * Git LFS
* Watch, Star, Fork
* View watchers, stars, and forks
* Code
    * Issues
    * Pull requests
    * Commits
    * Releases
    * Wiki
    * Settings
* Package Registries
    * Composer
    * Conan
    * Container
    * Generic
    * Helm
    * Maven
    * NPM
    * Nuget
    * PyPI
    * RubyGems

## Context
Gitea is sponsored by INBlockchain, Equinix Metal, Two Sigma, SoEBeS, Allspice, Towhee, Hostea, and all of the backers on Open Collective.  
This project has been forked from Gogs since November of 2016, but a lot has changed.



## Quality Attributes

### Cross-platform

Gitea runs anywhere Go can compile for. It can run on multiple operating systems: Windows, macOS, Linux, etc. And also multiple CPU architectures: x86_64, i386, arm64, arm, risc-v, etc. Choose the one you love!

### Easy to install

As simple as run the binary for your platform. This also make other options easy, for example ship it with Docker, or get it packaged.

### Lightweight

Gitea has low minimal requirements and can run on an inexpensive Raspberry Pi. Save your machine energy!

### Open Source

Go get code.gitea.io/gitea! Join us by contributing to make this project even better. Don’t be shy to be a contributor!

### Interoperability

Gitea provides webhooks to notify an external system of any changes in repositories.
Also, it provides OAuth/OAuth2 to login, making it easy to integrate with 3rd-party authenticate systems.

### Security

Gitea comes with CSRF and XSS protection and HTTPS support. This improves the security of the deployed instance.

### Multi-database support

Gitea is designed to support multiple databases, including MySQL, PostgreSQL, SQLite3, MSSQL, and TiDB. Allowing user to choose from their favourites.


## Key Drivers

### Quality Attributes
* Low resource consuming
* More platforms supported
* Safe with 2FA support

### Functional Requirements
* More 3rd-party integrations
* More functions in issue tracker

## Early Design Decision 
Gitea shall consume a little resource.  
Gitea shall support multiple platforms.  
Gtiea shall provide an easy and fast self-hosted Git service.  
Gitea should be able to integrate OAuth2.  
Gitea shall provide user with an web editor interface.  
Gitea should be similar to existing Git hosting solutions hence users could migrate painlessly.
