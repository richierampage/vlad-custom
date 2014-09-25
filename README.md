# Custom role for Vlad

## Adding to Vlad

This codebase needs to be located at the following path relative to [Vlad](https://bitbucket.org/philipnorton42/vlad):

```
../vlad-custom
```
See Vlad's docs on the [custom role](https://bitbucket.org/philipnorton42/vlad/src/1c2e2048c0e849ab431f747054fdade31bd302db/vlad/docs/custom_role.md?at=dev) for full details.

## Settings

### Option 1

Copy & rename ```vars/main.yml``` to ```../settings/vlad-custom-settings.yml``` and edit to suit.

### Option 2

Just edit vars/main.yml as required (note that this will get overwritten if you ```git pull``` in future).

## Drush site aliases

A local Drush alias will be automatically created for you. Further remote aliases can be added by placing a ```[whatever].aliases.drushrc.php``` file in ```../settings/drush_aliases/```. These will automatically be added to the VM.