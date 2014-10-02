# Custom role for Vlad

## HEADS UP!

This project will soon be moving to GitHub. Details to be posted here when the move is complete. I'll sync both repos for a short time after the migration to help ease the move ;)

## Adding to Vlad

This codebase needs to be located at the following path relative to [Vlad](https://github.com/hashbangcode/vlad):

```
../vlad-custom
```
See Vlad's docs on the [custom role](https://github.com/hashbangcode/vlad/blob/dev/vlad/docs/custom_role.md) for full details.

## Settings

### Option 1 (best)

Copy & rename ```vars/main.yml``` to ```../settings/vlad-custom-settings.yml``` and edit to suit.

### Option 2

Just edit vars/main.yml as required (note that this will get overwritten if you ```git pull``` in future).

## Drush site aliases

A local Drush alias will be automatically created for you.

Further remote aliases can be added by placing a *single* ```[whatever].aliases.drushrc.php``` file in ```../settings```. These will automatically be added to the VM when provisioned.