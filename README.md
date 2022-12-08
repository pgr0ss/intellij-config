# intellij-config

Config files for [IntelliJ IDEA](https://www.jetbrains.com/idea/) version 2022.3.

## Notable Changes

Notable changes compared to the default settings on a fresh installation:

- Adds Vim plugin
- Adds [GitLink](https://plugins.jetbrains.com/plugin/8183-gitlink) plugin for easily opening files in GitHub/GitLab
- Turns on annotation processing (e.g. for Immutables, Lombok)

And a handful of other smaller changes, such as:
- Add unambiguous imports on the fly
- Open projects in new windows
- Turn off tooltips

## Installation

Close IntelliJ IDEA and symlink the files to the proper places with:

```
./setup_symlinks
```

You may also need to configure the project JDK since the path may be different. `File -> Project Structure` and set `Project SDK`.

## Project Level Settings

IntelliJ also has many project level settings that cannot be set globally. These need to be configured each time per project, and will reset if the `.idea` directory is deleted:
- Preferences -> Tools -> Actions on Save
  - Reformat Code
  - Optimize Imports
- Preferences -> Build, Execution, Deployment -> Build Tools
  - Reload project after changes in the build scripts: Any changes
- Preferences -> Version Control -> Commit
  - Clear initial commit message
  - Limit body line
