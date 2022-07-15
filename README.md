# Redmine20220714

## Redmine Link

https://downloads.bitnami.com/files/stacks/redmine/4.2.4-0/bitnami-redmine-4.2.4-0-windows-x64-installer.exe

## Redmine Plugin 설치

### Gem Install
```
bundle install --without development test
```


### DB Migration
```
bundle exec rake redmine:plugins:migrate RAILS_ENV=production
```


## DMSF Migraton
```
bundle exec rake db:migrate RAILS_ENV=production
```

```
bundle exec rake redmine:plugins:migrate NAME=redmine_dmsf RAILS_ENV=production
```
