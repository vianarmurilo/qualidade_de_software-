# Atividade 1: Fundamentos e Características da Qualidade

## 1. Funcionalidade Escolhida
* **Módulo:** Tela de *Checkout* (Finalização de Compra em um E-commerce).

## 2. Necessidades do Usuário
* **Necessidade Explícita:** O sistema precisa dar a opção para o cliente escolher a forma de pagamento (Pix ou Cartão) e finalizar a compra preenchendo os dados de cobrança corretamente.
* **Necessidade Implícita:** A gente espera que a plataforma não trave na hora de pagar, que seja super rápida e que nossos dados pessoais e financeiros não vazem de jeito nenhum.

## 3. Requisito de Qualidade Formulado
* "O sistema de pagamento deve processar as transações via Pix em no máximo 3 segundos e usar criptografia de ponta a ponta (HTTPS/TLS 1.3) para proteger todas as informações confidenciais enviadas pelo usuário."

## 4. Características e Subcaracterísticas (Norma ISO/IEC 25010)
* **Desempenho (Performance Efficiency):**
  * *Subcaracterística:* Comportamento Temporal (Time Behavior) – garante que o sistema responda rápido, respeitando o limite de 3 segundos.
* **Segurança (Security):**
  * *Subcaracterística:* Confidencialidade (Confidentiality) – garante que os dados sensíveis do cartão e do cliente fiquem protegidos por criptografia.

## 5. Como o Requisito Poderia ser Avaliado
* **Para testar o desempenho:** A gente usaria uma ferramenta de teste de carga (como o JMeter) para simular várias pessoas pagando ao mesmo tempo e ver se o tempo de resposta se mantém abaixo de 3 segundos.
* **Para testar a segurança:** Faríamos uma inspeção no certificado SSL/TLS e varreduras para checar se o tráfego de dados está realmente criptografado e seguro.
