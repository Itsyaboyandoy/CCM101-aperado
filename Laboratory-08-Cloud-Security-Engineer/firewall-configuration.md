# 🛡️ Firewall Configuration

## 🔐 1. Allow SSH

```bash
sudo ufw allow ssh
```

This command allows SSH connections so administrators can remotely access and manage the Ubuntu server.

## 🚫 2. Set the Default Firewall Rules

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

The first command blocks incoming connections unless they are specifically allowed. The second command allows outgoing connections by default.

## ⚙️ 3. Enable the Firewall

```bash
sudo ufw enable
```

This activates the UFW firewall and applies the configured security rules.

## 🌐 4. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This allows incoming TCP connections through port 8080, which is used to access the Nginx web application running inside the Docker container.

## 🔎 5. Check the Firewall Rules

```bash
sudo ufw status verbose
sudo ufw status numbered
```

These commands display the firewall status, default policies, and numbered rules. The results confirm that SSH and port 8080 are allowed while other incoming connections remain blocked by default.

## ⚠️ 6. Why SSH Must Be Allowed First

Allowing SSH before enabling UFW is important because activating the firewall without an SSH rule could block remote access. This may prevent administrators from managing the server remotely.
