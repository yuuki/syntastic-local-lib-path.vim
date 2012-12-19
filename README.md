# syntastic-local-lib-path

syntastic-local-lib-path is a plugin for [syntastic](https://github.com/scrooloose/syntastic).

It solves the problem that syntastic doesn't search modules installed to local directories by bundler, carton and npm and you must specify the absolute path of them.
It demands you just specifing relative path from project root directory to the local directories.

Currently, syntastic-local-lib-path doesn't support languages except for Perl because syntastic enables you specifing lib path only for Perl.

## Usage

```vim
g:syntastic_perl_local_lib_path = "vendor/lib"  " default is 'lib,extlib,local/lib/perl5'
autocmd FileType perl SyntasticLocalLibPath
```
