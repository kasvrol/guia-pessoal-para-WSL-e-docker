# Comandos WSL

Atualizar Linux:
```sudo apt update && upgrade```

Confirmar se a distribuição Linux está instalada a versão:
```cat /etc/os-release```

Instalar app no Linux:
```sudo apt install <app>```

Abrir o WSL no powershell:
```wsl ~```

Sair da WSL no powershell:
```exit```

Abrir o explorador de arquivo (interface gráfica):
```explorer.exe .```

Listar mais detalhes sobre o conteúdo do diretório (tamanho, proprietário e data da última modificação)
```ls -l```

Listar TODOS os conteúdos de um diretório
```ls -a```

Remove arquivo
```rm```

Remove diretório
```rm -r```

Criar arquivo vazio
```touch```

Criar arquivo de texto o preenchendo no console (ctrl+d salva o arequivo)
```cat > file.txt```

Para verificar se o diretório encontra-se no Linux ou no Windows, verificar o caminho
```\\wsl.localhost\Ubuntu...``` - Linux - ```\mnt\c\Users\``` - Windows.

## Configurando a WSL

Instalar node ```sudo apt install nodejs```

Verificar versão ```node -v```

Instalar npm ```sudo apt install npm```

Instalar curl ```sudo apt install curl```

Instalar NVM 
```bash
curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash
source ~/.bashrc
```

Atualizar node
```bash
nvm install <version>
nvm install --lts
nvm use <version>
```

Instalar ferramentas
```bash
npm install -g @nestjs/cli
npm install --global yarn
```
