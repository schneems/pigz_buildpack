## PIGz Buildpack
[![Help Contribute to Open Source](https://www.codetriage.com/schneems/pigz_buildpack/badges/users.svg)](https://www.codetriage.com/schneems/pigz_buildpack)

Installs parallel gzip binary http://zlib.net/pigz/ into your heroku app

## Use

Set up multibuildpack https://github.com/ddollar/heroku-buildpack-multi.

add this buildpack to your `.buildpacks` file.

```
$ echo 'https://github.com/schneems/pigz_buildpack' >> .buildpacks
```

Then whatever buildpack you normally use (like heroku ruby)

```
$ echo 'https://github.com/heroku/heroku-buildpack-ruby' >> .buildpacks
```


Then deploy

## Verify

Use

```
$ heroku run bash
```

Then in the shell, run

```
$ pigz --help
```

## License

MIT