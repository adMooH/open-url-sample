# Breve descrição
Exemplo de como interagir com o adMooH Signage de 2a geração a partir de sua página. Esse repo tem como objetivo servir de exemplo para produção de uma página que será utilizada no sistema adMooH descrito na [FAQ](https://help.admooh.com/i474-o-que-%C3%A9-app-din%C3%A2mico-e-como-habilitar)

# Arquitetura
Sua página será aberta acima dos outros conteúdos ocupando a tela toda, ou seja o ideal é que ela seja parcialmente transparente ou que em determinados momentos ela pause a reprodução dos conteúdos e então fique opaca para exibr o você desejar e depois de um tempo volte a ser transparente e inicie novamente a reprodução dos conteúdos.

# Comando aceitos

## Pausar a reprodução dos conteúdos
```
parent.postMessage("pauseContent","*")
```

## Recomeçar a reprodução dos conteúdos 
```
parent.postMessage("playContent","*")
```

# Exemplo
Nesse repo o arquivo index.html demonstra uma pagina que alterna entre totalmente transparente com a reprodução do conteúdo e totalmente opaca pausando a reprodução do conteúdo a cada 2 minutos
