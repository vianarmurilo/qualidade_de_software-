# Atividade 3: Estratégia e Projeto de Testes

## 1. Funcionalidade sob Responsabilidade
* **Funcionalidade:** Validação de cupom de desconto na tela de *checkout*.

## 2. Riscos Identificados e Prioridade
* **Risco 1:** O usuário aplicar um cupom expirado ou inválido e o sistema conceder o desconto incorretamente (Prioridade: Alta).
* **Risco 2:** O sistema permitir o uso acumulado de múltiplos cupons quando a regra de negócio permite apenas um por compra (Prioridade: Média).

## 3. Técnica de Teste Escolhida e Aplicação
* **Técnica:** Particionamento de Equivalência e Análise de Valor Limite.
* **Aplicação:** Vamos dividir os dados de entrada em partições válidas (cupons ativos, dentro da validade) e inválidas (cupons expirados, inexistentes ou já utilizados) para verificar como o sistema se comporta.

## 4. Casos de Teste Elaborados
* **Caso de Teste 01 (CT01 - Cupom Válido):**
  * *Objetivo:* Testar a aplicação de um cupom ativo de 10% de desconto.
  * *Passos:* Inserir o código "DESCONTO10" no campo de cupom e clicar em "Aplicar".
  * *Resultado Esperado:* O sistema deve calcular o desconto corretamente, subtraindo 10% do valor total da compra e exibir a mensagem de sucesso.

* **Caso de Teste 02 (CT02 - Cupom Expirado):**
  * *Objetivo:* Testar a tentativa de uso de um cupom fora da validade.
  * *Passos:* Inserir o código "NATAL2024" (expirado) e clicar em "Aplicar".
  * *Resultado Esperado:* O sistema deve recusar o cupom e exibir a mensagem de erro: "Cupom expirado ou inválido".

* **Caso de Teste 03 (CT03 - Campo Vazio):**
  * *Objetivo:* Testar o clique no botão de aplicar sem digitar nenhum código.
  * *Passos:* Deixar o campo em branco e clicar em "Aplicar".
  * *Resultado Esperado:* O sistema deve impedir a ação e avisar que o campo não pode estar vazio.

## 5. Relação entre Funcionalidade, Risco, Técnica e Casos
* A funcionalidade de cupom carrega o risco financeiro de dar descontos indevidos. Usando a técnica de particionamento, criamos casos de teste específicos (CT01, CT02 e CT03) que cobrem tanto o caminho feliz quanto os principais cenários de erro, mitigando os riscos mapeados.

## 6. Decisões Gerais do Plano de Testes
* Os testes manuais serão executados em ambiente de homologação antes de ir para produção.
* Qualquer falha crítica (como aplicar cupom inválido) impede o deploy imediato da funcionalidade até que o erro seja corrigido pelos desenvolvedores.
