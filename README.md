# Prospec — Gerador de Leads

App que roda **inteiramente no navegador** (sem instalar nada) para achar negócios locais no Google Maps e transformar em leads de venda de sites e apps.

**URL:** https://mirandahildebrando.github.io/prospec-leads/

## Como usar (3 passos)

1. **Abra o link**, digite a cidade (ex.: `Campinas, SP`), os **bairros** (ex.: `Cambuí, Barão Geraldo`) e marque os segmentos.
2. Clique em **Gerar leads**. O app lista os negórcios com nota, site e telefone, e **classifica automaticamente**:
   - 🔴 **QUENTE** — não tem site (ou só tem Instagram/site gratuito): seu melhor discurso.
   - 🟠 **MORNO** — tem site antigo ou sem HTTPS: candidato a redesign.
   - ⚪ **FRIO** — já tem site profissional: vender app/sistema.
3. Clique em **WhatsApp** (mensagem já personalizada com o nome do negócio) ou exporte a **planilha XLSX/CSV**.

## Leads "infinitos" e recorrentes

- A **memória** guarda todos os leads já vistos e a busca seguinte **nunca repete** — cada rodada traz negócios novos.
- O campo **Bairros** multiplica a varredura: cada bairro gera buscas separadas, cobrindo a cidade inteira aos poucos.
- Troque os segmentos, os bairros ou a cidade e rode de novo — sempre sai lead novo.

## Configurando a chave do Google (recomendado, ~10 min, grátis)

Sem a chave o app funciona com o OpenStreetMap (dados limitados — muitos negócios sem telefone/site).
Com a chave, você recebe **telefone, site e nota** de tudo: 5.000 buscas grátis por mês.

1. Abra [console.cloud.google.com](https://console.cloud.google.com/) e crie um projeto.
2. Busque **Places API (New)** e clique em **Ativar**.
3. **Credenciais → Criar credencial → Chave de API** e copie.
4. O Google pede conta de faturamento, mas **dentro do grátis você não paga nada**. Crie um alerta de orçamento para se avisar se algo sair do controle.
5. No app, clique em **Configurar**, cole a chave e salve.

## Boas práticas

- Identifique-se nas abordagens e respeite a recusa do contato (LGPD).
- O app usa apenas **APIs oficiais** (Google Places e OpenStreetMap) — não faz scraping.
- A chave fica salva só no seu navegador; a página não envia seus dados para nenhum servidor próprio.
