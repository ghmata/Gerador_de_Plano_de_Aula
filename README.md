# 📚 Planejador de Aulas BNCC Pro

> **SaaS EdTech** que utiliza Inteligência Artificial Generativa para criar planos de aula alinhados à legislação educacional brasileira.

![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![Python](https://img.shields.io/badge/Backend-Python%20%7C%20Flask-blue)
![AI](https://img.shields.io/badge/AI-Google%20Gemini-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 🎯 Sobre o Projeto

O **Planejador BNCC** resolve uma das maiores dores dos professores brasileiros: a burocracia do planejamento alinhado à BNCC (Base Nacional Comum Curricular).

A aplicação atua como um "Coordenador Pedagógico Virtual", recebendo o contexto da turma e gerando um documento completo com:
*   Códigos de Habilidades BNCC (ex: `EF15LP01`).
*   Metodologias Ativas (Rotação por estações, PBL, Sala invertida).
*   Adaptações curriculares para inclusão e diversidade.
*   Jogos e atividades lúdicas detalhadas.

## ✨ Funcionalidades Principais

*   **IA Contextualizada:** Prompt engineering avançado focado na educação brasileira.
*   **Compliance Legal:** Inserção automática de pautas sobre as Leis 10.639/03 (História Afro-Brasileira) e 11.645/08 (Indígena).
*   **Mobile-First:** Interface responsiva que funciona como App nativo no celular.
*   **Gamification Engine:** Módulo específico para criar Quizzes, Jogos de Tabuleiro ou Gartic baseados no conteúdo da aula.
*   **Exportação:** Gera o plano em HTML/PDF formatado para impressão ou envio à coordenação.

## 🛠️ Tecnologias Utilizadas

### Frontend (Client)
*   **HTML5 / CSS3 Moderno:** Design responsivo com variáveis CSS e tema escuro.
*   **JavaScript (ES6+):** Lógica de estado e manipulação de DOM sem frameworks pesados (Vanilla JS) para alta performance.
*   **Marked.js:** Renderização de Markdown para HTML em tempo real.

### Backend (Server)
*   **Python & Flask:** API RESTful para processamento seguro das requisições.
*   **Google Gemini API (1.5 Flash):** LLM responsável pela geração do conteúdo.
*   **PythonAnywhere:** Infraestrutura de hospedagem da API.

## 🚀 Como Rodar Localmente

### Pré-requisitos
*   Python 3.8+
*   Uma chave de API do Google AI Studio (Gemini).

### 1. Clone o repositório
```bash
git clone https://github.com/SEU-USUARIO/planejador-bncc.git
cd planejador-bncc
2. Configuração do Backend
code
Bash
cd backend
pip install -r requirements.txt
# Defina sua chave de API no arquivo .env ou direto no código (para dev)
python app.py
3. Configuração do Frontend
Abra o arquivo index.html e, caso esteja rodando localmente, aponte a variável API_URL para o seu localhost:
code
JavaScript
const API_URL = "http://127.0.0.1:5000/api/gerar";
🧠 Arquitetura da Solução
O projeto foi desenhado para escalar como um produto SaaS (Software as a Service):
Frontend: Coleta os dados pedagógicos.
API Gateway (Flask): Protege a chave da IA e aplica regras de negócio (validação de assinatura).
LLM: Processa o pedido com um System Prompt especializado.
Output: Retorna JSON estruturado que é renderizado no navegador.
🛣️ Roadmap & Monetização

MVP Funcional (Geração de Planos).

Integração com BNCC.

Sistema de Login/Cadastro (Auth).

Integração com Stripe/Mercado Pago.

Histórico de Planos salvos na nuvem (Supabase/PostgreSQL).
📄 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
Desenvolvido por [Gabriel Hipólito da Mata] 
