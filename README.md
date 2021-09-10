# Verdaccio-sample

Private NPM Server Sample

## Create User

```cli
htpasswd -c .htpasswd {user name}

New password: ''
Re-type new password: ''
```

## Add User

```cli
htpasswd .htpasswd {user name}

New password: ''
Re-type new password: ''
```

Add user in Server

```cli
npm adduser --registry {private npm URL}

Username: {user name}
Password: {password}
Email: (this IS public) {your email}
```

## Crate .npmrc file

```cli
echo registry={private npm URL} > .npmrc
```

## Publich Library to Prvate npm server

```cli
npm publish
```
