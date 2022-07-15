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


## Redmine 플러그인 설치(공식)
https://www.redmine.org/projects/redmine/wiki/Plugins?utm_source=newsletter&utm_medium=email&utm_campaign=TRG_1801-gantt-01-installation-package-eng

## 이지간트는 여기
https://www.easyredmine.com/redmine-gantt-plugin

https://www.easyredmine.com/redmine-gantt-plugin#pux-modal-redmine-gantt-download


## 추가 플러그인
1. AJAX 플러그인: 상태 값 등을 edit 안하고 바꾸기
https://github.com/Ilogeek/redmine_issue_dynamic_edit

2. Agile 플러그인: 칸반 보드처럼 쓰기
https://www.redmineup.com/pages/plugins/agile

## 백업 방법
https://kmin135.blogspot.com/2017/08/bitnami-redmine.html

Redmine packaged by Bitnami 사용 으로 실행할 것

### DB Backup
```
mysqldump -ubitnami -p bitnami_redmine > RedmineDBBackup.dump
```

### DB 복원
```
mysql -ubitnami -p bitnami_redmine < RedmineDBBackup.dump
```
