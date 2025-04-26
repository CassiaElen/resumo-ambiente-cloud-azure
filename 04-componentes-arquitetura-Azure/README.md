#  **Componentes de Arquitetura do Azure**

## **Regiões**

- São áreas geográficas que contêm um ou mais datacenters próximos.
    
- A Azure possui **mais de 60 regiões**, cobrindo mais de 140 países.
    
- **Benefícios**:
    
    - Reduzem a latência de acesso aos dados.
        
    - Ajudam a manter a **residência dos dados** com opções de conformidade local.
        
- 💡 **Dica**: Escolha a região mais próxima dos seus usuários finais para garantir melhor performance e conformidade legal.
    


## **Zonas de Disponibilidade**

- Conjuntos de datacenters com energia, refrigeração e redes **independentes**, mas interconectadas.
    
- Ajudam a proteger aplicativos e dados contra falhas de datacenter local.
    
- 💡 **Dica**: Para alta disponibilidade, implante suas **VMs em diferentes zonas** dentro da mesma região.
    

## **Pares de Regiões**

- Conjuntos de duas regiões **separadas por no mínimo 300 milhas**.
    
- Usadas para **replicação automática** e **recuperação prioritária** em caso de falha.
    
- 💡 **Dica**: Use **pares de regiões** ao planejar sua estratégia de recuperação de desastres.
    

## **Regiões Soberanas do Azure**

- **Azure Governamental (EUA)**:
    
    - Instância separada e isolada.
        
    - Atende exigências rigorosas de agências públicas e fornecedores.
        
- **Azure China**:
    
    - Gerido por 21Vianet, com conformidade com regulamentos chineses.
        
    - Os dados ficam **restritos dentro da China**.
        
- 💡 **Dica**: Use essas regiões apenas se tiver obrigações legais específicas nesses países.
    

## **Recursos do Azure**

- São os **blocos de construção** de soluções na nuvem.
    
- Exemplos:
    
    - Máquinas Virtuais
        
    - Armazenamento
        
    - Redes Virtuais
        
    - Bancos de Dados
        
    - Serviços de Aplicativos
        
- 💡 **Dica**: Use **tags** para organizar seus recursos e facilitar o monitoramento e os relatórios.
    

## **Grupos de Recursos**

- Um **container lógico** para agrupar e gerenciar recursos relacionados.
    
- Características:
    
    - Recursos só podem estar **em um grupo por vez**.
        
    - Podem estar **em diferentes regiões**.
        
    - **Podem ser movidos** entre grupos.
        
- 💡 **Dica**: Crie grupos por **ambiente (Dev/Test/Prod)** ou por **aplicação** para facilitar a gestão e a automação com templates.
    

## **Assinatura do Azure**

- Garante acesso **autenticado e autorizado** aos serviços.
    
- Tipos comuns:
    
    - **Desenvolvimento**
        
    - **Teste**
        
    - **Produção**
        
- Permite:
    
    - **Relatórios de cobrança** separados.
        
    - **Controle de acesso refinado**.
        
- 💡 **Dica**: Use múltiplas assinaturas para isolar ambientes e definir limites de orçamento.
    

## **Grupos de Gerenciamento**

- Hierarquia para organização de múltiplas assinaturas:
- Grupos de Gerenciamento ➝ Assinaturas ➝ Grupos de Recursos ➝ Recursos
- 💡 **Dica**: Ideal para empresas com **várias equipes** ou **divisões**, pois permite aplicar políticas e controle de acesso de forma centralizada.
