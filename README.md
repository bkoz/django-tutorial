# django-tutorial

## Openshift deployment

Deploy from the command line.

```
oc new-app https://github.com/bkoz/django-tutorial --env=APP_SCRIPT=runme.sh
oc expose svc django-tutorial
```
