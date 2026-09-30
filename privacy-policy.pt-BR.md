# Política de Privacidade do UnScroll

**Data de vigência:** 30 de setembro de 2026

Esta Política de Privacidade explica como o **UnScroll** (pacote `com.otvmrnslv.unscroll`, "o Aplicativo") trata as informações. O Aplicativo é desenvolvido por **Almost Done Studios** ("nós").

O UnScroll ajuda você a limitar o tempo gasto nos aplicativos que você escolher. Ele foi projetado para funcionar quase inteiramente no seu dispositivo: não tem contas de usuário, anúncios nem servidores próprios.

---

## 1. Resumo

- O UnScroll usa o **Serviço de Acessibilidade** e o **Acesso ao uso** do Android apenas para detectar quando um aplicativo que você selecionou (ou o feed do YouTube Shorts) está aberto em primeiro plano, para aplicar os limites de tempo que você definiu.
- O UnScroll **não** lê, grava nem transmite suas mensagens, textos digitados, senhas, histórico de navegação ou o conteúdo da sua tela.
- Suas configurações e seu histórico de bloqueios ficam armazenados **somente no seu dispositivo**.
- O Aplicativo usa o **Google Firebase** (Analytics, Crashlytics e Performance Monitoring) para coletar dados limitados e pseudonimizados de uso, falhas e desempenho, para que possamos melhorar a estabilidade.
- **Não** vendemos seus dados nem os usamos para publicidade.

---

## 2. Permissões e por que são usadas

| Permissão | Por que o UnScroll precisa dela |
|---|---|
| **Serviço de Acessibilidade** | Para detectar qual aplicativo está em primeiro plano e, no YouTube, se a aba "Shorts" é a que está selecionada. O Aplicativo só inspeciona a interface na tela para encontrar esse indicador de aba. Ele não lê nem armazena nenhum outro conteúdo da tela, e pode executar a ação "Início" para fechar um aplicativo monitorado quando você escolhe *Fechar app*. |
| **Acesso ao uso** (`PACKAGE_USAGE_STATS`) | Para listar os aplicativos instalados no seu dispositivo, para que você escolha quais deseja monitorar. |
| **Sobrepor a outros apps** (`SYSTEM_ALERT_WINDOW`) | Para exibir a tela de bloqueio sobre um aplicativo monitorado quando seu limite de tempo é atingido. |
| **Notificações** (`POST_NOTIFICATIONS`) | Para mostrar a notificação do cronômetro, avisar se o serviço de monitoramento foi interrompido e enviar um resumo diário do seu progresso. |
| **Serviço em primeiro plano** | Para manter o cronômetro da tela de bloqueio funcionando de forma confiável. |

Você concede cada permissão manualmente nas configurações do Android e pode revogá-las a qualquer momento. Sem elas, o Aplicativo não funcionará corretamente.

---

## 3. Informações armazenadas no seu dispositivo

Os dados a seguir são criados e mantidos **somente no seu dispositivo**. Eles não são enviados para nós:

- **Suas configurações:** a lista de aplicativos que você escolheu monitorar, limites de tempo, durações de pausa e períodos de tolerância.
- **Histórico de bloqueios:** para cada vez que a tela de bloqueio é exibida, o nome do pacote do aplicativo monitorado, a data e a hora, e o resultado (fechado, ignorado ou concluído).
- **Estado do monitoramento:** cronômetros temporários de sessão usados para medir há quanto tempo um aplicativo monitorado está aberto.

Esses dados são usados apenas para aplicar seus limites e mostrar seu próprio progresso, por exemplo na notificação de resumo diário.

### Backup automático do Android

Se o **backup do Google** estiver ativado no seu dispositivo, o Android pode incluir os dados locais do Aplicativo (configurações e histórico de bloqueios) no backup do dispositivo na sua conta Google. Esse backup é gerenciado pelo Google, conforme a [Política de Privacidade do Google](https://policies.google.com/privacy?hl=pt-BR). Nós não temos acesso a ele. Você pode desativar o backup nas configurações do Android.

---

## 4. Informações coletadas por serviços de terceiros

O UnScroll usa os seguintes serviços do Google Firebase. Eles coletam informações automaticamente quando você usa o Aplicativo e as enviam para os servidores do Google.

### Firebase Analytics

Usado para entender, de forma agregada, como o Aplicativo é utilizado, por exemplo com que frequência a tela de bloqueio aparece e se os usuários fecham o aplicativo ou continuam. O Aplicativo registra estes eventos:

- `starting_block`: inclui o tempo de espera configurado para a tela de bloqueio
- `stop_app`: sem parâmetros adicionais
- `continue_app`: inclui o período de tolerância, em minutos, que você selecionou

Esses eventos **não incluem os nomes dos aplicativos que você monitora**. O Firebase Analytics também coleta automaticamente informações como um identificador da instância do aplicativo, modelo do dispositivo, versão do sistema operacional, versão do aplicativo, idioma, localização aproximada (país, região e cidade, obtida a partir do seu endereço IP) e dados de sessão e engajamento.

### Firebase Crashlytics

Usado para diagnosticar falhas. Quando o Aplicativo trava, o Crashlytics coleta o rastreamento da pilha (stack trace), modelo do dispositivo, versão do sistema operacional, versão do aplicativo, o estado do dispositivo no momento da falha (por exemplo memória livre e orientação da tela) e um identificador de instalação.

### Firebase Performance Monitoring

Usado para medir o desempenho do Aplicativo. Coleta dados como tempo de inicialização, desempenho de renderização das telas, tempo de requisições de rede, modelo do dispositivo, versão do sistema operacional e um identificador de instalação.

O Google trata esses dados conforme seus próprios termos:

- [Política de Privacidade do Google](https://policies.google.com/privacy?hl=pt-BR)
- [Privacidade e segurança no Firebase](https://firebase.google.com/support/privacy?hl=pt-br)

Usamos esses dados apenas para manter e melhorar o Aplicativo. Não os combinamos com outros dados para identificar você e não os usamos para publicidade.

---

## 5. Compartilhamento de informações

Não vendemos, alugamos nem trocamos suas informações. Os dados são compartilhados apenas:

- com o **Google (Firebase)**, como prestador de serviços, conforme descrito na Seção 4;
- quando exigido por lei, regulamento ou ordem judicial válida.

Os dados coletados pelo Firebase podem ser processados em servidores do Google localizados fora do Brasil, com as salvaguardas previstas nos termos do Google.

---

## 6. Retenção de dados

- **Dados no dispositivo** permanecem no seu dispositivo até você limpar os dados do Aplicativo ou desinstalá-lo.
- **Dados do Firebase** são mantidos de acordo com as configurações de retenção do Google. Os dados no nível do evento do Analytics são mantidos por até 2 meses, e os dados no nível do usuário (vinculados ao identificador da instância do aplicativo) são mantidos por até 14 meses. Os relatórios de falhas do Crashlytics são mantidos por até 90 dias.

---

## 7. Suas escolhas e controles

- **Apagar dados locais:** acesse *Configurações do Android → Apps → UnScroll → Armazenamento → Limpar dados*, ou desinstale o Aplicativo.
- **Interromper o monitoramento:** desative o Serviço de Acessibilidade ou o Acesso ao uso do UnScroll nas configurações do Android a qualquer momento.
- **Backups:** desative o backup do Google nas configurações do Android para evitar que os dados locais sejam incluídos nos backups do dispositivo.
- **Outras solicitações:** para perguntar sobre, acessar ou excluir dados coletados pelo Firebase, entre em contato conosco (veja a Seção 10). Como não coletamos seu nome, e-mail ou dados de conta, talvez precisemos da sua ajuda para identificar quais dados se referem a você.

### Seus direitos pela LGPD

Nos termos da Lei Geral de Proteção de Dados (Lei nº 13.709/2018), você tem direito a:

- confirmar a existência de tratamento dos seus dados;
- acessar seus dados;
- corrigir dados incompletos, inexatos ou desatualizados;
- solicitar a anonimização, o bloqueio ou a eliminação de dados desnecessários ou excessivos;
- solicitar a portabilidade dos dados;
- obter informações sobre com quem seus dados são compartilhados;
- revogar seu consentimento, quando aplicável;
- apresentar reclamação à Autoridade Nacional de Proteção de Dados (ANPD).

Usuários de outras regiões (por exemplo União Europeia, Reino Unido ou Califórnia) podem ter direitos semelhantes pelas leis locais. Para exercer qualquer um desses direitos, entre em contato conosco.

---

## 8. Segurança

Os dados locais ficam armazenados no espaço privado do Aplicativo, que outros aplicativos não podem acessar em um dispositivo sem root. Os dados enviados ao Firebase são criptografados durante a transmissão por HTTPS. Nenhum método de armazenamento ou transmissão é totalmente seguro, mas adotamos medidas razoáveis para proteger suas informações.

---

## 9. Privacidade de crianças

O UnScroll não é direcionado a crianças menores de 13 anos (ou da idade mínima exigida no seu país). Não coletamos intencionalmente informações pessoais de crianças. Se você acredita que uma criança forneceu informações pessoais por meio do Aplicativo, entre em contato conosco e tomaremos as medidas necessárias para excluí-las.

---

## 10. Contato

Em caso de dúvidas sobre esta Política de Privacidade, entre em contato com:

**Almost Done Studios**
E-mail: **otaviosmarin@gmail.com**

---

## 11. Alterações nesta política

Podemos atualizar esta Política de Privacidade periodicamente. As alterações serão publicadas nesta página com uma nova data de vigência. Mudanças significativas também serão informadas nas notas de versão do Aplicativo.
