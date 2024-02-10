# Restricted Environment Customization

## Overview

This repo provides the solution for individuals working in environments where installing bash extensions or configuring zsh is restricted. In such cases, users can leverage this project to customize their working environment by making modifications to their `.profile` file and adding custom plugins maintained independently.

## Table of Contents

- [Introduction](#restricted-environment-customization)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Customization](#customization)
- [Adding Custom Plugins](#adding-custom-plugins)
- [Maintaining Custom Plugins](#maintaining-custom-plugins)

## Prerequisites

Before getting started, ensure that the following prerequisites are met:

- A working knowledge of the shell environment.
- Access to the `.profile` file on your workstation.

## Getting Started

1. Clone this repository to your local machine and place it where you want:

    ```bash
    git clone https://github.com/AleNegrini/bash-plugins.git
    ```

3. Add the following code snippets to your `.profile`:

    ```bash
    source ~/.bash-plugins/dir.aliases.sh
    source ~/.bash-plugins/ls.aliases.sh
    source ~/.bash-plugins/git.plugin.sh
    source ~/.bash-plugins/misc.aliases.sh
    ```

    Just add the plugin you'd like to use

4. Reload your shell to apply the changes:

    ```bash
    source ~/.profile
    ```

Edit the `.profile` file to tailor it to your specific requirements. You can add environment variables, aliases, and other custom configurations to enhance your shell experience within the constraints of your restricted environment.

## Adding Custom Plugins

To extend functionality, you can create and add custom plugins to the directory. Follow these steps:

1. Create a new file for your plugin:

    ```bash
    touch plugins/my_custom_plugin.sh
    ```

2. Add your custom functionality to `my_custom_plugin.sh`.

3. Update your `.profile` file to load the new plugin:

    ```bash
    # Add the following line to the .profile file
    source /path/to/restricted-environment-customization/plugins/my_custom_plugin.sh
    ```

4. Reload your shell:

    ```bash
    source ~/.profile
    ```

## Maintaining Custom Plugins

As you create and modify custom plugins, ensure to keep them organized within the `bash-plugin/` directory. Regularly update your `.profile` file to include or exclude specific plugins based on your needs.



