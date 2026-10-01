# Multi-Tier Architecture

## What is a Two-Tier Architecture?
A two-tier architecture separates an application into a web/application tier and a database tier. In this laboratory, Nextcloud is the web/application tier and MariaDB is the database tier.

## The Web/Application Tier
The web/application tier uses Nextcloud to provide the user interface and handle web requests from users.

## The Database Tier
The database tier uses MariaDB to store persistent application data, including user information and file metadata.

## Why Separate Them?
Separating the web application and database into different containers organizes their responsibilities. It also makes each service easier to manage, update, and troubleshoot independently.
