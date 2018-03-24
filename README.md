# Twig Namespaces Plugin

This plugin adds Twig Namespacing capabilities to [Grav CMS](http://github.com/getgrav/grav). This means that you can write things like `{% include "@atoms/button" %}` and Grav will know where to look.

## Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `twig-namespaces`. You can find these files on [GitHub](https://github.com/phase2/grav-plugin-twig-namespaces).

You should now have all the plugin files under

    /your/site/grav/user/plugins/twig-namespaces
	
> NOTE: This plugin is a modular component for Grav which requires [Grav](http://github.com/getgrav/grav) and the [Error](https://github.com/getgrav/grav-plugin-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) to operate.

## Configuration

Before configuring this plugin, you should copy the `user/plugins/twig-namespaces/twig-namespaces.yaml` to `user/config/plugins/twig-namespaces.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```yaml
enabled: true
namespaces:  // Array of namespaces
  test:  // Namespace to be used in twig files as `@test`.
    paths:  // Array of paths 
      - path to folder containing twig files to be included in namespace
      - another path be included for namespaces
```
