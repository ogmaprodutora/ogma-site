# OGMA Produtora — site

Site institucional da OGMA Produtora Audiovisual: https://ogmaprodutora.com

- `index.html` — página única (CSS, JS e imagens embutidos)
- `.htaccess` — configuração gerada pelo cPanel (HostGator)

## Publicar
HostGator → cPanel → Gerenciador de arquivos → `public_html` → Carregar `index.html`.

## Publicação automática
Todo push na branch `main` publica o site na HostGator via FTP (`.github/workflows/deploy.yml`).
Secrets necessários no GitHub: `FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD`.
A conta FTP deve ter como diretório a pasta `public_html`.
