# ⚖️ JAIA — Legal AI Assistant (Estudo de Caso)

## 🎯 Problema
O escritório precisava revisar e padronizar peças jurídicas de forma rápida e consistente.  
A revisão manual tomava tempo e criava divergências de estilo entre advogados.

---

## 💡 Solução
Criei, junto à equipe da Tavros Tech, o **JAIA — Juridical AI Assistant**,  
um sistema multiagente que utiliza **LLMs (Gemini)** e **RAG** com **PostgreSQL + pgvector**  
para corrigir, padronizar e gerar automaticamente documentos jurídicos em `.docx`.

Principais ideias da arquitetura:
- Um **agente administrador** identifica o tipo de documento (ex: petição inicial, contrarrazões etc.)
- Envia para **agentes especializados** com prompts específicos por tipo.
- O backend salva cada versão corrigida com histórico e logs de tokens.
- O frontend permite upload, chat e download do `.docx` final com marcações.

---

## 🧩 Stack Técnica
| Camada | Tecnologias |
|---------|--------------|
| **Backend** | Python, Django, FastAPI |
| **IA / LLM** | Gemini, LangChain, pgvector |
| **Banco** | PostgreSQL |
| **Frontend** | React + TypeScript |
| **Infraestrutura** | AWS EC2, S3, Docker, Nginx |
| **Documentos** | python-docx, regex, Pandoc |

---

## 🔧 Papel Pessoal
- Defini a **arquitetura multiagente** e os fluxos de correção.  
- Modelei o banco vetorial e a integração RAG.  
- Desenvolvi o gerador `.docx` com marcações jurídicas automáticas.  
- Implementei controle de tokens e logs detalhados por requisição.  
- Fiz deploy e manutenção em ambiente AWS.

---

## 📈 Resultados
- Redução expressiva no tempo de revisão documental.  
- Padrão de escrita jurídica unificado conforme o estilo **JASA**.  
- Processos auditáveis e escaláveis para múltiplos tipos de peça.

---

> 🔒 Código privado por confidencialidade institucional.  
> Este estudo descreve apenas **arquitetura, impacto e decisões técnicas.**
