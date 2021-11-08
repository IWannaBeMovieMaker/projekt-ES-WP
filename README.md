# ElasticSearch - Wordpress Integrace
## Docker
* vysvetleni fungovani
* zaindexovani polozek
* pridani pameti

## Odkazy:
* https://docs.docker.com/samples/wordpress/
* https://codeforgeek.com/integrate-wordpress-elasticsearch/
* https://github.com/10up/wp-local-docker-v2

## Odkazy intalaci:
* https://docs.docker.com/desktop/windows/install/
* https://nodejs.org/en/
* https://www.python.org/downloads/windows/

## Příkazy
### instalace WSL 2 (Windows subsystem pro Linux)
* wsl --install
1. Povolení WSL 
* dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
2. Povoleni Virtual Machine feature
* dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
3. stáhněte Linux kernel update package
* https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi
4. Nastavte WSL 2 jako vaši defaultní verzi WSL
* wsl --set-default-version 2
5. Nainstalujte Ubuntu, například z Microsoft Storu
6. Ověření instalace
* wsl --list --verbose

### Docker Desktop
stáhnout

### WSL Windows Terminal
1. spuštění WSL ve Windows Terminálu
* wsl
2. dostaňte se do Domovského repozitáře vašeho Linuxu
* cd ~
3. vytvořte projektovou složku
* mkdir ~/wordpress

### Enviroment Variables
1. Vytvořte .env v kořenové složce projektu
* nano ~/wordpress/.env
Vložte zde: 
MYSQL_ROOT_PASSWORD=your_root_password
MYSQL_USER=your_wordpress_database_user
MYSQL_PASSWORD=your_wordpress_database_password

