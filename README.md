# Guia de Instalação do Ubuntu e Acesso via IP

Este guia oferece um passo a passo para a instalação do sistema operacional Ubuntu e detalha como acessá-lo via IP.

## Instalação do Ubuntu

### Requisitos do Sistema

Certifique-se de atender aos seguintes requisitos mínimos:

- **Processador:** 2 GHz dual core ou superior
- **Memória:** 4GB de RAM
- **Espaço em Disco:** 25GB de espaço livre
- **Conexão à Internet**

### Passos para Instalação

1. **Baixe o Ubuntu:**
   - Acesse o [site oficial do Ubuntu](https://ubuntu.com/download) e baixe a versão desejada do sistema operacional.
  
2. **Crie uma Mídia de Instalação:**
   - Grave a imagem ISO em um pendrive ou DVD utilizando ferramentas como o Rufus (Windows) ou dd (Linux).

3. **Inicialize o Computador a partir da Mídia:**
   - Reinicie o computador e inicie a partir do pendrive ou DVD onde o Ubuntu foi gravado.

4. **Instale o Ubuntu:**
   - Siga as instruções na tela para selecionar o idioma, fuso horário, particionamento de disco e criar um usuário.

5. **Conclua a Instalação:**
   - Após a conclusão, reinicie o sistema e remova a mídia de instalação.

## Acesso ao Ubuntu via IP

### Configuração da Rede

1. **Verifique o Endereço IP:**
   - Abra um terminal no Ubuntu e execute o comando:
     ```
     ip addr show
     ```
   - Anote o endereço IP atribuído à sua interface de rede (por exemplo, `192.168.1.100`).

2. **Acesso via SSH (Linux/macOS) ou PuTTY (Windows):**
   - Abra um terminal (Linux/macOS) ou o PuTTY (Windows).
   - Use o comando SSH para acessar o Ubuntu:
     ```
     ssh seu_usuario@seu_endereco_ip
     ```
     Substitua `seu_usuario` pelo nome do seu usuário no Ubuntu e `seu_endereco_ip` pelo endereço IP do Ubuntu.

### Nota Importante
Certifique-se de que o Ubuntu e o dispositivo a partir do qual está tentando acessá-lo estejam na mesma rede local. Se estiverem em redes diferentes, pode ser necessário configurar o roteamento ou a porta de encaminhamento para acessar o Ubuntu remotamente.
