Puppet Cheatsheet
=================

Default **ModulePath** is in `$codedir/modules`

Validate a manifest:

    $ puppet parser validate mymanifest.pp

Apply a manifest:

    $ puppet apply mymanifest.pp

Inspect a resource:

    $ puppet resource [type] [title]
