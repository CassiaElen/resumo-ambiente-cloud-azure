# **Computação e Rede na Azure**

## **Serviços de Computação do Azure**

- Computação sob demanda: fornece **discos, processadores, memória, redes e sistemas operacionais**.
    
- 💡 **Dica**: Escolha o serviço de computação de acordo com a carga de trabalho: tradicional (VMs), moderno (contêineres), event-driven (Functions).
    

## **Máquinas Virtuais do Azure (VMs)**

- Emulação completa de um computador físico.
    
- Você gerencia o **sistema operacional, armazenamento, e redes**.
    
- Oferta de **IaaS** para controle total e personalização.
    
- 💡 **Dica**: Ideal para cargas de trabalho tradicionais ou migração "lift-and-shift" para a nuvem.
    

## **Conjuntos de Dimensionamento de VMs**

- Permitem **escalar automaticamente** o número de VMs de acordo com a demanda.
    
- **Escala horizontal** (adicionar/remover instâncias).
    
- 💡 **Dica**: Útil para apps web com alta variação de tráfego (ex: lojas virtuais em época de promoções).
    


## **Conjuntos de Disponibilidade de VMs**

- Agrupam máquinas para aumentar a disponibilidade.
    
- Protegem contra falhas de hardware e manutenção programada.
    
- 💡 **Dica**: Sempre crie **Conjuntos de Disponibilidade** para aplicações críticas.
    

## **Área de Trabalho Virtual do Azure**

- Serviço de **virtualização de desktops** baseado em nuvem.
    
- Ambiente multiusuário (várias sessões simultâneas).
    
- 💡 **Dica**: Ideal para trabalho remoto seguro ou ambientes corporativos com acesso a desktops virtuais.
    


## **Serviços de Contêineres do Azure**

- **Contêineres** são ambientes leves, isolados e rápidos.
    
- **Instâncias de Contêiner do Azure** (ACI):
    
    - Execução rápida de contêineres individuais.
        
- **Aplicativos de Contêiner do Azure**:
    
    - Suporte a balanceamento e escalonamento de microsserviços.
        
- **Azure Kubernetes Service (AKS)**:
    
    - Gerenciamento de grandes volumes de contêineres de forma orquestrada.
        
- 💡 **Dica**: Use **ACI** para cargas rápidas e simples e **AKS** para aplicações distribuídas e escaláveis.
    

## **Azure Functions (Serverless)**

- Computação baseada em **eventos**: executa código sob demanda.
    
- Nenhuma infraestrutura para gerenciar entre as execuções.
    
- 💡 **Dica**: Perfeito para automações rápidas, APIs leves e processamento de eventos sem manter servidores ativos.
    


## **Comparação: Opções de Computação**

| Serviço                      | Melhor Uso                                          |
| ---------------------------- | --------------------------------------------------- |
| **Máquinas Virtuais**        | Lift-and-shift de servidores físicos para a nuvem.  |
| **Área de Trabalho Virtual** | Trabalho remoto seguro e acesso a desktops Windows. |
| **Contêineres**              | Microsserviços, apps modernos e escaláveis.         |



## **Serviços de Aplicativo do Azure**

- Plataforma **PaaS** para criação e hospedagem rápida de aplicativos web e APIs.
    
- Suporte para .NET, Java, Node.js, Python e PHP.
    
- 💡 **Dica**: Use para desenvolver **APIs RESTful** ou **sites web** com escalabilidade e segurança integradas.
    

## **Serviços de Rede do Azure**

- **Virtual Network (VNet)**:
    
    - Permite a comunicação segura entre recursos do Azure e redes externas.
        
    - **Pontos de extremidade públicos e privados** para diferentes cenários.
        
- **Sub-redes**:
    
    - Segmentam e organizam a rede virtual.
        
- **Emparelhamento de Redes**:
    
    - Conecta diferentes VNets, sem uso da Internet pública.
        
- 💡 **Dica**: Divida aplicações em sub-redes específicas (ex: app, banco de dados, serviços internos).
    

## **Gateway de VPN**

- Cria uma conexão segura e criptografada entre o Azure e sua rede local.
    
- Usa a **Internet pública** para comunicação.
    
- 💡 **Dica**: Boa opção para pequenas ou médias empresas conectarem infraestrutura local ao Azure.
    

## **ExpressRoute**

- Conexão **privada** (não passa pela internet) entre Azure e seu datacenter.
    
- Alta velocidade e latência mínima.
    
- 💡 **Dica**: Escolha o **ExpressRoute** para cargas críticas que exigem alta confiabilidade e desempenho.
    

## **DNS do Azure**

- Gerenciamento de nomes de domínio usando a infraestrutura do Azure.
    
- Usa a tecnologia **Anycast** para garantir alta disponibilidade e desempenho.
    
- 💡 **Dica**: Integre seu DNS com o Azure para administrar tanto nomes internos quanto públicos em um só lugar.