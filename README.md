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

## OpenJDK 다운로드
홈페이지: https://github.com/ojdkbuild/ojdkbuild

다운로드 링크: https://github.com/ojdkbuild/ojdkbuild/releases/download/java-11-openjdk-11.0.15.9-1/java-11-openjdk-11.0.15.9-1.windows.ojdkbuild.x86_64.zip

## SCMManager
홈페이지: https://scm-manager.org/
다운로드 링크: https://scm-manager.org/download/#windows
