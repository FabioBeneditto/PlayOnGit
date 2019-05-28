# PlayOnGit   
#### - Scripts do Wine - para iniciar sem precisar de PlayOnLinux, Proton ou Lutris, inicie direto do menu iniciar com um desempenho muito melhor e superior.
###### Criado por Felipe Facundes
###### Grupo do Telegram: https://t.me/winehq_linux
###### Canal do Telegram: https://t.me/comandos_linux
###### Canal do YouTube: https://www.youtube.com/channel/UCfssKpnkpyUC4sedaZd6N3g
##### Licença: GPLv3

### PRIMEIRO. Aumente a performance com mais +50 de FPS - habilite o Esync.
### SEGUNDO. Diminua a prioridade de SWAP e REINICIE o PC.
```bash
su -c 'echo -e "* hard nofile 1048576" >> /etc/security/limits.conf'
su -c 'echo -e "vm.swappiness=0" > /etc/sysctl.conf'
reboot
```
### TERCEIRO. Certifique-se que o seu driver Vulkan está habilitado. Para plascas Nvídia, basta instalar o driver proprietário. Para placas RADEON da AMD, siga esse meu tutorial abaixo:
https://github.com/felipefacundes/desktop/tree/master/amdgpu
#
# Vamos aos Jogos:

##### Local dos scripts de jogos:

https://github.com/felipefacundes/desktop/tree/master/wine-jogos/

### GTA V - com suporte a DXVK - Veja primeiro o tutorial no youtube:
##### Instalar automaticamente:
`bash <(curl -s https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/GTAV.sh)`
##### Ou instale manualmente:
`wget https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/GTAV.sh`
###### Veja o vídeo, caso queira alterar o caminho do instalador do jogo: `xdg-open GTAV.sh`
```bash
bash GTAV.sh
pkill -9 AutoHotkey.exe
```
###### Clique na figura ▼↓abaixo↓▼ para acessar o tutorial do YouTube:
[![GTA V](https://i.ytimg.com/vi/Lako69C_sw4/hqdefault.jpg)](https://youtu.be/Lako69C_sw4)

### Age Of Empires III - Veja primeiro o tutorial no youtube:
```bash
wget https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/ageofempiresIII.sh
bash ageofempiresIII.sh
```
###### Clique na figura ▼↓abaixo↓▼ para acessar o tutorial do YouTube:
[![Age Of Empires III](https://i.ytimg.com/vi/Di8j04UFY4c/hqdefault.jpg)](https://www.youtube.com/watch?v=Di8j04UFY4c)
