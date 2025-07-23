# About `template-component`

## Before using the template

### Enable GitHub Pages

Visit [Settings], [Pages] in the side menu at left, and choose [GitHub Actions]
as [Source] under [Build and deployment].

### Protect the default branch

1. Visit [Settings].
1. Click [Rules] in the side menu at left and click [Rulesets].
1. Click [New ruleset] button, and click [New branch ruleset].
1. [New branch ruleset] page is shown.
1. In [Ruleset Name], type "default"
1. Under [Enforcement status], select [Active]
1. Under [Target branches], click [Add target] button, and select [Include
   default branch].
1. Under [Branch rules], make sure the default rules, [Restrict deletions] and
   [Block force pushes], are checked.
1. Check [Require a pull request before merging]. Leave its options as-is.
1. Check [Require status checks to pass].


## Obtain an access token of ESP Component Registry

To automate uploading a component to ESP Component Registry with GitHub
Actions workflow, you need:

* to be an admin of the component
* to have a privilege to set Actions secrets and variables in the GitHub
  repository.

Contact @trombik if you don't or are not sure.

To use a workflow to upload the component when the component has been released,
you need an access token of ESP Component Registry. The token is used in a
workflow via GitHub secrets.


1. Visit [ESP Component Registry](https://components.espressif.com/) and
   login.
1. Click your profile menu on top and click [Tokens]
1. In [Create new access token] page, fill in [Description], e.g. "Uploading
   component from GitHub Action".

Next, create a GitHub secret in the repository.

1. Visit the component repository on GitHub.
1. Click [Settings]
1. Click [Secrets and variables] in the side menu at left.
1. Under [Repository secrets], click [New repository secret]
1. In [Actions secrets / New secret] page, fill in [Name] with `ESP_TOKEN`
1. Paste the access token value from the previous step into [Secret].
1. Click [Add secret].
