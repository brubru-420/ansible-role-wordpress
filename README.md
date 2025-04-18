# Ansible Role: wordpress_role

Ce rôle Ansible installe et configure **WordPress** avec **Apache**, **PHP** et **MariaDB** sur des systèmes basés sur **Ubuntu/Debian** ou **Rocky Linux/RedHat**.

---

## 🧰 Fonctionnalités

- Installation automatique d'Apache ou httpd, PHP, MariaDB
- Téléchargement et déploiement de WordPress depuis wordpress.org
- Configuration automatique de la base de données WordPress
- Génération sécurisée de `wp-config.php`
- Activation du VirtualHost Apache + module `rewrite`
- Support multi-distributions (Debian/RedHat)

---

## 📦 Variables par défaut

```yaml
mysql_root_password: "examplerootPW"
wordpress_db_name: "wordpress"
wordpress_db_user: "example"
wordpress_db_password: "examplePW"
wordpress_web_root: "/var/www/html"
wordpress_url: "https://wordpress.org/latest.zip"

🖥️ Compatibilité
OS	Versions testées
Ubuntu	20.04+
Debian	10+
Rocky Linux	8+

📦 Installation via Ansible Galaxy

Une fois le rôle importé avec succès :

ansible-galaxy install brubru_420.wordpress_role

🧑‍💻 Auteur

    brubru-420

    GitHub : https://github.com/brubru-420