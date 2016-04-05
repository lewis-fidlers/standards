# 10to1 Code styles

In this repo we'll add the code style configuration that is used by our CI by default.

The CI uses [pronto](https://github.com/mmozuras/pronto).

## The ruby styleguide

You can use the ruby styleguide as a base by adding it to your homedirectory

```
curl -Lo ~/.rubocop.yml https://raw.githubusercontent.com/10to1/styleguides/master/guides/ruby.yml
```

In our case this is installed for the CI-user. But can be overridden on a per project basis
