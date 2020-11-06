# Introduction

Here you will find some information about how the configuration file works, and in the next pages, how to completely setup everything.

First of all, the server owner or an administrator has to run the `tp//setup` command. If you are not an administrator and need to run this command, contact a developer in the [support server](https://discord.gg/aUNhdFD).

The next thing you need to know is how to fetch the YAML file that we will be working on. To do this, you have to run the [export](../commands/configuration/export.md) command.

{% hint style="info" %}
We recommend you to use a text editor such as Visual Studio Code or Notepad++ in order to open the file. However, you can use the one you like the most, even your PC's notepad.
{% endhint %}

This is what your file will look like the first time:

{% code title="YouServerID.yaml" %}
```yaml
levels:
  '459649180969730050': 100 # ThePhoDit#1801 - Your ID will be here. 

prefix: ';'
locale: 'en'
on_join_roles: []
local_blacklist: []
```
{% endcode %}

Those properties that you can see in the default configuration are necessary for the bot to work, so **DO NOT REMOVE THEM**.

We will be going through all different modules in the following pages.

