# npm.chelaike.com

## Usage

Alias NPM to use it:

```bash
alias cnpm="npm --registry=https://registry.npm.chelaike.com \
                --cache=$HOME/.npm/.cache/cnpm \
                --disturl=https://npm.taobao.org/mirrors/node \
                --userconfig=$HOME/.cnpmrc"
```

Or alias it in .bashrc or .zshrc

```
$ echo '\n#alias for cnpm\nalias cnpm="npm --registry=http://registry.npm.chelaike.com \
  --cache=$HOME/.npm/.cache/cnpm \
  --disturl=https://npm.taobao.org/mirrors/node \
  --userconfig=$HOME/.cnpmrc"' >> ~/.zshrc && source ~/.zshrc
```

### Install

```bash
$ cnpm install [name]
```

### Sync

Only `cnpm` cli has this command. Meaning sync package from source npm.

```bash
$ cnpm sync connect
```

sync package on web: [sync/connect](/sync/connect)

```bash
$ open http://registry.npm.chelaike.com/sync/connect
```

### publish / unpublish

Only `admin` user can publish / unpublish package to private registry.

```bash
$ cnpm publish [name]
$ cnpm unpublish [name]
```

### Other commands

Support all the other npm commands. e.g.:

```bash
$ cnpm info cnpm
```
