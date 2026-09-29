# Desafio DevSecOps — Gerenciador de Tarefas

## Sobre o Projeto
Este repositório faz parte do desafio prático do módulo de DevSecOps da ADA Tech.
Você receberá este projeto com vulnerabilidades propositais e uma pipeline incompleta.
Seu objetivo é **implementar a pipeline de segurança** e **corrigir as vulnerabilidades**.

## Estado atual
A pipeline está **incompleta**. Os steps de segurança precisam ser implementados por você.

## Sua missão
1. Implementar os steps de segurança no `pipeline.yml`
2. Fazer a pipeline **quebrar** ao detectar os problemas
3. Corrigir as vulnerabilidades encontradas
4. Fazer a pipeline **passar** com tudo verde ✅
5. Documentar o funcionamento da pipeline neste README

## O que implementar
- [ ] Secrets Scanning com **Gitleaks**
- [ ] SAST com **Semgrep**
- [ ] SCA com **Grype**
- [ ] Deploy com **GitHub Pages**

## Como a pipeline funciona
Nossa esteira de segurança funciona como uma **porta automática**: se encontrar qualquer falha, ela paralisa o processo e impede que o site vá ao ar. A cada etapa, o código é verificado e os erros são apontados para correção. A publicação só é liberada quando o sistema passa por todos os testes com sucesso.

1. Checkout do Código: Baixa os arquivos do projeto para o ambiente de testes.
2. Setup do Ambiente: Prepara o sistema e instala as ferramentas necessárias.
3. Secrets Scanning (Gitleaks): Procura senhas ou chaves salvas por engano no código.
4. SAST (Semgrep): Analisa o código em busca de brechas e erros de programação.
5. SCA (Grype): Verifica se os pacotes e bibliotecas de terceiros possuem vulnerabilidades conhecidas.
6. Build e Deploy (GitHub Pages): Publica o site na internet (só executa se todos os testes anteriores passarem).

## URL de Produção
https://kellersimara-eng.github.io/projeto-devsecop-desafio/
