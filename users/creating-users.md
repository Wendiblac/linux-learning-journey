# 👤 Creating Users in Linux

Learning to create and manage users is fundamental for any Linux administrator.

## 🔹 `adduser` Command

```bash
sudo adduser doe
```

🔸 This command creates a new user `doe`, creates a home directory `/home/doe`, and sets up necessary configurations.
`Features`
The features of this command includes;
-High-level wrapper around `useradd`.
-Prompts you to interactively to set:
    -Full Name
    -Password
    -Room Number
    -Work Phone
    -Home Phone
    -Other user info
-Automatically:
    -Creates the home directory
    -Sets default shell `(/bin/bash)`
    -Adds to some default groups (not sudo unless specified)

> 📷 *images\adduser.png*


## 🔹 `useradd` Command

```bash
sudo useradd -m -s /bin/bash linda
sudo passwd linda
```
🔸 This command creates a new user `linda`, creates a home directory `/home/linda`, and sets up necessary configurations.
`Features`
The features of this command includes;
-Creates a new user linda
-`-m` creates a home directory at /home/linda.
-`-s /bin/bash` sets the default shell to /bin/bash.
-Does not set a password or add the user to any groups.
-You must manually:
    -Set the password after creating the user; `sudo passwd linda` you'd then be prompted to set a new a password for the user.
    -Add to groups (eg., sudo); `sudo usermod -aG sudo linda`

> 📷 *images\useradd-linda.png*

## 🔹 Check Created Users

```bash
cat /etc/passwd | grep doe
cat /etc/passwd | grep linda
```

> 📷 *images\grepdoe.png*
> 📷 *images\greplinda.png*
