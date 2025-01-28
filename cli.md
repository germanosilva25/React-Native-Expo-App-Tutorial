To check if a user is logged in to Expo via the CLI, you can use the following command:

```bash
expo whoami
```

This command will display the currently logged-in user's information. If no user is logged in, it will prompt that you are not logged in.

### If You Need to Log In
If no user is logged in, you can log in using:

```bash
expo login
```

To change the account logged into the Expo CLI, you can follow these steps:

1. **Log out of the current account**:
   Run the following command to log out of the current user:
   ```bash
   expo logout
   ```

2. **Log in with a different account**:
   After logging out, you can log in with a different account:
   ```bash
   expo login
   ```
