## 📋 Sobre o Projeto

Este projeto foi desenvolvido a partir de um site simples criado por uma familiar como teste para uma loja de uniformes. O objetivo do site era simular a venda de camisetas, permitindo que o usuário selecionasse tamanho e quantidade, adicionasse ao carrinho temporário e finalizasse o pedido via WhatsApp.

A aplicação foi construída em **HTML puro** com alguns arquivos em **JavaScript**, sem integração com banco de dados, meios de pagamento ou persistência de carrinho. O carrinho é apenas temporário e o fluxo de compra redireciona diretamente para o WhatsApp com as informações do pedido.

Aproveitei essa oportunidade para:

- Praticar análise de requisitos  
- Elaborar casos de teste manuais  
- Criar cenários BDD  
- Validar fluxo de compra  
- Testar regras de seleção de tamanho e quantidade  
- Identificar possíveis melhorias  


<table>
  <tr>
   <td>N
   </td>
   <td>1
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Validação de quantidades inválidas no carrinho de compras
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Menu inicial > Loja > Ver detalhes > selecionar tamanho > quantidade "<strong>48489748</strong>” ou "2.5” > adicionar ao carrinho
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário insira a quantidade inválida no carrinho com números grandes e valores decimais.
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>❌O sistema aceita a quantidade e adiciona no carrinho.
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>❌Apresentar valor máximo permitido, não permitir números absurdamente altos, mensagem de erro.
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>Adicionar mínimo e máximo.
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>


<img src="evidence_images/image1.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>2
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Validação de quantidades válidas no carrinho de compras
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Menu inicial > Loja > Ver detalhes > selecionar tamanho > quantidade "<strong>01</strong>” > adicionar ao carrinho
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário insira uma quantidade válida no carrinho “<strong>01".</strong>
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>✅A quantidade é inserida no carrinho com sucesso
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>✅A quantidade é inserida no carrinho com sucesso
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>



<img src="evidence_images/image2.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>3
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Validação de tamanhos
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Menu inicial > Loja > Ver detalhes > selecionar tamanho > adicionar ao carrinho
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário escolha um tamanho e adicione o item no carrinho  
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>✅O tamanho escolhido aparece corretamente no carrinho
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>✅O tamanho escolhido aparece corretamente no carrinho
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>

<img src="evidence_images/image3.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>4
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Tentativa de adicionar ao carrinho sem selecionar tamanho
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Menu inicial > Loja > Ver detalhes > nao selecionar tamanho > adicionar ao carrinho
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário não selecione um tamanho e adicione o item no carrinho  
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>✅Mensagem de erro "Selecione o tamanho”
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>✅Mensagem de erro "Selecione o tamanho”
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>



<img src="evidence_images/image4.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>5
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Adicionar ao carrinho e atualizar a página
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Menu inicial > Loja > Ver detalhes > selecionar tamanho > quantidade > adicionar ao carrinho > atualizar página
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário esteja com itens no carrinho e atualize a página
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>❌O usuário perde o que havia adicionado no carrinho e reinicia a página
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>❌A página é atualizada e os itens permanecem no carrinho
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>


<img src="evidence_images/image5.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>6
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Finalização > Redirecionamento WhatsApp
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Loja > Ver detalhes > selecionar tamanho > quantidade > adicionar ao carrinho > ver sacola/finalizar >Solicitar orçamento no whatsapp
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário finalize a compra e solicite o pedido pelo whatsapp
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>❌O usuário é redirecionado ao whatsapp com a solicitação do pedido
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>❌O usuário é redirecionado ao whatsapp com a solicitação do pedido
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>



<img src="evidence_images/image6.png" width="" alt="alt_text" title="image_tooltip">



<img src="evidence_images/image7.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>



<table>
  <tr>
   <td>N
   </td>
   <td>7
   </td>
  </tr>
  <tr>
   <td>Cenário
   </td>
   <td>Verificar Layout por outros dispositivos (mobile)
   </td>
  </tr>
  <tr>
   <td>Passos
   </td>
   <td>Página inicial
   </td>
  </tr>
  <tr>
   <td>Dado
   </td>
   <td>Que o usuário utilize outros dispositivos para acessar o site
   </td>
  </tr>
  <tr>
   <td>Resultado Obtido
   </td>
   <td>❌Os tamanhos não ficam responsivos 
   </td>
  </tr>
  <tr>
   <td>Resultado Esperado
   </td>
   <td>❌Conseguir navegar sem que o layout fique desorganizado
   </td>
  </tr>
  <tr>
   <td>Observação
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>Evidências
   </td>
   <td>



<img src="evidence_images/image8.png" width="" alt="alt_text" title="image_tooltip">




<img src="evidence_images/image9.png" width="" alt="alt_text" title="image_tooltip">




<img src="evidence_images/image10.png" width="" alt="alt_text" title="image_tooltip">

   </td>
  </tr>
</table>
