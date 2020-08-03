# django-tutorial

## Openshift deployment

Select Add to Project -> from GIT -> Use python builder image

set APP_SCRIPT=runme.sh in deployment config

```
oc set env dc/django-tutorial-git APP_SCRIPT=runme.sh
```

Deploy from cmd line (not tested).

```
oc new-app https://github.com/bkoz/django-tutorial --env=APP_SCRIPT=runme.sh
```
