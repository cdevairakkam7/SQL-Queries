### Granting Reader, Owner, and Writer access to users.

```{sql}
GRANT READER ON TABLE GIT_TEST To 'xyz@github.com'
GRANT OWNER  ON TABLE GIT_TEST To  'rst&yahoo.com'
GRANT WRITER  ON TABLE GIT_TEST To  'rst&yahoo.com'
```

### Revoking ALL, SELECT & UPDATE access from users.

```{sql}

REVOKE ALL ON GIT_TETST FROM 'rst@gmail.com'
REVOKE SELECT,UPDATE ON GIT_TETST FROM 'rst@gmail.com'
```
