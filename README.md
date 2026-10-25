# Design-Sprint-de-Tecnologia-Social

# Design Sprint de Tecnologia Social — Engenharia Frugal & Metodologia Maker
**Instituição:** Universidade Católica de Brasília (UCB)  
**Metodologia:** Aprendizagem Baseada em Problemas (PBL) & Design Sprint (40 min)  
**Desafio Territorial:** Creche Comunitária no Sol Nascente/DF (70 crianças, faturas elevadas de água/energia e passivo de sucata informática/PCs avariados).  
**Nome:** Pedro Lucas Lopes de Melo
**Data:** 25/10/2026  

---

## 1. Diagnóstico Comunitário & Salvaguardas do ECA (10 min)

### 1.1 Mapeamento da Carência (Abordagem Não Tecnocêntrica)
* **Descentralização da Solução:** A prioridade imediata da creche não é a aquisição de computadores topo de gama, mas a redução do custo fixo de manutenção básica (água para limpeza/sanitários e energia para banho/refeições). A tecnologia deve apoiar a rotina já existente sem introduzir dependências de assistência técnica externa ou custos de licenciamento.
* **Pactuação Horizontal com os Voluntários:** As decisões de montagem e operação partem do conhecimento dos próprios voluntários e merendeiras da creche. A equipa de engenharia atua como facilitadora técnica de montagem frugal, respeitando os horários da instituição e adaptando as intervenções ao espaço físico disponível.

### 1.2 Salvaguardas Práticas do ECA (Lei 8.069/90) no Ambiente Infantil
* **Art. 17 e Art. 18 (Direito ao Respeito, Integridade Física e Proteção contra Riscos):**
  * **Segurança Física Frugal:** O reservatório hídrico e os pontos de captação ficam isolados do pátio comum através de fecho mecânico trancado com cadeado, evitando qualquer risco de queda, afogamento ou contacto com água não filtrada.
  * **Higiene e Sanidade:** Instalação de filtro de malha fina de retenção de sedimentos e ralo de descarte da primeira água da chuva (first-flush), impedindo a contaminação por dejetos do telhado e garantindo o uso restrito da água de chuva para descargas e lavagem de pátios.
  * **Segurança Elétrica e Fiação:** A bancada de computadores recuperados tem as fontes de alimentação e calhas elétricas embutidas em canaletas de PVC aparafusadas na parede acima da altura de alcance das crianças (mínimo de 1,60 m), com disjuntor diferencial residual (DR) de proteção contra choques acidentais.

---

## 2. Arquitetura Frugal, Metarreciclagem & Orçamento (15 min)

### 2.1 Integração Técnica Frugal
A solução conjuga duas frentes de impacto imediato a custo reduzido:

1. **Cisterna de Captação Pluvial Modular (Barril/PET) com Descarte de Primeira Chuva:**
   * Captação da água da calha do telhado com desviador mecânico de resíduos sólidos e boia de corte automático. A água acumulada alimenta diretamente a lavagem das áreas externas e os autoclismos/sanitários da creche, reduzindo a fatura da concessionária local em até 35%.
2. **Laboratório Pedagógico via Metarreciclagem e Linux Ultraleve:**
   * Triagem dos computadores avariados acumulados: canibalização de peças funcionais (troca de módulos de RAM e fontes em bom estado entre gabinetes).
   * Substituição de discos rígidos mecânicos danificados por pens USB configuradas como *Live USB persistente* ou SSDs SATA de entrada reaproveitados.
   * Sistema Operativo: **Lubuntu (LXQt) ou Antix Linux**, consumindo menos de 300 MB de RAM em repouso, com instalação local da suíte educativa GCompris e navegadores otimizados com bloqueador de anúncios para poupar largura de banda.

### 2.2 Orçamento Estrito (Limite R$ 250,00)
Todo o material é adquirido localmente no comércio do Sol Nascente ou reaproveitado de sucata:

| Item | Origem / Aplicação | Qtd | Valor Unitário | Total (R$) |
| :--- | :--- | :---: | :---: | :---: |
| **Barril Plástico 200L com Tampa (Reaproveitado)** | Comércio local de embalagens (ex-indústria alimentícia limpo) | 1 un | R$ 90,00 | R$ 90,00 |
| **Tubos PVC 75mm, Curvas e Junções** | Loja de materiais de construção local (conexões da calha) | 2 barras + conexões | — | R$ 55,00 |
| **Torneira de Esfera 3/4" e Flanges de Caixa** | Saída da cisterna e ladrão de escape | 2 kits | R$ 18,00 | R$ 36,00 |
| **Pasta Térmica + Álcool Isopropílico** | Manutenção e limpeza das motherboards/processadores dos PCs | 1 kit | R$ 25,00 | R$ 25,00 |
| **Filtro de Tela Mosquiteira de Alumínio** | Bloqueio mecânico contra larvas de mosquito (Dengue) | 1 metro | R$ 14,00 | R$ 14,00 |
| **Extensão com Disjuntor / Régua de Tomadas** | Alimentação protegida para a bancada de computadores | 1 un | R$ 30,00 | R$ 30,00 |
| **TOTAL GERAL** | | | | **R$ 250,00** |

*(Nota: Fita teflon, parafusos e abraçadeiras metálicas foram articulados com o estoque residual da própria manutenção comunitária da creche).*

### 2.3 Mecanismo Poka-Yoke e Independência de Ferramentas
* **Conexões de Engate Manual:** Todo o encanamento externo utiliza conexões soldáveis com bucha roscável ou engates rápidos sem necessidade de termofusão ou ferramentas mecânicas pesadas.
* **Cores Indicativas de Circuito:** As mangueiras de descarte de sedimentos e a torneira de saída limpa usam marcações por fita colorida (Azul = Utilização Geral; Vermelho = Manutenção/Limpeza da Primeira Chuva), impossibilitando erros de manobra por leigos.
* **Boot Automatizado:** Os computadores recuperados são configurados na BIOS para arranque automático diretamente na interface pedagógica simplificada, bloqueando acesso root ou ecrãs de linha de comando para evitar desconfigurações acidentais.

---

## 3. Plano de Autonomia, Manuais & Pitch (15 min)

### 3.1 Esboço de Manual Visual Plastificado (Guia de Manutenção em 3 Passos)
Um painel A4 afixado na parede, plastificado com fita adesiva larga contra poeira e salpicos de água[cite: 2]:

```text
=====================================================================
         GUIA RÁPIDO DO SISTEMA DE ÁGUA E COMPUTADORES (CRECHE)
=====================================================================

[ 1. ANTES DA CHUVA FORTE ]
  * Olhe o tubo transparente do descarte.
  * Certifique-se de que a torneira vermelha da ponta de baixo está FECHADA.
  * O primeiro fluxo de água suja ficará preso no tubo antes de encher o barril.

[ 2. APÓS A CHUVA ]
  * Abra a torneira vermelha para esvaziar a água barrenta no ralo do pátio.
  * Use a torneira AZUL do tambor grande para baldes de limpeza e chão.
  * ATENÇÃO: Água exclusiva para limpeza e descarga. NÃO beber nem cozinhar!

[ 3. COMPUTADORES (LIGAR E DESLIGAR) ]
  * Ligue apenas a chave central da régua de tomadas na parede.
  * O sistema entra direto nos jogos infantis (GCompris).
  * Para desligar: aperte 1 vez o botão redondo do gabinete (desligamento automático).
=====================================================================

### 3.2 Plano de Transição: Coensino, Operação Assistida e Emancipação Soberana
* **Coensino (Semana 1):** Oficina de meio período com 3 voluntários da creche para montagem guiada da tubulação da cisterna e canibalização/limpeza do primeiro PC.
* **Operação Assistida (Semanas 2 a 4):** A equipe da creche opera o sistema de água e o laboratório com canal de suporte direto via WhatsApp para eventuais dúvidas operacionais.
* **Emancipação Soberana (Mês 2 em diante):** A própria equipe comunitária assume o ciclo semanal de descarte de sedimentos e substituição de pendrives clonados sobressalentes em caso de falha de sistema, sem dependência da universidade.

---

### 3.3 Pitch Relâmpago de Bancada (Roteiro de 2 Minutos)
"Boa tarde. Nosso diagnóstico no Sol Nascente focou no que realmente estrangula a operação da creche: custos fixos de água e descarte eletrônico acumulado. Com orçamento estrito de R$ 250,00, integramos uma cisterna de captação de chuva com barril reaproveitado e sistema first-flush de descarte mecânico de sujeira, direcionando a água exclusivamente para descarga e limpeza das áreas comuns — atendendo com rigor as normas do ECA ao isolar fisicamente o acesso das crianças por cadeados e grades. Na bancada de TI, canibalizamos as peças sadias dos computadores queimados para subir 3 máquinas funcionais com Lubuntu leve em boot persistente via USB, carregando jogos educativos offline como o GCompris e fiação isolada a 1,60m de altura com proteção DR. A instituição ganha autonomia imediata através de um manual visual de 3 passos plastificado e pendrives de backup clonados, garantindo emancipação técnica soberana desde o primeiro mês. Obrigado."
