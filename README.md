# dokku-email

A simple dokku plugin to send email notifications on successful deployment.

It relies on the "mail" command existing. Install it with `apt-get install mailutils`.

It's suggested you also install `postfix` as a satellite system that uses a 3rd party mail server for sending mail.

## Plugin installation

```sh
dokku plugin:install https://github.com/badsyntax/dokku-email.git
```

You can update the plugin with:

```sh
dokku plugin:update email
```

## Commands

Show help:

```sh
dokku email:help
```

Add an email:

```sh
dokku email:set email@example.com
```

Remove an email

```sh
dokku email:remove email@example.com
```

List emails:

```sh
dokku email:list
```
