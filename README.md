# 📋 To-Do List

Neste projeto foi criada um aplicativo web de lista de tarefas usando HTML, CSS e JavaScript. A aplicação permite adicionar, marcar como concluída ou pendente, e excluir tarefas. Foi usado o armazenamento local em JavaScript para persistir a lista de tarefas no navegador, proporcionando uma experiência contínua mesmo após reinicialização.

O código JavaScript manipula dinamicamente a DOM, permitindo a adição de tarefas com um simples clique no botão 'Adicionar' e a marcação do status de conclusão ao clicar na tarefa. Implementamos um ícone de fechamento para exclusão eficiente de tarefas específicas. O uso de armazenamento local assegura a persistência dos dados, mantendo a lista de tarefas intacta entre sessões.

## Tecnologias Utilizadas

- HTML
- CSS
- JavaScript

## Como Usar

1. Abra o arquivo `index.html` em um navegador da web.
2. Você verá uma caixa de entrada para adicionar suas tarefas e um botão "Add" para incluir uma nova tarefa na lista.
3. Cada item na lista pode ser marcado como concluído clicando nele. Clique novamente para desmarcar.
4. Cada item também possui um botão "X" à direita para removê-lo da lista.

## Pré-requisitos

Não há pré-requisitos específicos para executar este projeto. Apenas abra o arquivo HTML em um navegador da web compatível.

## Capturas de Tela

![image]()

## 🚀 Futuras atualizações

Pretendo ajustar o layout para outros dispositivos, principalmente mobile com Flutter ou outra linguagem

## Personalização

Sinta-se à vontade para modificar o estilo da aplicação ajustando o arquivo `style.css` ou expandir a lógica de funcionalidade em `script.js` conforme necessário.

## Códigos Relevantes

### Adição de Tarefa (script.js)

```javascript
function addTask() {
    if (inputBox.value === '') {
        alert("Você deve escrever alguma coisa!");
    } else {
        let li = document.createElement("li");
        li.innerHTML = inputBox.value;
        listContainer.appendChild(li);
        let span = document.createElement("span");
        span.innerHTML = "\u00d7";
        li.appendChild(span);
    }
    inputBox.value = "";
    saveData();
}
```

## Licença

Este aplicativo é distribuído sob a [Licença MIT](LICENSE).

Este projeto foi criado como parte de um desafio de programação.
