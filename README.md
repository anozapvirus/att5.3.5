# Adicionar o diretório como seguro
git config --global --add safe.directory C:/vipclub_5.3.5

# Verificar os diretórios seguros
git config --global --get-all safe.directory

# Inicializar o repositório (se ainda não o fez)
git init

# Adicionar todos os arquivos ao stage
git add .

# Fazer um commit
git commit -m "Inicializando repositório com os arquivos do projeto"

# Adicionar o remote origin (se necessário)
git remote add origin https://github.com/anozapvirus/att5.3.5.git

# Enviar para o GitHub
git push -u origin master
# ou, se estiver usando main
git push -u origin main

# (Opcional) Configurar o Git Credential Manager
git config --global credential.helper manager-core
