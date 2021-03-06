# coc-jira-complete
[coc.nvim](https://github.com/neoclide/coc.nvim) extension for autocompleting issue keys from JIRA.  
Fetches unresolved issues assigned to your user.  
Useful in commit messages if using the [JIRA/GitHub plugin](https://github.com/marketplace/jira-software-github).

<img width="536" alt="demo" src="https://user-images.githubusercontent.com/6368728/64489737-d1c6d500-d256-11e9-8819-3a75c5ee8046.png">

## Getting Started
### Installing
#### Using [vim-plug](https://github.com/junegunn/vim-plug)
```vim
Plug 'jberglinds/coc-jira-complete', {'do': 'yarn install --frozen-lockfile'}
```
#### Using coc.nvim
Run `:CocInstall coc-jira-complete`

### Configuring
1. Generate an API key for your JIRA user at https://id.atlassian.com/manage/api-tokens
2. Run `:CocConfig` and add the following keys:

    ```json
    "jira.workspaceUrl": "<URL for your JIRA workspace, w/o trailing slash>",
    "jira.user.email": "<Your JIRA account email>",
    "jira.user.apiKey": "<Your JIRA account API key>"
    ```
3. Run `:CocRestart` to reload extension with new config

## Credits
Inspired by [mnpk/vim-jira-complete](https://github.com/mnpk/vim-jira-complete)
