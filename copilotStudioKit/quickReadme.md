# Copilot Studio Kit Quick Readme

This guide summarizes how to get and set up Copilot Studio Kit.

## Getting the Kit

You can get Copilot Studio Kit in two ways:

- From AppSource
- From the GitHub repository

### Recommended approach: AppSource

Using AppSource is the recommended path.

## Installation

1. Go to the AppSource listing for Copilot Studio Kit.
2. Choose the environment where you want to install it.
3. Start the installation.
4. Expect the installation to take a few hours to complete.

> Important: The AppSource installation path is different from the GitHub repository installation path. Follow the AppSource instructions carefully.

## What you will see after installation

After installation completes, you will immediately be able to see the Prompt tools in the environment.

You will also see Power Automate flows in the environment, but they are not directly viewable from Copilot Studio because they are not Agent Flows. They appear as flows in the Copilot Studio plan and solution.

You will also see Power Apps apps. However, the flows and apps are not all immediately ready to use.

## Post-install setup you must do

After installing the kit, complete the required setup before trying to use everything.

### 1. Configure apps and connection references

The kit includes apps and connection references that need to be configured.

### 2. Enable flows in the correct order

The flows need to be enabled, and the recommended order is:

1. Flows that end with "Grandchild"
2. Flows that end with "Child"
3. The remaining flows, as needed

### 3. Review the included apps

There are three main types of apps in the kit:

- The flagship app
- An app for makers
- An app for admins

Once the apps, connection references, and flows are configured and enabled, you can truly enjoy the kit.

## Official instructions

Follow the official installation guidance here:

- Microsoft GitHub instructions: https://github.com/microsoft/Power-CAT-Copilot-Studio-Kit/blob/main/INSTALLATION_INSTRUCTIONS.md
- Related article: [Copilot Studio Kit: Beyond Test Automation | The Custom Engine](https://microsoft.github.io/mcscatblog/posts/copilot-studio-kit/)

Be sure to follow the AppSource installation instructions, not the GitHub import instructions.

## Updating the Kit

If you already have the kit installed and want to update it, read the update instructions in the official documentation as well.

## Summary

- Recommended install path: AppSource
- Choose the target environment during installation
- Installation may take a few hours
- Prompt tools appear right away
- Additional setup is required for apps, connection references, and flows
- Enable flows in the specified order
- Use the official installation and update guidance for the full experience
