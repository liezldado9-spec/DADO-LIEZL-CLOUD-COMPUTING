# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a software design pattern where an application is split into two distinct layers: a **presentation/application tier** and a **data tier**. Each tier runs independently and communicates over a network, allowing them to be developed, deployed, and scaled separately.

## The Web/Application Tier

The web/application tier is responsible for:
- Serving the user interface (HTML, CSS, JavaScript) to end users
- Handling HTTP/HTTPS requests from browsers
- Processing business logic and user authentication
- Communicating with the database tier to read/write data

In our deployment, **Nextcloud** runs in this tier. It receives browser requests on port 8080, renders the web interface, and queries the database for user credentials and file metadata.

## The Database Tier

The database tier is responsible for:
- Storing persistent data (user accounts, passwords, file metadata)
- Providing structured query access (SQL) to the application tier
- Ensuring data integrity, transactions, and backups

In our deployment, **MariaDB 10.6** runs in this tier. It listens on the internal Docker network and only accepts connections from the Nextcloud container.

## Why Separate Them?

Separating the web server and database into two containers provides **isolation, scalability, and resilience**. If the web container crashes or needs to be updated, the database remains intact and untouched, preventing data loss. Additionally, each tier can be scaled independently — you can run multiple Nextcloud containers behind a load balancer while keeping a single database, or upgrade the database engine without redeploying the web application. This separation also improves security because the database is never directly exposed to the public internet.
