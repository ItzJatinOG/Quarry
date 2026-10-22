# Minecraft Paper Plugin Troubleshooting

When a Minecraft plugin fails to load or behaves unexpectedly, the fastest path to a fix is usually to read the server logs carefully and confirm compatibility before changing configuration or code.

## Plugin failed to load

### Likely causes

- incompatible server version
- missing dependency
- invalid plugin descriptor
- Java runtime mismatch
- plugin conflict with another plugin
- a broken or partial JAR file

### How to investigate

- check the startup log for stack traces
- confirm the plugin is designed for the server software in use
- make sure the JAR file is complete and uncorrupted
- test the plugin on a development server before production

### Safe troubleshooting steps

- stop the server
- remove the plugin from the `plugins` folder or move it aside temporarily
- review the logs for the exact error message
- compare the plugin requirements with the actual server version and Java install

## Incorrect Java version

### Likely causes

- the server runs on a Java version not supported by the plugin
- the plugin was built with a newer Java target than the server is using
- the environment is running the wrong Java runtime

### How to investigate

- check the server startup logs
- verify the installed Java version against the server documentation
- confirm the plugin's compatibility notes

### Safe troubleshooting steps

- install or point the server to a compatible Java runtime
- test one change at a time
- restart the server only after confirming the version is correct

## Missing dependencies

### Likely causes

- the plugin depends on another library or plugin that is not installed
- a plugin update changed dependency requirements
- the dependency was removed or renamed

### How to investigate

- read the error output for missing class names or library names
- inspect the plugin documentation or release notes
- verify that all required dependency jars are present in the correct location

### Safe troubleshooting steps

- install the missing dependency with the same version expectations
- avoid mixing incompatible versions of the same library
- check whether another plugin is overriding the dependency unexpectedly

## Invalid plugin descriptor

### Likely causes

- a missing or malformed `plugin.yml` or `paper-plugin.yml`
- invalid name, version, or main class metadata
- a plugin built incorrectly or packaged without the required descriptor

### How to investigate

- read the startup log and look for descriptor errors
- inspect the plugin JAR contents for metadata files
- compare the metadata to the expected plugin pattern for the server software

### Safe troubleshooting steps

- rebuild the plugin or re-download from a trusted source
- ensure the main class path matches the descriptor exactly
- test on a minimal setup before production use

## Unsupported API version

### Likely causes

- wrong Paper or Bukkit API version
- plugin uses methods or classes not available in the current server version
- outdated plugin not maintained for the installed server build

### How to investigate

- confirm the server version and plugin version match
- review the plugin's compatibility notes
- inspect the stack trace for `NoSuchMethodError` or related API incompatibility errors

### Safe troubleshooting steps

- use a plugin version that matches the server implementation
- update the server and plugin together in a controlled environment
- avoid mixing incompatible API libraries in the same setup

## Permission problems

### Likely causes

- missing permission nodes in the permission plugin or configuration
- commands not registered with permissions as expected
- server uses a different permission system than the plugin documentation assumes

### How to investigate

- inspect the plugin's commands and permission documentation
- review the permission plugin configuration
- test command execution under an admin and a regular player account

### Safe troubleshooting steps

- configure permissions carefully
- test commands after deployment on a development server
- ensure players cannot trigger restricted commands by mistake

## Configuration errors

### Likely causes

- malformed YAML
- invalid values in settings
- missing required keys
- conflicting config options

### How to investigate

- read the startup log for config parsing errors
- check the generated config file format against plugin documentation
- inspect the server directory for the plugin's config files

### Safe troubleshooting steps

- back up configuration before editing
- correct the file one change at a time
- restart the server after each meaningful fix

## Runtime exceptions

### Likely causes

- null values or invalid player state
- event listeners triggering on unexpected conditions
- logic errors in commands or world interaction
- unsupported operations during server lifecycle transitions

### How to investigate

- read the full exception stack trace
- identify the exact plugin class involved
- reproduce the issue with minimal steps if possible

### Safe troubleshooting steps

- disable the plugin temporarily to confirm the behavior
- isolate the command or event that triggers the exception
- test in a staging server before adjusting a live environment

## Server startup errors

### Likely causes

- invalid plugin metadata or files
- plugin dependency issues
- conflicting or corrupted worlds or config state
- incompatible server version or runtime

### How to investigate

- examine the full startup log from the beginning of boot
- inspect the `plugins` directory for incomplete or stale files
- test with only one plugin enabled at a time when narrowing down a conflict

### Safe troubleshooting steps

- keep a recent backup of the server files
- remove problematic plugins one at a time
- restart only after confirming the root cause has been addressed

## General guidance

- always read the startup logs before changing anything else
- make one hypothesis at a time
- back up the server before modifying plugins or config
- prefer a staging server for production experiments
- treat generated code as untrusted until it has been reviewed and tested

## Related resources

- [paper-plugin-guide.md](paper-plugin-guide.md)
- [plugin-installation.md](plugin-installation.md)
- [minecraft-plugin-ideas.md](minecraft-plugin-ideas.md)
- [QuarryAI website](https://quarryai.dpdns.org/)
