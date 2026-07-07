WhatsApp Ofertas Bot — Radar Tech
Manual Completo de Configuração, Instalação e Execução (Linux & Windows)


Descrição do Projeto

Este documento detalha o processo passo a passo para configurar o ambiente virtual e executar de forma
isolada e segura o robô de automação de envios de ofertas para grupos do whatsapp. O script utiliza Selenium e Schedule para
gerenciar disparos programados de ofertas do Mercado Livre estruturadas em formato JSON diretamente
para o WhatsApp Web.


Vantagem do Ambiente Isolado (.venv): A utilização do ambiente virtual evita o erro de ambiente
gerenciado externamente (PEP 668) no Linux e garante que todas as dependências corretas (Selenium,
Schedule, etc.) fiquem restritas à pasta do projeto, mantendo seu sistema operacional limpo e seguro.

Guia de Execução no Linux (Ubuntu / Debian / Termux)


Abra o seu terminal, copie e cole os comandos abaixo em sequência:

1. Acessar a pasta raiz do projeto
cd "/home/lucas/Área de trabalho/Projetos/whatsappbotoffers"

2. Criar o ambiente virtual isolado
python3 -m venv .venv

3. Ativar o ambiente virtual
source .venv/bin/activate

4. Instalar as dependências necessárias

pip install requests schedule selenium webdriver-manager

5. Iniciar o bot

  python3 whatsapp_ofertas.py


POR ULTIMO!

De onde veio esse json? a partir de um sistema que faz o scrapper automatico de ofertas do mercado livre disponível no repositório radar-tech!!!