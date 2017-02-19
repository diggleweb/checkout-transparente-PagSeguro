## Checkout Transparente PagSeguro ##

Exemplo de CheckoutTransparente do PagSeguro feito em PHP.

Este projeto foi desenvolvido para sanar necessidades específicas do [Portal infoEnem](http://www.infoenem.com.br/), tenha em mente que sua implementação não é trivial e este arquivo não dispensa um contato técnico para efetuar a instalação, configuração e personalização conforme as próprias necessidades.

![Checkout Transparente PagSeguro em PHP](https://raw.githubusercontent.com/lubuzzo/Checkout-Transparente-PagSeguro/master/screenshot.png "Checkout Transparente PagSeguro em PHP")

### Projeto efetua: ###
 - Transação inteiramente em Checkout Transparente;
 - Fácil mudança entre os ambientes do PagSeguro (sandbox/produção);
 - Responsivo usando o [Bootstrap](http://getbootstrap.com) (versão 3.3.7, via Content Delivery Network do [MaxCDN](https://www.maxcdn.com/))
 - Pesquisa de cep no [República Virtual](http://www.republicavirtual.com.br/) para rápido preenchimento de campos;
 - Campos com máscara de entrada (CPF, CEP, Data de Nascimento) para melhor visualização;
 - Segundo nova exigência de informar ao cliente o país no qual a transação está sendo processada;
 - Em casos de erros, retornados pelo PagSeguro, é exibido um modal e o campo com erro recebe destaque;
 - Quando Dados do Comprador são os mesmos do Titular do Cartão de Crédito, ocorre preenchimento automático;
 - Pega informações de parcelamento disponíveis pelo PagSeguro, para o valor da transação.
 - Em caso de pagamento com boleto, a pessoa será redirecionada para o boleto ao final da transação;

### Projeto não efetua: ###
 - Venda de mais que um produto;
 - Pagamento via eft (transferência eletrônica);

### Como utilizar: ###
 1. Executar um git clone no repositório: *git clone https://github.com/lubuzzo/Checkout-Transparente-PagSeguro.git*;
 2. Renomei o arquivo **env-example.php** para **env.php**;
 3. Altere os valores dentro do arquivo, renomeado no passo anterior, para os dados próprios (e-mail e token - obtido em https://pagseguro.uol.com.br/preferencias/integracoes.jhtml);
 4. Altere o **favicon.ico** conforme o seu;
 5. Dentro da pasta images, altere o arquivo **logo.png** para o seu.