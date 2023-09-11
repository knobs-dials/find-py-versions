# find-py-versions

Quick and dirty script to list all the python installations and virtual environments I can find.

Uses `locate` to not have to scan your filesystem every time, so 
* won't work on installs without it installed, e.g. containers, some slimmed down server setups
* you may want to `updatedb` if you want it to be up to date


Just trying to understand this mess ...though of course that potentially includes understanding all project managers think about this too :)

## Example output

```
# find-py-versions
    3.8.10    venv or virtualenv      '/data/coding/envtests/venv'
    3.8.10    venv or virtualenv      '/data/coding/envtests/virtualenv'
    3.8.10    venv or virtualenv      '/data/coding/LOOKAT/proj/.venv'
    3.8.10                 pyenv      '/root/.pyenv/versions/3.8.10'
    3.9.16                 pyenv      '/root/.pyenv/versions/3.9/envs/NAME'
    3.9.16                 pyenv      '/root/.pyenv/versions/3.9.16'
     3.9.2                 pyenv      '/root/.pyenv/versions/3.9.2'
     3.7.6                            '/root/miniconda3'
     3.7.6                            '/root/miniconda3/pkgs/python-3.7.6-h0371630_2'
     3.7.7                            '/root/miniconda3/pkgs/python-3.7.7-hcff3b4d_5'
     3.5.2                            '/snap/core/15511/usr'
     3.5.2                            '/snap/core/15511/usr'
     3.5.2                            '/snap/core/15925/usr'
     3.5.2                            '/snap/core/15925/usr'
    3.8.10                            '/snap/core20/1974/usr'
    3.8.10                            '/snap/core20/1974/usr'
    3.8.10                            '/snap/core20/2015/usr'
    3.8.10                            '/snap/core20/2015/usr'
         3                            '/snap/core22/858/usr'
      3.10                            '/snap/core22/858/usr'
         3                            '/snap/core22/864/usr'
      3.10                            '/snap/core22/864/usr'
       2.7                            '/usr'
    3.8.10                            '/usr'
    3.8.10                            '/usr'
     3.8.5                            '/var/lib/docker/overlay2/1718344e6b8af4081900854dc58b420627eb1c8c7dcd17dbb4ffa218f2778ba3/diff/usr'
     3.8.5                            '/var/lib/docker/overlay2/1718344e6b8af4081900854dc58b420627eb1c8c7dcd17dbb4ffa218f2778ba3/diff/usr'
       2.7                            '/var/lib/docker/overlay2/6fe9617297862cf624e5fe57d64980d28eb76c7a1edb00283e23edce6f413e5f/diff/usr'
     3.6.7                            '/var/lib/docker/overlay2/6fe9617297862cf624e5fe57d64980d28eb76c7a1edb00283e23edce6f413e5f/diff/usr'
     3.6.7                            '/var/lib/docker/overlay2/6fe9617297862cf624e5fe57d64980d28eb76c7a1edb00283e23edce6f413e5f/diff/usr'
       2.7                            '/var/lib/docker/overlay2/7a012ee7709ba569a1593bfa437bda6788b48f1d164ed6f0c5be66aa04bf10ea/merged/usr'
     3.6.7                            '/var/lib/docker/overlay2/7a012ee7709ba569a1593bfa437bda6788b48f1d164ed6f0c5be66aa04bf10ea/merged/usr'
     3.6.7                            '/var/lib/docker/overlay2/7a012ee7709ba569a1593bfa437bda6788b48f1d164ed6f0c5be66aa04bf10ea/merged/usr'
    3.8.10                            '/var/lib/docker/overlay2/a45cc113204a81d8895a74abc35a31a7b9c855873bfdeae9cad538683743d224/diff/usr'
```


