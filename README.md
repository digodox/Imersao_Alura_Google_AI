# Imersao_Alura_Google_AI - Assistende de Operação e Manutenção em Plantas Industriais
Projeto da imersão em Generative AI da Alura/Google

# Objetivo:
Criar um assistente para correlacionar diferentes informações sobre instalações industriais considerando suas documentações de projeto, racionalização de alarmes, atuação de alarmes em tempo real e análise de variáveis de processo em tempo real.

# Descrição
Para o projeto foram criadas 4 planilhas com informações das instalações:
* Planilha **Alarmes.xlsx** - Apresenta quais alarmes estão atuados ou não no sistema de monitoramento das estações. Em uma aplicação real, estes dados seriam coletados diretamente da base de dados de Alarmes do sistema de supervisão e controle (SCADA).
* Planilha **TAGs_Analogicos.xlsx** - Apresenta as variáveis analógicas das estações com seus respectivos valores e unidades de engenharia. Em uma aplicação real, esses dados seriam coletados da base de dados de processo do sistema SCADA.
* Planilha **Limites Operacionais.xlsx** - Define os limites operacionais de projeto como, por exemplo, pressão máxima de entrada. Caso a pressão ultrapasse os limites operacionais, há risco de danos aos equipamentos das instalações.
* Planilha **Racionalizacao_de_alarmes.xlsx** - Define, para cada alarme do sistema, quais as prováveis causas, consequências e ações a serem tomadas pela equipe de Operação e Manutenção. Além disso, define as prioridades de cada alarme (Baixa, Média, Alta ou Crítica).

Usando os dados das planilhas como contexto para o modelo, é possível solicitar informações gerais e específicas sobre os alarmes ou o estado geral das estações. Dessa forma, o modelo será capaz de correlacionar as diferente informações disponíveis e indicar de forma acertiva a condição e atuação que deve ser tomada para um eventual problema.

Além disso, seria possível (em uma implementação futura) adicionar documentos específicos dos equipamentos de cada instalação. Permitindo que o modelo indique qual a melhor estratégia de reparo para uma falha qualquer.

# Utilização:
* Inicialmente é necessário importar e atualizar o caminho das planilhas, caso necessário.
* Em seguida é necessário alterar a API KEY para utilização do modelo (https://ai.google.dev/gemini-api/docs/api-key)
* Finalmente, basta perguntar!

