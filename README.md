PORTUGUÊS

# Redirecionamento Dinâmico de Elementos

Este repositório contém dois scripts JavaScript que visam realizar redirecionamentos dinâmicos de elementos em páginas web. Os scripts foram criados para interceptar eventos gerados dinamicamente por meio do consumo de uma API e aplicar redirecionamentos personalizados a esses eventos. A seguir, detalhamos o funcionamento de cada script:

## Script 1

### Descrição

O primeiro script é destinado a páginas que contêm elementos com IDs específicos, como `1186440` e `1186443`. Ele cria um evento de clique personalizado para cada elemento e redireciona o usuário para URLs específicas ao clicar nesses elementos.

### Funcionamento

1. O script aguarda até que o DOM esteja completamente carregado usando o evento `DOMContentLoaded`.
2. A função `checkElementsAndExecute()` é chamada, que procura por elementos com os IDs `1186440` e `1186443`.
3. Se ambos os elementos forem encontrados, eventos de clique são adicionados a esses elementos que redirecionam o usuário para URLs específicas.
4. Caso os elementos não sejam encontrados imediatamente, o script aguarda 100ms e tenta novamente, até que os elementos sejam encontrados.

## Script 2

### Descrição

O segundo script destina-se a páginas que contenham uma lista de cartões de categoria com a classe `.coursesCategoriesCard`. Ele verifica o conteúdo de cada cartão e, com base nas informações de texto, personaliza os redirecionamentos dos links contidos nos cartões.

### Funcionamento

1. Assim como o primeiro script, o segundo também aguarda o carregamento completo do DOM usando o evento `DOMContentLoaded`.
2. A função `checkElementsAndExecute()` é chamada, que seleciona todos os elementos com a classe `.coursesCategoriesCard` e itera sobre eles.
3. Para cada cartão, o script verifica se o texto contido no cartão inclui "Plano Básico" ou "Plano Especial".
4. Se "Plano Básico" for encontrado, o script obtém o link contido no cartão e redefine seu atributo `href` para uma URL específica.
5. Se "Plano Especial" for encontrado, o mesmo processo é aplicado para redirecionar o link para outra URL.
6. Se nenhum dos textos for encontrado nos cartões imediatamente, o script aguarda 100ms e tenta novamente, até que os elementos sejam encontrados.

## Considerações Finais

Ambos os scripts têm o objetivo de manipular eventos gerados dinamicamente, adicionando redirecionamentos personalizados aos elementos correspondentes. Certifique-se de incluir esses scripts em suas páginas da web de acordo com as condições descritas para garantir que os redirecionamentos sejam aplicados corretamente.

Se tiver alguma dúvida ou quiser contribuir para aprimorar esses scripts, sinta-se à vontade para abrir uma issue ou pull request neste repositório.

<hr>
ENGLISH

# Dynamic Element Redirection

This repository contains two JavaScript scripts aimed at dynamically redirecting elements on web pages. The scripts were created to intercept events dynamically generated through API consumption and apply custom redirections to these events. Below, we detail the functionality of each script:

## Script 1

### Description

The first script is intended for pages containing elements with specific IDs, such as `1186440` and `1186443`. It creates a custom click event for each element and redirects the user to specific URLs upon clicking these elements.

### Functionality

1. The script waits until the DOM is fully loaded using the `DOMContentLoaded` event.
2. The `checkElementsAndExecute()` function is called, which searches for elements with the IDs `1186440` and `1186443`.
3. If both elements are found, click events are added to these elements that redirect the user to specific URLs.
4. If the elements are not immediately found, the script waits for 100ms and retries until the elements are found.

## Script 2

### Description

The second script is intended for pages containing a list of category cards with the class `.coursesCategoriesCard`. It checks the content of each card and, based on the text information, customizes the redirection of the links contained within the cards.

### Functionality

1. Similar to the first script, the second one also waits for the complete DOM loading using the `DOMContentLoaded` event.
2. The `checkElementsAndExecute()` function is called, which selects all elements with the class `.coursesCategoriesCard` and iterates through them.
3. For each card, the script checks whether the text within the card includes "Basic Plan" or "Special Plan".
4. If "Basic Plan" is found, the script retrieves the link inside the card and resets its `href` attribute to a specific URL.
5. If "Special Plan" is found, the same process is applied to redirect the link to another URL.
6. If neither of the texts is immediately found in the cards, the script waits for 100ms and retries until the elements are found.

## Final Remarks

Both scripts aim to handle dynamically generated events by adding custom redirections to the corresponding elements. Make sure to include these scripts on your web pages according to the described conditions to ensure that the redirections are applied correctly.

If you have any questions or wish to contribute to improving these scripts, feel free to open an issue or pull request in this repository.
