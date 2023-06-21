1. Run the following command to configure `main` as the default branch name for new repositories instead of `master`.

   ```bash
   git config --global init.defaultBranch main
   ```

   > This change will occur for any new git repositories you initialize on your computer but will not affect existing repositories initialized before the command was run.


```sh
git config --global push.default current
git config --global --add --bool push.autoSetupRemote true
```
