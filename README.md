# posix-shutdown-shim: a quick hack for UNIX systems that lack a full `shutdown` command

# EXAMPLE

```console
$ shutdown
```

# ABOUT

posix-shutdown-shim is a minimal drop-in replacement for [shutdown](https://linux.die.net/man/8/shutdown), a program with several knobs for terminating a UNIX host. posix-shutdown-shim does not attempt to match the different semantics of any particular system's `shutdown` flags, but rather provides minimal syntactical compatibility, in order to help in porting shell scripts between different UNIX systems, where `shutdown` may not be present, but is called for by the scripts.

# INSTALL

```console
$ git clone https://github.com/mcandre/posix-shutdown-shim.git
$ cp posix-shutdown-shim/lib/shutdown /bin
```

# UNINSTALL

```console
$ rm /bin/shutdown
```
