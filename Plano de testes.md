# Plano e Cenários de Testes 

## 1. Identificação
- Nome do Projeto: E-commerce médico
- Versão Avaliada: V1
- Ambiente de Testes: dev, homolog e prod.
- Tipo de Teste: Teste Funcional Manual
- Data do Documento: 30/10/2025
- Responsável: Júlia Teles

## 2. Objetivo:
> Validar as funcionalidades e fluxos principais do sistema, garantindo que os comportamentos estejam de acordo com os requisitos definidos e que as informações sejam exibidas corretamente.


## 3. Escopo 
Os teste svão cobrir: 
  - Acesso à plataforma (homepage)
  - Login e autenticação de paciente e admin (AdminMaster, Financeiro e Atendente)
  - Navegação pela área logada (sidebar e header fixo)
  - Visualização e filtros da tela de orçamentos
  - Visualização dos detalhes de orçamentos
  - Acesso e edição de informações em configurações

O que não vai ser testado no momento: 
  - Testes em dispositivos móveis
  - Testes de integração com sistemas externos
  - Testes de performance ou carga

## 4. Pré-requisitos gerais
  - O paciente deve possuir cadastro prévio com CPF e senha
  - Deve haver orçamentos associados ao CPF do paciente para exibição nas listagens

## 5. Ferramentas Utilizadas
  - Navegador Google Chrome / Edge
  - Ferramentas de inspeção do navegador (DevTools)
  - Google Sheets / Docs e Linear (reportar bugs e registrar evidências)
  - Extensões:
      - Check my links
      - Jam

## 6. Técnicas de Teste
  - Particionamento de equivalência
  - Caminho feliz (Happy Path)
  - Testes exploratórios

## 7. Critérios de Aceitação
  - Todos os casos de teste devem passar com sucesso, conforme o resultado esperado.
  - Nenhuma falha crítica deve estar presente em funcionalidades principais.
  - Mensagens de erro e validações devem ser consistentes.

## 8. Critérios de Saída 
  - Todos os testes do escopo foram executados.
  - Bugs foram registrados, analisadas e fluxos reexecutados se necessário.
  - Documentação de evidências de sucesso e falhas está completa.

## 9. Cronograma Estimado
| Atividade                   | Data Início | Data Fim   |
| --------------------------- | ----------- | ---------- |
| Planejamento de Testes      | 06/10/2025  | 10/10/2025 |
| Criação de Casos de Teste   | 10/10/2025  | 17/10/2025 |
| Execução dos Testes Manuais | 17/10/2025  |  -         | 
| Registro e Report de Bugs   | 17/10/2025  |     -      |
| Encerramento e Evidências   | 13/05/2025  |     -      |



### 10. **Módulos para serem testados**

| Código RF | Módulo                   | Prioridade |
| --------- | ------------------------ | ---------- |
| RF01      | Autenticação de Usuários |    Alta    |
| RF02      | HomePage                 |    Média   |
| RF03      | Área de Paciente         |    Alta    |
| RF04      | Área de Administração    |    Alta    |
| RF05      | Pagamento                |    Alta   |

---

### 11. **Gestão de Defeitos**

* Bugs serão documentados com:

  * Título
  * Descrição
  * Fluxo para reproduzir
  * Evidência (print ou vídeo)
  * Gravidade (Crítica, Alta, Média, Baixa)
* Ferramenta sugerida: homologação (para simulação)

### 12. **Riscos Identificados**
| Risco                                  | Impacto | Mitigação                        |
| -------------------------------------- | ------- | -------------------------------- |
| Sistema fora do ar                     | Alto    | Tentar novamente após intervalo  |
| Dados da demo não sendo persistentes   | Médio   | Refazer cenários se necessário   |
| Testes limitados à conta "Admin" única | Médio   | Documentar esse limite no escopo |



