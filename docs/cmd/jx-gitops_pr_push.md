## jx-gitops pr push

Pushes the current git directory to the branch used to create the Pull Request

### Usage

```
jx-gitops pr push
```

### Synopsis

Pushes the current git directory to the branch used to create the Pull Request

### Examples

  # pushes the current directories git contents to the branch used to create the current PR via $BRANCH_NAME
  jx-gitops pr push

### Options

```
  -b, -- branch string       the git branch to push to. If not specified we will find the branch from the PullRequest.Source property
      -- git-kind string     the kind of git server to connect to
      -- git-server string   the git server URL to create the git provider client. If not specified its defaulted from the current source URL
      -- git-token string    the git oauth token used to query the Pull Request to discover the branch name
  -d, --dir string           the directory to run the git push command from
  -h, --help                 help for push
  -r, --repo string          the full git repository name of the form 'owner/name' for the Pull Request
  -s, --source string        the git source URL of the current git clone
```

### SEE ALSO

* [jx-gitops pr](jx-gitops_pr.md)	 - Commands for working with Pull Requests

###### Auto generated by spf13/cobra on 17-Jul-2020
