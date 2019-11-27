# Dockerenv

`dockerenv` is a tool to create isolated environments using `Docker`.

`Docker` is great to run various projects without installing all their 
dependencies in your global envionments.
With `dockerenv` you can also retrieve all dev tools in your shell 
without installing them globally.
For a `typescript` project, it can be `yarn`, `jest`, `tslint`...
For a `PHP` project, it can be `composer`, `phpunit` ...

`dockerenv` will help you switch easily from a project to another.

This tool is widely inspired by [virtualenv](https://github.com/pypa/virtualenv) :heart:


## Usage

```bash
dockerenv
```

It will create a directory `.dockerenv.d` to place the new virtual environment.

If you want to rename this directory, you can use :

```bash
dockerenv mydirectory
```

### Activate script

Previous commands will also *activate* shell but on already created virtual
environment, you can run :

```bash
source .dockerenv.d/bin/activate
```

### Deactivate script

To undo these change :

```bash
deactivate
```

Or simply close your shell.

