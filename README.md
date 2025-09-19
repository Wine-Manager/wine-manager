# wine-manager 
Um simples script Bash para ajudar a gerenciar prefixos Wine e facilitar a execução de aplicativos e jogos Windows no Linux. 
## Instalação Escolha o método de instalação que melhor se adapta ao seu sistema: 

### 1\. No Arch Linux (AUR) O wine-manager está disponível no [Arch User Repository (AUR)](https://aur.archlinux.org/packages/wine-manager). 
**a) Usando um AUR helper (recomendado, ex: yay)** Se você já tem o yay (ou outro AUR helper) instalado:
```bash
yay -S wine-manager
```
**b) Manualmente via git e makepkg** Se você preferir instalar manualmente:
```bash
# Clone o repositório do AUR
git clone https://aur.archlinux.org/wine-manager.git

# Entre no diretório clonado
cd wine-manager

# Compile e instale o pacote
makepkg -si
```
### 2\. Em Outros Sistemas Linux (Instalação Manual)
No seu terminal:
```bash
    # Baixe o script
    sudo wget -O /usr/local/bin/wine-manager https://raw.githubusercontent.com/pedrodev2025/wine-manager/refs/heads/main/wine-manager

    # Dê permissão de execução
    sudo chmod +x /usr/local/bin/wine-manager
```
*É recomendado usar /usr/local/bin/ para scripts instalados manualmente, pois ele geralmente está no seu $PATH e não interfere com pacotes do sistema.*
