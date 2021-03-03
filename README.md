# IDEA settings repo

Settings themselves are on [master](https://github.com/temporalio/idea-settings/tree/master) branch which gets overwritten with every sync.

Full doc from JetBrains is here: https://www.jetbrains.com/help/idea/sharing-your-ide-settings.html#settings-repository.

1. Enable **Settings Repository** plugin.
2. Make sure you **don't** have `https://github.com/` override in your `.gitconfig` file:
    ```
    [url "ssh://git@github.com/"]
        insteadOf = https://github.com/
    ```
    (again, these lines should **NOT** be there).
3. Create personal token [here](https://github.com/settings/tokens) with only `public_repo` scope.
4. Add settings repository ("File/Manage IDE Settings/Settings Repository..."): https://github.com/temporalio/idea-settings.git and click "Overwrite Local".
5. Settings will be automatically synced with every IDE/project restart.
