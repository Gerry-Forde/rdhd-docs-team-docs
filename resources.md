# Resources

This page contains useful links for the Red Hat Developer Hub Docs team.

---

## Installation Methods
### Local Installation
**RHDH Local** is the fastest and simplest way to test your software catalogs, techdocs, plugins, templates, homepage customizations, and configurations.

RHDH Local is ideal for trying out the basic features of RHDH (like Software Catalogs or TechDocs) without the need for a Kubernetes cluster. It is also great for testing dynamic plugins and their configuration settings. To use RHDH Local, all you really need is basic knowledge of Docker or Podman, a PC, and a web browser. You can run it on your laptop, desktop, or homelab.

#### Prerequisites

- You have installed **Podman** on your PC.
- You have installed **podman-compose**.

#### Procedure

1. Clone the [RHDH Local](https://github.com/redhat-developer/rhdh-local) repository to a location on your PC:
   ```bash
   cd rhdh-local
   cp env.sample .env

2. Set the `RHDH_IMAGE` environment variable in your `.env` file:
   ```bash
   RHDH_IMAGE=quay.io/rhdh-community/rhdh:next

3. Install podman-compose using Homebrew: 
    ```bash
    brew install podman-compose

4. Start the RHDH Local instance:
    ```bash
    podman-compose up -d

5. Open your web browser and navigate to:
    ```bash
    localhost:7007

## Useful links
### [Red Hat Developer Hub Helm Chart](https://github.com/redhat-developer/rhdh-chart)
### [Red Hat Developer Hub documentation](https://gitlab.cee.redhat.com/red-hat-developers-documentation/rhdh)
  
## Project information
Red Hat Developer Hub documentation. Synced from upstream at https://github.com/redhat-developer/red-hat-developers-documentation-rhdh (aka https://github.com/redhat-developer/rhdh-documentation-sync). NOTE: changes made directly to this repo's protected branches will be OVERWRITTEN by sync from upstream repo.
