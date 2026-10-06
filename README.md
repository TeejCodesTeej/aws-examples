# aws-examples

Login with aws-cli using:

```
aws login
```

!!!
Make sure you do NOT login with your root-user.
!!!

Best practice is to create a root user and another user with whatever policies you need so that both are seperate.
You can use a machine user as well but I created a user with admin access and logged in with that.

## Checking that login works

```
aws sts get-caller-identity
```

Should return something like:
```
{
    "UserId": "A_USER_ID_GOES_HERE_WITH_NO_UNDERSCORES",
    "Account": "Account_id_goes_here",
    "Arn": "arn:aws:iam::userid:user/username"
}
```

Another way to check is to list s3 buckets.  If you do not have s3 buckets, you won't get anything back.

```
➜  aws-examples git:(main) ✗ aws s3 ls
2026-07-10 11:30:12 name-of-bucket
2026-04-22 10:34:37 name-of-another-bucket
```