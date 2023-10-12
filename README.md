# Foreman fapolicyd Rules

fapolicyd rules for Foreman.

## Testing

To test these rules manually:

```
dnf -y install fapolicyd
cp *.rules /etc/fapolicy.d/rules/
systemctl start fapolicyd
```

To debug the rules, start fapolicyd manually in debug mode:

```
fapolicyd --debug-deny 2> fapolicy.output
```
