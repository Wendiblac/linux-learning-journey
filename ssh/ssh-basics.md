# 🔐 SSH Basics in Linux

## 🔹 Generating SSH Keys

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

> 📷 *Screenshot here*

## 🔹 Copying the Public Key to a Server

```bash
ssh-copy-id username@remote_host
```

> 📷 *Screenshot here*

## 🔹 Connecting to a Remote Server

```bash
ssh username@remote_host
```

> 📷 *Screenshot here*

## 🔹 SSH Config File Setup (Optional)

```bash
nano ~/.ssh/config
```

```
Host myserver
    HostName 192.168.1.10
    User john
    IdentityFile ~/.ssh/id_rsa
```

```bash
ssh myserver
```

> 📷 *Screenshot here*
