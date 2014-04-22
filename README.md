# Custom playbooks for Vlad

## Adding to Vlad

This codebase needs to located at the following path within [Vlad](https://bitbucket.org/philipnorton42/vlad):

```
vlad/playbooks-custom/custom
```
Note the ```custom``` directory at the end of that path; you'll need to create this as it's not already present in Vlad.

## Including playbooks

Copy & rename ```example.main.yml``` to ```main.yml``` in the ```tasks``` directory. Customise ```main.yml``` to include playbooks for use.

```main.yml``` is kept out of version control to ensure that any customisations are not overwritten on ```git pull```. While ```main.yml``` could be further abstracted to get around this, the current solution ensures that it's still possible to include playbooks in *any order*.

## The distinction between 'common & 'project'

Files are often divided into 'common' and 'project':

* **common**: files that could be used in any project
* **project**: files that are or could be specific to a project

Generally, 'common' files are included in this repo and 'project' files are not in order to prevent overwriting on ```git pull```. Examples of 'project' files are included (see below).

## Example files

Example files have been included where you would normally want to use project specific code. These can be copied to where they would normally reside and modified to suit.

Some 'common' tasks will attempt to use 'project' templates - these will require that the template file is in place (again, these have been included as example files).