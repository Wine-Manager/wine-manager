# wine-manager

Um simples script Bash para ajudar a gerenciar prefixos Wine e facilitar a execução de aplicativos e jogos Windows no Linux.

## Instalação

Escolha o método de instalação que melhor se adapta ao seu sistema:

### 1\. No Arch Linux (AUR)

O `wine-manager` está disponível no [Arch User Repository (AUR)](https://www.google.com/search?q=https://aur.archlinux.org/packages/wine-manager).

**a) Usando um AUR helper (recomendado, ex: `yay`)**

Se você já tem o `yay` (ou outro AUR helper) instalado:

```bash
yay -S wine-manager
```

**b) Manualmente via `git` e `makepkg`**

Se você preferir instalar manualmente:

```bash
# Clone o repositório do AUR
git clone https://aur.archlinux.org/wine-manager.git

# Entre no diretório clonado
cd wine-manager

# Compile e instale o pacote
makepkg -si
```

### 2\. No Ubuntu (via PPA)

Você pode instalar o `wine-manager` através do meu PPA oficial no Launchpad.

```bash
# Adicione o PPA ao seu sistema
sudo add-apt-repository ppa:pedrolucas2025/wine-manager-ppa

# Atualize sua lista de pacotes
sudo apt update

# Instale o wine-manager
sudo apt install wine-manager
```

### 3\. No Debian (via pacote .deb)

Você pode baixar o pacote `.deb` diretamente do meu PPA no Launchpad e instalá-lo.

1.  Vá para a página do PPA: [https://launchpad.net/\~pedrolucas2025/+archive/ubuntu/wine-manager-ppa](https://launchpad.net/~pedrolucas2025/+archive/ubuntu/wine-manager-ppa)

2.  Clique no pacote `wine-manager`.

3.  Na seção "Downloadable files", encontre o arquivo `.deb` para sua arquitetura (ex: `amd64`) e sua versão do Debian/Ubuntu (ex: `noble` para Ubuntu 24.04, que é compatível com Debian Testing/Sid ou versões futuras estáveis).

4.  Baixe o arquivo `.deb`.

5.  Instale o pacote:

    ```bash
    # Exemplo: se o arquivo for wine-manager_1.0.0-8_all.deb
    sudo dpkg -i wine-manager_1.0.0-8_all.deb
    sudo apt --fix-broken install # Para resolver dependências ausentes, se houver
    ```

### 4\. Em Outros Sistemas Linux (Instalação Manual)

Para outras distribuições Linux, você pode baixar o script diretamente e colocá-lo no seu `$PATH`.

1.  Vá para o repositório do script wine-manager :
[https://github.com/pedrodev2025/wine-manager](https://github.com/pedrodev2025/wine-manager)
2.  Clique no arquivo `wine-manager`, depois no botão "Raw" (ou "Bruto") para ver o conteúdo puro do script.

3.  Copie a URL da página do "Raw" (ela deve terminar com `/wine-manager`).

4.  No seu terminal:

    ```bash
    # Baixe o script
    sudo wget -O /usr/local/bin/wine-manager "URL_DO_SCRIPT_RAW"

    # Dê permissão de execução
    sudo chmod +x /usr/local/bin/wine-manager
    ```

    *É recomendado usar `/usr/local/bin/` para scripts instalados manualmente, pois ele geralmente está no seu `$PATH` e não interfere com pacotes do sistema.*
