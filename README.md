# Computação e Rede na Azure 

- Comparar tipos de computação, incluindo instâncias de container, máquinas virtuais e funções. <br>
- Descrever os recursos exigidos para as máquinas virtuais. <br>
- Definir pontos de extremidade públicos e privados. <br>
- Descrever as opções de máquina virtual, incluindo VMs, conjuntos de dimensionamento de máquinas virtuais, conjuntos de disponibilidade de máquinas virtuais e a Área de Trabalho Virtual do Azure. <br>
<br>

### Serviços de Computação do Azure

 A **Computação do Azure** é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

   <div align="center">
   <img  width="530" height="123" alt="Servicos-computacao1" src="https://github.com/user-attachments/assets/01d6fa06-508e-4ccd-abcc-6a0898ce29fe" />
   </div>
<br>

### Máquinas virtuais do Azure
- As máquinas virtuais do Azure (VMs) são emulações de software de computadores físicos.
- Inclui processador virtual, memória, armazenamento e rede.
- Oferta de IaaS que oferece personalização e controle total.
<br>

### Conjuntos de DIMENSIONAMENTO de VMs
Os conjuntos de dimensionamento oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente.

- Escalar horizontalmente quando o recurso precisar aumentar.
- Reduzir horizontalmente quando o recursos precisar diminuir.

***NÃO É LOAD BALANCE***

<br>

### Conjuntos de DISPONIBILIDADE de VMs

   <div align="center">
   <img width="680" height="316" alt="Conjunto-disponibilidade-vm1" src="https://github.com/user-attachments/assets/528f0bb2-a567-402b-9ad7-1639afa4af6a" />
   </div>
<br>

Domínio de falha == Rack
(sentido vertical da imagem acima)

Domínio de atualização ==  contém as máquinas virtuais; 
(identificada no sentido horizontal na imagem acima (VM1 | VM2 | VM3 …))

<br>

### Área de Trabalho Virtual do Azure
Se trata de uma virtualização de área de trabalho e aplicativo executada na nuvem.

- Crie um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway.

- Reduza o risco de que o recurso seja deixado para trás.

- Implantações reais de várias sessões.

- Entrega um gerenciamento mais centralizado

<br>

### Serviço de Container do Azure
Os contêineres do Azure fornecem um ambiente leve e virtualizado que não exige o gerenciamento do sistema operacional e pode responder a alterações sob demanda.

Contêiner é um ambiente de virtualização diferente de uma VM por não possuir processador, disco, memória, sistema operacional. Possui uma rotina, ou seja, é como subir um serviço e quando não precisar mais o eliminamos.

- + Leve que uma VM;
- Projetado para ser interrompido;
- Pode ser recriado quantas vezes for preciso;

**Dentro do Azure, nós temos vários modelos de serviços de contêiner.** 

<br>

### Instâncias de contêiner do Azure
Uma oferta de PaaS que executa um contêiner ou pod de contêineres no Azure.

<br>

### Aplicativos de contêiner do Azure: 
Uma oferta de PaaS, como instâncias de contêineres, que pode balancear a carga e escalar.

- Permite que se trabalhe de forma imediata, removendo essa parte de gerenciamento de contêineres;

<br>

### Serviço de Kubernetes do Azure 
Um serviço de orquestração para contêineres com arquiteturas distribuídas e grandes volumes de contêineres.

<br>

### Azure Functions
Uma oferta de PaaS que dá suporte a operações de computação sem servidor.

   O Código baseado em eventos é executado quando chamado, sem exigir uma infraestrutura de servidor durante períodos inativos.

   ***“A soluções podem ser usadas quando você precisa executar um trabalho em resposta à um evento e, por isso, iremos executá-la por meio de uma solicitação (chamada de rest)... as funções serão dimensionadas automaticamente com base na demanda.”***

   **Palavra chave: Execução baseada em eventos**

<br>

#### Comparar opções de computação do Azure

Máquina virtuais
- Servidor baseado em nuvem que dá suporte a ambientes Windows ou Linux.
- Útil para migrações de lift-and-shift para a nuvem.<br>
                  lift-and-shift == levar como está
- Pacote do sistema operacional completo, incluindo o sistema operacional do host.

<br>

#### Área de Trabalho Virtual
- Fornece uma experiência de área de área de trabalho do Windows baseada em nuvem.
- Aplicativos dedicados para conexão e uso ou acessíveis de qualquer navegador moderno.
- O logon de vários clientes permite que vários usuários façam logon no mesmo computador ao mesmo tempo.

<br>

#### Contêineres
- Ambiente leve e em miniatura adequado para a execução de microsserviços.
- Projetado para escalabilidade e resiliência por meio da orquestração **(orquestração feita pelo AKS)**.

- Aplicativos e serviços são empacotados em um contêiner que fica na parte superior do sistema operacional do host. Vários contêineres podem ficar em um sistema operacional do host.

<br>

### Serviços de Aplicativo do Azure
Os serviços de aplicativos do Azure consistem em uma plataforma totalmente gerenciada para criar, implantar e dimensionar aplicativos Web e APIs rapidamente.

- Trabalha com .NET, .NET Core, Node.js, Java, Python ou php.
- Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.

<br>

### Serviços de Rede do Azure
A Rede Virtual do Azure (VNet) permite que os recursos do Azure se comuniquem uns com os outros, com a Internet e com as redes locais.

- Pontos de extremidade públicos, acessíveis de qualquer lugar na internet.

- Pontos de extremidade privados, acessíveis somente de dentro da sua rede.

   - As sub-redes virtuais segmentam sua rede para atender às suas necessidades.

   - O emparelhamento de rede conecta suas redes privadas diretamente

<br>

### Serviços de Rede do Azure: Gateway de VPN
Gateway de VPN é usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela internet pública.

   <div align="center">
   <img width="723" height="185" alt="Gateway-VPN1" src="https://github.com/user-attachments/assets/a0305bad-cec4-465a-a6f1-c017ca5a6188" />
   </div>


<br>
<br>

### Serviços de Rede do Azure: ExpressRoute
*É um cabo do datacenter da empresa até o datacenter da Microsoft.*

O **ExpressRoute** estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade.

   <div align="center">
   <img width="713" height="284" alt="Express-Route1" src="https://github.com/user-attachments/assets/8d17264f-90ee-470c-83ac-de96e6a5ce91" />
   </div>

<br>
<br>

### DNS do Azure
- Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando a rede Anycast.

- A segurança do DNS do Azure baseia-se no gerenciador de recursos do Azure, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log.

- Facilidade de uso para gerenciar recursos externos e do Azure com um único serviço DNS.

- As redes virtuais personalizáveis permitem que você use nomes de domínio privados e totalmente personalizados em suas redes virtuais.

- Os registros de alias dão suporte a conjuntos de registros de alias para apontar diretamente para um recurso do Azure.
<br>


### Computação e Rede - Revisão
- Tipos de computação, instâncias de contêiner, máquinas virtuais e funções.

- Opções de hospedagem de aplicativos, Aplicativos Web do Azure, contêineres e máquinas virtuais.

- Redes virtuais, sub-redes, emparelhamento, DNS do Azure, Gateway de VPN e ExpressRoute.

<br>


### Links para Estudar
[https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/6-functions](https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/6-functions)

[https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/12-domain-name-system](https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/12-domain-name-system)

[https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/11-expressroute/](https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/11-expressroute/)

[https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/9-exercise-configure-network-access/](https://learn.microsoft.com/training/modules/describe-azure-compute-networking-services/9-exercise-configure-network-access/)












