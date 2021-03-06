---
date: 2019-04-15T10:04:09Z
title: "jx get stream"
slug: jx_get_stream
url: /commands/jx_get_stream/
---
## jx get stream

Displays the version of a chart, package or docker image from the Version Stream

### Synopsis

Displays the version of a chart, package or docker image from the Version Stream 

For more information see: https://jenkins-x.io/architecture/version-stream/

```
jx get stream [flags]
```

### Examples

```
  # List the version of a docker image
  jx get stream -k docker gcr.io/jenkinsxio/builder-jx
  
  # List the version of a chart
  jx get stream -k charts jenkins-x/tekton
```

### Options

```
      --dir string    the directory containing a git clone of the jenkins-x/jenkins-x-versions git repository. Leave blank and a new clone will be made
  -h, --help          help for stream
  -k, --kind string   The kind of version. Possible values: charts, packages, docker (default "docker")
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --install-dependencies      Enables automatic dependencies installation when required
      --log-level string          Sets the logging level (panic, fatal, error, warning, info, debug) (default "info")
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx get](/commands/jx_get/)	 - Display one or more resources

###### Auto generated by spf13/cobra on 15-Apr-2019
