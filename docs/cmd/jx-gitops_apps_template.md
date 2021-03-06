## jx-gitops apps template

Generate the kubernetes resources from a jx-apps.yml

### Usage

```
jx-gitops apps template
```

### Synopsis

Generate the kubernetes resources from a jx-apps.yml

### Examples

  # generates the resources from a jx-apps.yml
  jx-gitops step jx-apps template

### Options

```
      --commit-message string         the git commit message used (default "chore: generated kubernetes resources from helm chart")
  -d, --dir string                    the directory that contains the jx-apps.yml (default ".")
      --domain string                 the default domain name in the generated ingress (default "cluster.local")
      --git-commit                    if set then the template command will git commit any changed files
  -h, --help                          help for template
      --include-crds                  if CRDs should be included in the output (default true)
      --namespace string              the default namespace if none is specified in the jx-apps.yml or jx-requirements.yml (default "jx")
      --no-external-secrets           if set then disable converting Secret resources to ExternalSecrets
      --no-split                      if set then disable splitting of multiple resources into separate files
      --optional                      check if there is a charts dir and if not do nothing if it does not exist
  -o, --output-dir string             the output directory to generate the templates to. Defaults to charts/$name/resources
  -c, --ref string                    the git ref (branch, tag, revision) to git clone (default "master")
      --template-values stringArray   provide extra values.yaml files passed into evaluating any values.yaml.gotmpl files such as for generating dummy secret values
  -n, --url string                    the git clone URL of the version stream
      --version-stream-dir string     optional directory that contains a version stream
```

### SEE ALSO

* [jx-gitops apps](jx-gitops_apps.md)	 - Commands for working with jx-apps.yml

###### Auto generated by spf13/cobra on 17-Jul-2020
