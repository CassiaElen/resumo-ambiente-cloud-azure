# **Identidade, Acesso e Segurança**

## **Microsoft Entra ID**

_(Serviço de identidade e acesso baseado em nuvem no Azure)_

### **Funções principais:**

- **Autenticação**: funcionários fazem login para acessar recursos.
    
- **Logon Único (SSO)**: um único login para múltiplos aplicativos.
    
- **Gerenciamento de Aplicativos**: controle de quais apps os usuários acessam.
    
- **B2B (Business-to-Business)**: colaboração segura entre empresas.
    
- **Gerenciamento de Dispositivos**: controle sobre os dispositivos usados.
    


## **Microsoft Entra Domain Services**

- Fornece **serviços de domínio na nuvem** sem precisar de controladores de domínio tradicionais.
    
- Suporta **aplicativos legados** que não usam autenticação moderna.
    
- **Sincroniza automaticamente** com o Microsoft Entra ID.
    
- 💡 **Dica**: Ideal para empresas que precisam manter apps antigos funcionando na nuvem.
    


## **Comparando Autenticação e Autorização**

|Termo           |Significado                                                                |
|----------------|---------------------------------------------------------------------------|
|**Autenticação**|Verifica _quem é_ a pessoa/serviço (ex.: login e senha).                   |
|**Autorização** |Define _o que_ a pessoa/serviço pode acessar e fazer depois de autenticado.|


## **Autenticação Multifator (MFA)**

- Exige **2 ou mais fatores** para autenticar:
    
    - Algo que você **sabe** (senha).
        
    - Algo que você **possui** (celular/token).
        
    - Algo que você **é** (biometria: impressão digital, reconhecimento facial).
        

💡 **Dica**: MFA é uma prática **essencial** para proteger identidades na nuvem.


## **B2B e B2C no Microsoft Entra**

- **B2B External ID**:
    
    - Permite que parceiros externos acessem seus recursos **com segurança**.
        
- **B2C External ID**:
    
    - Permite que **clientes** usem suas próprias identidades (ex.: Google, Facebook) para acessar seus aplicativos.
        


## **Acesso Condicional**

- Impõe políticas de acesso baseadas em:
    
    - Usuário ou grupo.
        
    - Localização do IP.
        
    - Dispositivo usado.
        
    - Aplicativo acessado.
        
    - Detecção de risco.
        

💡 **Dica**: Pode forçar o uso de MFA apenas em acessos considerados arriscados!


## **Controle de Acesso Baseado em Função (RBAC)**

- **Granularidade fina** no acesso: apenas o mínimo necessário para a função do usuário.
    
- Permite controlar quem gerencia e acessa **recursos do Azure**.
    
- 💡 **Dica**: Use RBAC para separar as funções (ex.: Admin, Operador, Leitor).
    


## **Confiança Zero ("Zero Trust")**

- Não confiar **em nada por padrão**, nem dentro da rede corporativa.
    
- Sempre validar:
    
    - Identidade.
        
    - Dispositivo.
        
    - Localização.
        


## **Proteção Completa no Azure**

- **Camadas de Segurança**:
    
    - Física (datacenter).
        
    - Identidade e acesso.
        
    - Perímetro da rede.
        
    - Aplicativos.
        
    - Dados.
        
- **Defesa em Profundidade**: proteção redundante para isolar ataques.
    


## **Microsoft Defender para Nuvem**

- Serviço de monitoramento de segurança no Azure e datacenters locais.
    
- **Principais funções**:
    
    - Recomendações de segurança.
        
    - Detecção e bloqueio de malware.
        
    - Identificação de ataques potenciais.
        
    - Controle de acesso "Just-in-Time" (libera portas temporariamente e sob demanda).