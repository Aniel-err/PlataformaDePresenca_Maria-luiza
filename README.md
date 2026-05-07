# 📓 Diário de Classe Digital Pro

> Sistema inteligente e automatizado para gestão de frequência escolar, desenvolvido para facilitar a rotina de professores com cliques rápidos e cálculos em tempo real.

---

## ✨ Funcionalidades Principais

* ✅ **Chamada Ultra-Rápida:** Clique esquerdo para `Presente/Falta` e clique direito para `Justificada/Limpar`.
* 📊 **Estatísticas em Tempo Real:** Calcula automaticamente o total de dias, faltas, presenças e a porcentagem de frequência de cada aluno.
* 📅 **Calendário Inteligente:** Identifica automaticamente finais de semana e feriados (nacionais e do Maranhão), bloqueando essas datas e ajustando os cálculos letivos.
* 🏷️ **Etiquetas Personalizadas (Tags):** Identifique alunos com necessidades especiais ou de outras turmas usando etiquetas coloridas (ex: "Parcial", "Sala E").
* 🔤 **Organização Automática:** Alunos organizados por ordem alfabética e numerados automaticamente.
* 💾 **Banco de Dados Local:** Não precisa de internet para funcionar; os dados ficam salvos de forma segura no seu computador.

---

## 🚀 Guia de Instalação (Para Professores)

Se você não é da área de tecnologia, não se preocupe! Siga estes 3 passos simples para colocar o sistema para funcionar:

### 1. Instale o "Motor" (Node.js)
O sistema precisa de um programa chamado **Node.js** para rodar. 
* Acesse: [https://nodejs.org/](https://nodejs.org/)
* Baixe a versão **LTS mais recente** (é a mais estável).
* Instale como qualquer outro programa (clicando em "Avançar" até o fim).

### 2. Prepare a Pasta
* Coloque os arquivos do Diário de Classe em uma pasta de sua preferência (ex: Documentos ou Área de Trabalho).

### 3. Inicie o Sistema
* Dentro da pasta onde estão os arquivos, procure por um arquivo chamado **`INICIAR.bat`** e dê um duplo clique para executá-lo.
* Uma tela preta aparecerá com a mensagem de inicialização do servidor. **Não feche essa tela enquanto estiver usando o sistema.**

### 4. Abra o Diário
* Agora, basta abrir o arquivo **`index.html`** no seu navegador (Chrome, Edge ou Firefox).
* Pronto! Você já pode cadastrar seus alunos e marcar as presenças.

---

## 🛠️ Instalação Técnica (Para Desenvolvedores/Estudantes)

Se você já conhece terminal, siga os comandos abaixo:

1. Clone o repositório ou baixe os arquivos.
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie o servidor:
   ```bash
   node server.js
   ```
4. Abra o `index.html` no navegador.

---

## 🖱️ Como Utilizar (Atalhos Rápidos)

Para tornar a chamada rápida, o sistema utiliza o mouse de forma inteligente:

* **Clique Esquerdo:** Alterna entre `P` (Presente) e `F` (Falta).
* **Clique Direito:** Alterna entre `J` (Justificada) e o estado vazio.
* **Botão ✎ ID:** Permite criar ou editar a etiqueta colorida ao lado do nome do aluno.
* **Destaques:** Use o painel superior para pintar dias de prova ou eventos importantes no calendário.

---

## 📅 Feriados Maranhenses Incluídos
O sistema já vem configurado para ignorar os feriados nacionais e o feriado estadual da **Adesão do Maranhão (28 de julho)**, garantindo que os dias letivos não sejam contabilizados erradamente nessas datas.

---

## 🎓 Créditos
Desenvolvido por **Aniel Nascimento** — *Estudante de Análise e Desenvolvimento de Sistemas*

---

### 💡 Dica Bônus: O arquivo `INICIAR.bat`

Para os professores que não sabem abrir o terminal, o arquivo de "atalho" já acompanha o projeto. Se ele for apagado por engano e você precisar recriar, use o modelo abaixo:

1.  Abra o Bloco de Notas.
2.  Cole o seguinte código:
    ```batch
    @echo off
    title Servidor do Diário de Classe
    echo Iniciando o sistema...
    node server.js
    pause
    ```
3.  Salve como **`INICIAR.bat`** dentro da mesma pasta onde está o seu `server.js`.
