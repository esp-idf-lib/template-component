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
