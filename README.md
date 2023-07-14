# Information 
This is a patched version of PlaceholderAPI made specifically for [Papyrus](https://github.com/StumpStudio/Papyrus)

Currently, it replaces all setPlaceholder calls to Papyrus's multi-source parser and prefixes all placeholder identifiers with "papi"
e.g. instead of %player_name% you would write %papi_player_name%.

# Contribution
To contribute you need to:
1. Clone project with
    ```shell
    git clone https://github.com/StumpStudio/PlaceholderAPI-Papyrus.git
    ```
2. Apply all the patches in patches folder
3. Make patches of your work and save in patches folder
4. Submit a pull request 

# Why
The authors did not merge a [PR](https://github.com/PlaceholderAPI/PlaceholderAPI/pull/958) that would allow compatibility between plugins.
The JVM also does not allow to modify ```private static final ``` constants via reflection.
The rigidity of Bukkit did not allow for bridge plugin that would modify necessary classes.
The only simple solution for now is to use patched version.

## Quick Links
[PlaceholderAPI](https://github.com/PlaceholderAPI/PlaceholderAPI)