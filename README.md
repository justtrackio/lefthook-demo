# lefthook-demo

```shell
cd subfolder
LEFTHOOK_VERBOSE=1 lefthook install
```

```shell

➜  subfolder git:(main) LEFTHOOK_VERBOSE=1 lefthook install                   
│ [lefthook] cmd:    [git rev-parse --show-toplevel]
│ [lefthook] stdout: /git-repos/github/justtrackio/lefthook-demo

│ [lefthook] cmd:    [git rev-parse --git-path hooks]
│ [lefthook] stdout: ../.git/hooks

│ [lefthook] cmd:    [git rev-parse --git-path info]
│ [lefthook] stdout: ../.git/info

│ [lefthook] cmd:    [git rev-parse --git-dir]
│ [lefthook] stdout: /git-repos/github/justtrackio/lefthook-demo/.git

│ [lefthook] cmd:    [git hash-object -t tree /dev/null]
│ [lefthook] stdout: 4b825dc642cb6eb9a060e54bf8d69288fbee4904

│ Searching config in:/git-repos/github/justtrackio/lefthook-demo
│ Merging remote config: git@github.com:evilmartians/lefthook: ../.git/info/lefthook-remotes/lefthook/examples/remote/ping.yml
│ Cloning remote config repository: ../.git/info/lefthook-remotes/lefthook
│ [lefthook] cmd:    [git -C ../.git/info/lefthook-remotes clone --quiet --origin origin --depth 1 git@github.com:evilmartians/lefthook lefthook]
│ [lefthook] dir:    /git-repos/github/justtrackio/lefthook-demo
│ [lefthook] error:  exit status 128
│ [lefthook] stdout: 
│ [lefthook] stderr: fatal: cannot change to '../.git/info/lefthook-remotes': No such file or directory

Couldn't sync from git@github.com:evilmartians/lefthook. Will continue anyway: exit status 128
```