# vagrant-templates

  

### Objetivo
Centralizar padrões de criação de Maquinas Virtuais (VM) utilizando Vagrant e Virtual Box.
Todas VM possui a configuração de rede como Bridge e IP Fixo, caso aja a necessidade essas configurações podem ser modificadas.

**Informações Adicionais:**

Todos os arquivos Vagrantfile possui variáveis que podem ser manipuladas conforme sua preferencia como mostra o exemplo abaixo:

    SONAME = "ubuntu/bionic64" # Nome da vbox a ser utilizada 
    VMNAME = "Ubuntu18" # Nome da VM
    HOSTNAME = "ubuntu18-server" # Hostname do sistema
    IPADDRESS = "" # Endereço de IP Fixo
    NETWORK_ADAPTER = "" # Adaptador de rede a ser utilizado pelo VM
    MEMORY = "1024" # Total de memória do sistema
    PUBLIC_SSHKEY_PATH = "~/.ssh/id_dsa.pub" # Caminho da sua chave publica
    
**Variáveis obrigatórias**
Para o funcionamento da VM é obrigatório preencher as seguintes variáveis do seu Vagrantfile:

    IPADDRESS = "" # Endereço de IP Fixo
    NETWORK_ADAPTER = "" # Adaptador de rede a ser utilizado pelo VM

---
### Sistemas Operacionais

- CentOS
- Debian
- Ubuntu
- FreeBSD