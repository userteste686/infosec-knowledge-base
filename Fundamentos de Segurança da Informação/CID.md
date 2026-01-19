# CID – Confidencialidade, Integridade e Disponibilidade

## 1. Conceito
A CID (Confidencialidade, Integridade e Disponibilidade), também conhecida como **Tríade CIA**, é o modelo fundamental da Segurança da Informação que define os três pilares essenciais para a proteção de dados e sistemas.  
Esse modelo estabelece que qualquer ativo da informação deve ser protegido simultaneamente contra:
- **Acesso não autorizado (Confidencialidade)**,
- **Alterações indevidas (Integridade)**,
- **Indisponibilidade operacional (Disponibilidade)**.

A CID serve como base para políticas de segurança, controles técnicos, frameworks de governança, normas internacionais (como ISO/IEC 27001) e arquiteturas de segurança corporativa. Todo controle de segurança implementado em uma organização existe para garantir, direta ou indiretamente, pelo menos um desses três pilares.

---

## 2. Funcionamento
O funcionamento da CID ocorre pela aplicação de **controles de segurança** mapeados a cada pilar:

- **Confidencialidade**
  - Controle de acesso
  - Autenticação e autorização
  - Criptografia
  - Segregação de funções
  - Classificação da informação

- **Integridade**
  - Hashing
  - Assinaturas digitais
  - Controle de versões
  - Logs e auditoria
  - Validação de dados

- **Disponibilidade**
  - Redundância
  - Backup
  - Failover
  - Balanceamento de carga
  - Proteção contra DDoS
  - Planos de continuidade de negócio

Esses controles atuam de forma integrada, garantindo que a informação permaneça protegida durante todo o seu ciclo de vida: criação, processamento, armazenamento, transmissão e descarte.

---

## 3. Exemplos práticos

**Confidencialidade**
- Uso de criptografia TLS em comunicações web  
- Controle de acesso por ACL em servidores  
- Autenticação multifator (MFA) em sistemas corporativos  

**Integridade**
- Hash de arquivos para verificação de alteração  
- Logs imutáveis em SIEM  
- Assinaturas digitais em documentos eletrônicos  

**Disponibilidade**
- Cluster de servidores em alta disponibilidade  
- Backup diário automatizado  
- Proteção contra ataques DDoS  
- Links redundantes de internet  

---

## 4. Impactos em Segurança
A quebra de qualquer pilar da CID gera impactos diretos:

- **Quebra da Confidencialidade**
  - Vazamento de dados
  - Espionagem
  - Fraude
  - Violação de LGPD/GDPR

- **Quebra da Integridade**
  - Manipulação de informações
  - Fraudes financeiras
  - Decisões baseadas em dados corrompidos
  - Perda de confiabilidade dos sistemas

- **Quebra da Disponibilidade**
  - Paralisação operacional
  - Perda financeira
  - Interrupção de serviços críticos
  - Impacto reputacional

---

## 5. Mitigações e Controles

**Controles técnicos**
- Criptografia em repouso e em trânsito  
- Firewall e IDS/IPS  
- SIEM e monitoramento contínuo  
- Backup e replicação  
- Controle de acesso baseado em função (RBAC)  

**Controles administrativos**
- Políticas de segurança da informação  
- Gestão de identidades e acessos  
- Classificação da informação  
- Segregação de funções (SoD)  
- Treinamento de usuários  

**Controles físicos**
- Controle de acesso físico  
- Monitoramento por câmeras  
- Datacenters seguros  
- Proteção ambiental  

---

## 6. Aplicação prática
No contexto operacional:

- **SOC**
  - Monitoramento de violações de confidencialidade
  - Detecção de alteração de integridade em logs
  - Resposta a incidentes de indisponibilidade

- **Blue Team**
  - Implementação de controles CID
  - Hardening de sistemas
  - Arquitetura segura

- **Red Team**
  - Exploração de falhas de confidencialidade
  - Manipulação de integridade de dados
  - Ataques de negação de serviço

- **Governança**
  - Base para políticas de segurança
  - Análise de riscos
  - Conformidade regulatória
  - Auditorias de segurança

A CID é o **alicerce conceitual de toda a Segurança da Informação**. Nenhum sistema, política, controle, ataque ou defesa existe fora desses três pilares.
