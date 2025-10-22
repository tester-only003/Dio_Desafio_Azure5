# Computação e Rede na Azure 

- Comparar tipos de computação, incluindo instâncias de container, máquinas virtuais e funções. <br>
- Descrever os recursos exigidos para as máquinas virtuais. <br>
- Definir pontos de extremidade públicos e privados. <br>
- Descrever as opções de máquina virtual, incluindo VMs, conjuntos de dimensionamento de máquinas virtuais, conjuntos de disponibilidade de máquinas virtuais e a Área de Trabalho Virtual do Azure. <br>
<br>

### Serviços de Computação do Azure

 A **Computação do Azure** é um serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

<img  width="530" height="123" alt="Servicos-computacao1" src="https://github.com/user-attachments/assets/01d6fa06-508e-4ccd-abcc-6a0898ce29fe" />
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

<img width="680" height="316" alt="Conjunto-disponibilidade-vm1" src="https://github.com/user-attachments/assets/528f0bb2-a567-402b-9ad7-1639afa4af6a" />
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

















