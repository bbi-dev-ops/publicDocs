# Development Time

We are using .NET Aspire. This framework speeds up, eases the pain points, and lowers the cost of development in a litany of ways:

* The application as it runs on local dev machines is nearly identical to what runs in the cloud

* The local dev experience is platform and IDE agnostic. It can be executed and debugged on MacOS, Windows, or Linux using any IDE or even a basic text editor. This massively improves the onboarding experience for new devs.

* Development Databases are containerized. This means that:
  * We do not have to incur costs for hosting development environment databases in Azure
  * Every dev can have their own copy of a database to use rather than everyone sharing the same one
  * Unique database versions can be shared amongst devs to sync up as needed
  * Testing, Migrations, and Seeding can occur in local containers which will run much faster than hosted

* The architecture is managed and simplified. It's largely already completed. This means more time spent on business logic and less resources spent on CI/CD