# 👥 Creating and Managing Groups in Linux

Groups are used to assign permissions collectively to multiple users.

## 🔹 Creating a Group

```bash
sudo groupadd developers
```

> 📷 *Screenshot here*

## 🔹 Adding a User to a Group

```bash
sudo usermod -aG developers john
```

```bash
groups john
```

> 📷 *Screenshot of before and after*

## 🔹 Removing a User from a Group

```bash
gpasswd -d john developers
```

> 📷 *Screenshot here*
