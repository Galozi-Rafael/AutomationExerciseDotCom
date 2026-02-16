# AutomationExerciseDotCom
Automatizar o site playground de e-commerce: https://automationexercise.com/

## Checklist — Automation Exercise

- [x] Test Case 1: Register User
- [x] Test Case 2: Login User with correct email and password
- [x] Test Case 3: Login User with incorrect email and password
- [x] Test Case 4: Logout User
- [x] Test Case 5: Register User with existing email
- [x] Test Case 6: Contact Us Form
- [x] Test Case 7: Verify Test Cases Page
- [x] Test Case 8: Verify All Products and product detail page
- [x] Test Case 9: Search Product
- [x] Test Case 10: Verify Subscription in home page
- [x] Test Case 11: Verify Subscription in Cart page
- [x] Test Case 12: Add Products in Cart
- [x] Test Case 13: Verify Product quantity in Cart
- [x] Test Case 14: Place Order — Register while Checkout
- [x] Test Case 15: Place Order — Register before Checkout
- [x] Test Case 16: Place Order — Login before Checkout
- [x] Test Case 17: Remove Products From Cart
- [x] Test Case 18: View Category Products
- [x] Test Case 19: View & Cart Brand Products
- [x] Test Case 20: Search Products and Verify Cart After Login
- [x] Test Case 21: Add review on product
- [x] Test Case 22: Add to cart from Recommended items
- [x] Test Case 23: Verify address details in checkout page
- [ ] Test Case 24: Download Invoice after purchase order
- [x] Test Case 25: Verify Scroll Up using 'Arrow' button and Scroll Down functionality
- [x] Test Case 26: Verify Scroll Up without 'Arrow' button and Scroll Down functionality

## Casos de test

### Test Case 01 — Register User

Este cenário valida o fluxo completo de cadastro de um novo usuário, incluindo login automático e exclusão da conta ao final do processo.

#### Objectivo

Validar o processo de **registro, autenticação e exclusão de usuário** no site Automation Exercise.

#### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Verificar se **"New User Signup!"** está visível  
6. Informar **Nome** e **Endereço de E-mail**  
7. Clicar no botão **Signup**  
8. Verificar se **"ENTER ACCOUNT INFORMATION"** está visível  
9. Preencher os dados da conta:
   - Título  
   - Nome  
   - E-mail  
   - Senha  
   - Data de Nascimento  
10. Marcar a caixa **"Sign up for our newsletter!"**  
11. Marcar a caixa **"Receive special offers from our partners!"**  
12. Preencher os dados de endereço:
    - Primeiro Nome  
    - Sobrenome  
    - Empresa  
    - Endereço  
    - Endereço 2  
    - País  
    - Estado  
    - Cidade  
    - CEP  
    - Número de Celular  
13. Clicar no botão **Create Account**  
14. Verificar se **"ACCOUNT CREATED!"** está visível  
15. Clicar no botão **Continue**  
16. Verificar se **"Logged in as _username_"** está visível  
17. Clicar no botão **Delete Account**  
18. Verificar se **"ACCOUNT DELETED!"** está visível e clicar em **Continue**

#### Resultado Esperado

- A conta do usuário é criada com sucesso  
- O usuário é autenticado automaticamente após o cadastro  
- A conta do usuário é excluída com sucesso  
- Todas as mensagens de confirmação são exibidas conforme esperado  


## Test Case 02 — Login User with Correct Credentials

Este cenário valida o fluxo completo de autenticação de um usuário já cadastrado no sistema, garantindo que o login ocorra com sucesso quando credenciais válidas são informadas. Ao final do processo, a conta é excluída para manter o ambiente limpo para execuções futuras.

### Objectivo

Validar o processo de **autenticação de usuário com credenciais válidas**, incluindo:

- Acesso à página de login  
- Inserção correta de e-mail e senha  
- Confirmação de login bem-sucedido  
- Exclusão da conta após autenticação  

### Pré-condição

- O usuário já deve estar previamente cadastrado no sistema  
- O e-mail e a senha utilizados devem ser válidos  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Verificar se o texto **"Login to your account"** está visível  
6. Informar **Endereço de E-mail válido** no campo de e-mail  
7. Informar **Senha correta** no campo de senha  
8. Clicar no botão **Login**  
9. Verificar se o texto **"Logged in as _username_"** está visível no topo da página  
10. Confirmar que o botão **Logout** está disponível  
11. Clicar no botão **Delete Account**  
12. Verificar se a mensagem **"ACCOUNT DELETED!"** está visível  
13. Clicar no botão **Continue**

### Resultado Esperado

- O usuário é autenticado com sucesso  
- O sistema exibe corretamente a mensagem **"Logged in as _username_"**  
- O botão **Logout** fica disponível após login  
- A conta é excluída com sucesso  
- A mensagem **"ACCOUNT DELETED!"** é exibida corretamente  
- O sistema redireciona para a página inicial após clicar em **Continue**


## Test Case 03 — Login User with Incorrect Credentials

Este cenário valida o comportamento do sistema quando um usuário tenta se autenticar usando credenciais inválidas. O objetivo é garantir que o login seja negado e que a mensagem de erro apropriada seja exibida.

### Objectivo

Validar o processo de **login com credenciais incorretas**, garantindo:

- Acesso à página de login  
- Tentativa de login com e-mail e/ou senha inválidos  
- Bloqueio da autenticação  
- Exibição da mensagem de erro correta  

### Pré-condição

- O usuário deve acessar a área de login do site  
- Pode existir (ou não) uma conta cadastrada, mas as credenciais informadas devem ser **inválidas** (e-mail incorreto, senha incorreta, ou ambos)

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Verificar se o texto **"Login to your account"** está visível  
6. Informar um **Endereço de E-mail inválido** no campo de e-mail  
7. Informar uma **Senha incorreta** no campo de senha  
8. Clicar no botão **Login**  
9. Verificar se a mensagem **"Your email or password is incorrect!"** está visível  

### Resultado Esperado

- O login **não** é realizado  
- O usuário permanece na área de login (sem autenticação)  
- A mensagem **"Your email or password is incorrect!"** é exibida corretamente  
- O sistema não apresenta a identificação **"Logged in as _username_"**  


## Test Case 04 — Logout User

Este cenário valida o processo completo de logout de um usuário autenticado, garantindo que a sessão seja encerrada corretamente e que o sistema redirecione o usuário para a página de login.

### Objectivo

Validar o processo de **logout do usuário autenticado**, garantindo:

- Existência de sessão ativa  
- Encerramento correto da sessão  
- Redirecionamento para a página de login  
- Remoção da identificação do usuário logado  

### Pré-condição

- O usuário deve estar previamente cadastrado  
- O usuário deve estar autenticado no sistema (login realizado com sucesso)  
- A identificação **"Logged in as _username_"** deve estar visível  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Informar **E-mail válido** e **Senha correta**  
6. Clicar no botão **Login**  
7. Verificar se o texto **"Logged in as _username_"** está visível  
8. Confirmar que o botão **Logout** está disponível  
9. Clicar no botão **Logout**  
10. Verificar se o sistema redireciona para a página de login  
11. Confirmar que o texto **"Login to your account"** está visível  
12. Confirmar que o texto **"Logged in as _username_"** não está mais visível  

### Resultado Esperado

- A sessão do usuário é encerrada com sucesso  
- O sistema redireciona para a página de login  
- A identificação do usuário logado deixa de ser exibida  
- O botão **Logout** não está mais disponível  
- O usuário não possui mais acesso autenticado  


## Test Case 05 — Register User with Existing Email

Este cenário valida o comportamento do sistema ao tentar registrar um novo usuário utilizando um endereço de e-mail que já está cadastrado na base de dados. 
O sistema deve impedir o cadastro duplicado e exibir a mensagem de erro apropriada.

### Objectivo

Validar a tentativa de **registro com e-mail já existente**, garantindo:

- Acesso correto à área de cadastro  
- Tentativa de registro com e-mail previamente cadastrado  
- Bloqueio do cadastro duplicado  
- Exibição da mensagem de erro apropriada  

### Pré-condição

- Deve existir uma conta previamente cadastrada no sistema  
- O e-mail utilizado no teste deve já estar registrado  
- O usuário deve estar na página inicial do site  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Verificar se o texto **"New User Signup!"** está visível  
6. Informar um **Nome válido** no campo de nome  
7. Informar um **Endereço de E-mail já cadastrado** no campo de e-mail  
8. Clicar no botão **Signup**  
9. Verificar se a mensagem **"Email Address already exist!"** está visível  
10. Confirmar que o sistema não redireciona para a tela de criação de conta  

### Resultado Esperado

- O cadastro não é realizado  
- O sistema impede duplicidade de e-mail  
- A mensagem **"Email Address already exist!"** é exibida corretamente  
- O usuário permanece na tela de cadastro  
- Nenhuma nova conta é criada  



## Test Case 06 — Contact Us Form

Este cenário valida o envio completo do formulário de contato, incluindo o preenchimento dos campos obrigatórios, upload de arquivo, confirmação do alerta e retorno à página inicial após envio bem-sucedido.

### Objectivo

Validar o funcionamento do **formulário de contato**, garantindo:

- Acesso correto à página de contato  
- Preenchimento dos campos obrigatórios  
- Upload de arquivo  
- Confirmação do alerta do navegador  
- Exibição da mensagem de sucesso  
- Retorno seguro à página inicial  

### Pré-condição

- O usuário deve estar na página inicial do site  
- O navegador deve permitir manipulação de alertas  
- Um arquivo válido deve estar disponível para upload  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Contact Us** no menu superior  
5. Verificar se o texto **"GET IN TOUCH"** está visível  
6. Informar **Nome válido** no campo Name  
7. Informar **E-mail válido** no campo Email  
8. Informar **Assunto válido** no campo Subject  
9. Informar uma **Mensagem válida** no campo Message  
10. Realizar upload de um arquivo no campo de upload  
11. Clicar no botão **Submit**  
12. Confirmar o alerta exibido pelo navegador (clicar em OK)  
13. Verificar se a mensagem **"Success! Your details have been submitted successfully."** está visível  
14. Clicar no botão **Home**  
15. Verificar se o sistema redireciona corretamente para a Página Inicial  

### Resultado Esperado

- O formulário é enviado com sucesso  
- O alerta é exibido e confirmado corretamente  
- A mensagem de sucesso é exibida  
- O botão **Home** redireciona corretamente para a página inicial  
- Nenhum erro é apresentado durante o processo  


## Test Case 07 — Verify Test Cases Page

Este cenário valida o acesso à página que lista todos os casos de teste disponíveis no site. 
O objetivo é garantir que o link de navegação funcione corretamente e que o conteúdo da página seja carregado sem erros.

### Objectivo

Validar o acesso à **página de Test Cases**, garantindo:

- Funcionamento correto do link de navegação  
- Redirecionamento adequado para a página de Test Cases  
- Carregamento completo do conteúdo da página  
- Exibição da lista de casos de teste  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- O menu superior deve estar visível e funcional  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Localizar o menu superior  
5. Clicar no botão **Test Cases**  
6. Verificar se o sistema redireciona para a página de casos de teste  
7. Confirmar que o título da página **"Test Cases"** está visível  
8. Verificar se a lista de casos de teste está exibida corretamente  
9. Confirmar que não há mensagens de erro na página  

### Resultado Esperado

- O clique no menu **Test Cases** redireciona corretamente  
- A página de Test Cases é carregada com sucesso  
- O título **"Test Cases"** está visível  
- A lista completa de casos de teste é exibida  
- Nenhum erro é apresentado durante o carregamento  


## Test Case 08 — Verify All Products and Product Detail Page

Este cenário valida o acesso à página de listagem de produtos e a navegação para a página de detalhes de um produto específico. 
O objetivo é garantir que os produtos sejam exibidos corretamente e que suas informações detalhadas estejam disponíveis.

### Objectivo

Validar a funcionalidade da **página de produtos e página de detalhes do produto**, garantindo:

- Acesso correto à listagem de produtos  
- Exibição completa da lista de produtos  
- Navegação para a página de detalhes de um produto  
- Exibição correta das informações detalhadas do produto  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- O menu superior deve estar funcional  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products** no menu superior  
5. Verificar se o sistema redireciona para a página **All Products**  
6. Confirmar que a lista de produtos está visível  
7. Selecionar um produto da lista  
8. Clicar no botão **View Product** correspondente  
9. Verificar se o sistema redireciona para a página de detalhes do produto  
10. Confirmar que as seguintes informações estão visíveis:
    - Nome do produto  
    - Categoria  
    - Preço  
    - Disponibilidade  
    - Condição  
    - Marca  
11. Confirmar que não há erros no carregamento da página  

### Resultado Esperado

- A página **All Products** é carregada corretamente  
- A lista de produtos é exibida com sucesso  
- O botão **View Product** redireciona corretamente  
- A página de detalhes exibe todas as informações do produto  
- Nenhum erro é apresentado durante o processo  



## Test Case 09 — Search Product

Este cenário valida a funcionalidade de busca de produtos na página de listagem. 
O objetivo é garantir que o sistema retorne corretamente os produtos correspondentes ao termo pesquisado.

### Objectivo

Validar a funcionalidade de **pesquisa de produtos**, garantindo:

- Acesso correto à página de produtos  
- Inserção de termo de busca válido  
- Execução da pesquisa  
- Exibição apenas dos produtos correspondentes  
- Exibição da seção de resultados pesquisados  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página **Products** deve estar acessível  
- Deve existir pelo menos um produto correspondente ao termo pesquisado  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products** no menu superior  
5. Verificar se o sistema redireciona para a página **All Products**  
6. Localizar o campo de busca de produtos  
7. Informar um **nome de produto válido** no campo de pesquisa  
8. Clicar no botão **Search**  
9. Verificar se a seção **"SEARCHED PRODUCTS"** está visível  
10. Confirmar que os produtos exibidos correspondem ao termo pesquisado  
11. Confirmar que nenhum produto fora do critério de busca é exibido  

### Resultado Esperado

- A pesquisa é executada com sucesso  
- A seção **"SEARCHED PRODUCTS"** é exibida  
- Apenas produtos relacionados ao termo pesquisado são apresentados  
- Nenhum erro é exibido durante a pesquisa  



## Test Case 10 — Verify Subscription in Home Page

Este cenário valida a funcionalidade de inscrição por e-mail (newsletter) disponível no rodapé da Página Inicial. 
O objetivo é garantir que o sistema aceite um e-mail válido e exiba a mensagem de confirmação corretamente.

### Objectivo

Validar o funcionamento da **inscrição de e-mail na Página Inicial**, garantindo:

- Presença da seção de Subscription no rodapé  
- Inserção de e-mail válido  
- Submissão correta da inscrição  
- Exibição da mensagem de sucesso  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- O rodapé da página deve estar visível  
- Um endereço de e-mail válido deve estar disponível para teste  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Rolar a página até o rodapé  
5. Verificar se a seção **"SUBSCRIPTION"** está visível  
6. Informar um **Endereço de E-mail válido** no campo de inscrição  
7. Clicar no botão de inscrição (ícone de seta ou botão Subscribe)  
8. Verificar se a mensagem **"You have been successfully subscribed!"** está visível  
9. Confirmar que nenhuma mensagem de erro é exibida  

### Resultado Esperado

- A seção **"SUBSCRIPTION"** está visível no rodapé  
- O e-mail é aceito pelo sistema  
- A mensagem **"You have been successfully subscribed!"** é exibida corretamente  
- Nenhum erro ocorre durante o processo  



## Test Case 11 — Verify Subscription in Cart Page

Este cenário valida a funcionalidade de inscrição por e-mail (newsletter) disponível no rodapé da página do carrinho de compras. 
O objetivo é garantir que o sistema aceite um e-mail válido e exiba corretamente a mensagem de confirmação.

### Objectivo

Validar o funcionamento da **inscrição de e-mail na página do Carrinho**, garantindo:

- Presença da seção de Subscription no rodapé da página Cart  
- Inserção de e-mail válido  
- Submissão correta da inscrição  
- Exibição da mensagem de sucesso  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página **Cart** deve estar acessível  
- Um endereço de e-mail válido deve estar disponível para teste  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Cart** no menu superior  
5. Verificar se o sistema redireciona para a página do carrinho  
6. Rolar a página até o rodapé  
7. Verificar se a seção **"SUBSCRIPTION"** está visível  
8. Informar um **Endereço de E-mail válido** no campo de inscrição  
9. Clicar no botão de inscrição (ícone de seta ou botão Subscribe)  
10. Verificar se a mensagem **"You have been successfully subscribed!"** está visível  
11. Confirmar que nenhuma mensagem de erro é exibida  

### Resultado Esperado

- A página **Cart** é carregada corretamente  
- A seção **"SUBSCRIPTION"** está visível no rodapé  
- O e-mail é aceito pelo sistema  
- A mensagem **"You have been successfully subscribed!"** é exibida corretamente  
- Nenhum erro ocorre durante o processo  



## Test Case 12 — Add Products in Cart

Este cenário valida a adição de múltiplos produtos ao carrinho de compras e a correta exibição das informações dos itens adicionados.

### Objectivo

Validar o processo de **adição de produtos ao carrinho**, garantindo:

- Acesso à página de produtos  
- Adição de mais de um produto ao carrinho  
- Exibição correta dos produtos no carrinho  
- Exibição correta de preço, quantidade e total  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página **Products** deve estar acessível  
- Devem existir produtos disponíveis para adição  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products** no menu superior  
5. Verificar se o sistema redireciona para a página **All Products**  
6. Selecionar um produto e clicar em **Add to cart**  
7. Clicar em **Continue Shopping**  
8. Selecionar outro produto e clicar em **Add to cart**  
9. Clicar em **View Cart**  
10. Verificar se ambos os produtos estão listados no carrinho  
11. Confirmar que os seguintes dados estão corretos para cada produto:
    - Nome do produto  
    - Preço unitário  
    - Quantidade  
    - Total  

### Resultado Esperado

- Ambos os produtos são adicionados com sucesso  
- O carrinho exibe corretamente todos os itens adicionados  
- Os valores de preço, quantidade e total estão corretos  
- Nenhum erro ocorre durante o processo  


## Test Case 13 — Verify Product Quantity in Cart

Este cenário valida se a quantidade selecionada de um produto antes da adição ao carrinho é corretamente refletida na página do carrinho.

### Objectivo

Validar a **quantidade de produto no carrinho**, garantindo:

- Alteração manual da quantidade na página do produto  
- Adição do produto com quantidade personalizada  
- Exibição correta da quantidade no carrinho  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- Deve existir pelo menos um produto disponível  
- O campo de quantidade deve estar funcional na página do produto  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **View Product** de qualquer produto  
5. Verificar se a página de detalhes do produto é exibida  
6. Localizar o campo de quantidade  
7. Limpar o valor padrão  
8. Informar uma **quantidade maior que 1** (por exemplo: 4)  
9. Clicar no botão **Add to cart**  
10. Clicar em **View Cart**  
11. Verificar se o produto está listado no carrinho  
12. Confirmar que a quantidade exibida corresponde ao valor informado  
13. Confirmar que o total do produto é calculado corretamente com base na nova quantidade  

### Resultado Esperado

- O produto é adicionado ao carrinho com a quantidade selecionada  
- A quantidade exibida no carrinho corresponde ao valor informado  
- O total é calculado corretamente  
- Nenhum erro ocorre durante o processo  



## Test Case 14 — Place Order: Register While Checkout

Este cenário valida o fluxo completo de finalização de compra realizando o cadastro do usuário durante o processo de checkout.

### Objectivo

Validar o processo de **finalização de pedido registrando o usuário durante o checkout**, garantindo:

- Adição de produto ao carrinho  
- Redirecionamento para registro ao iniciar checkout  
- Cadastro completo do usuário  
- Login automático após registro  
- Finalização do pedido com sucesso  
- Exclusão da conta ao final  

### Pré-condição

- O usuário não deve estar autenticado  
- Deve existir pelo menos um produto disponível para compra  
- Dados válidos devem estar disponíveis para cadastro e pagamento  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Adicionar produtos ao carrinho  
5. Clicar no botão **Cart**  
6. Verificar se a página do carrinho é exibida  
7. Clicar em **Proceed To Checkout**  
8. Clicar no botão **Register / Login**  
9. Preencher **Nome** e **Endereço de E-mail**  
10. Clicar no botão **Signup**  
11. Verificar se **"ENTER ACCOUNT INFORMATION"** está visível  
12. Preencher os dados da conta:
    - Título  
    - Nome  
    - E-mail  
    - Senha  
    - Data de Nascimento  
13. Marcar a opção **"Sign up for our newsletter!"**  
14. Marcar a opção **"Receive special offers from our partners!"**  
15. Preencher os dados de endereço:
    - Primeiro Nome  
    - Sobrenome  
    - Empresa  
    - Endereço  
    - Endereço 2  
    - País  
    - Estado  
    - Cidade  
    - CEP  
    - Número de Celular  
16. Clicar no botão **Create Account**  
17. Verificar se **"ACCOUNT CREATED!"** está visível  
18. Clicar no botão **Continue**  
19. Verificar se **"Logged in as _username_"** está visível  
20. Clicar no botão **Cart**  
21. Clicar em **Proceed To Checkout**  
22. Verificar os detalhes do endereço e revisar o pedido  
23. Inserir comentário no campo **Description**  
24. Clicar em **Place Order**  
25. Preencher os dados de pagamento:
    - Name on Card  
    - Card Number  
    - CVC  
    - Expiration Date  
26. Clicar em **Pay and Confirm Order**  
27. Verificar se a mensagem **"Your order has been placed successfully!"** está visível  
28. Clicar no botão **Delete Account**  
29. Verificar se **"ACCOUNT DELETED!"** está visível  
30. Clicar em **Continue**

### Resultado Esperado

- O usuário é registrado com sucesso durante o checkout  
- O login é realizado automaticamente  
- O pedido é finalizado com sucesso  
- A mensagem de confirmação do pedido é exibida  
- A conta é excluída corretamente ao final do teste  


## Test Case 15 — Place Order: Register Before Checkout

Este cenário valida o fluxo completo de finalização de compra realizando o cadastro do usuário antes de iniciar o processo de checkout.

### Objectivo

Validar o processo de **finalização de pedido com usuário previamente registrado**, garantindo:

- Registro completo antes da compra  
- Login bem-sucedido  
- Adição de produtos ao carrinho  
- Exibição correta dos detalhes no checkout  
- Finalização do pedido com sucesso  
- Exclusão da conta ao final  

### Pré-condição

- O usuário não deve estar autenticado  
- Deve existir pelo menos um produto disponível para compra  
- Dados válidos devem estar disponíveis para cadastro e pagamento  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Preencher **Nome** e **Endereço de E-mail**  
6. Clicar no botão **Signup**  
7. Verificar se **"ENTER ACCOUNT INFORMATION"** está visível  
8. Preencher os dados da conta:
   - Título  
   - Nome  
   - E-mail  
   - Senha  
   - Data de Nascimento  
9. Marcar a opção **"Sign up for our newsletter!"**  
10. Marcar a opção **"Receive special offers from our partners!"**  
11. Preencher os dados de endereço:
    - Primeiro Nome  
    - Sobrenome  
    - Empresa  
    - Endereço  
    - Endereço 2  
    - País  
    - Estado  
    - Cidade  
    - CEP  
    - Número de Celular  
12. Clicar no botão **Create Account**  
13. Verificar se **"ACCOUNT CREATED!"** está visível  
14. Clicar no botão **Continue**  
15. Verificar se **"Logged in as _username_"** está visível  
16. Adicionar produtos ao carrinho  
17. Clicar no botão **Cart**  
18. Verificar se a página do carrinho é exibida  
19. Clicar em **Proceed To Checkout**  
20. Verificar os detalhes do endereço e revisar o pedido  
21. Inserir comentário no campo **Description**  
22. Clicar em **Place Order**  
23. Preencher os dados de pagamento:
    - Name on Card  
    - Card Number  
    - CVC  
    - Expiration Date  
24. Clicar em **Pay and Confirm Order**  
25. Verificar se a mensagem **"Your order has been placed successfully!"** está visível  
26. Clicar no botão **Delete Account**  
27. Verificar se **"ACCOUNT DELETED!"** está visível  
28. Clicar em **Continue**

### Resultado Esperado

- O usuário é registrado com sucesso antes do checkout  
- O login é realizado corretamente  
- O pedido é finalizado com sucesso  
- A mensagem de confirmação do pedido é exibida  
- A conta é excluída corretamente ao final do teste  



## Test Case 16 — Place Order: Login Before Checkout

Este cenário valida o fluxo completo de finalização de compra realizando login antes de iniciar o processo de checkout.

### Objectivo

Validar o processo de **finalização de pedido com usuário previamente autenticado**, garantindo:

- Login bem-sucedido antes da compra  
- Adição de produtos ao carrinho  
- Exibição correta dos detalhes no checkout  
- Finalização do pedido com sucesso  
- Exclusão da conta ao final  

### Pré-condição

- O usuário deve estar previamente cadastrado  
- O usuário não deve estar autenticado no início do teste  
- Deve existir pelo menos um produto disponível para compra  
- Dados válidos devem estar disponíveis para pagamento  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Signup / Login**  
5. Informar **Endereço de E-mail válido** e **Senha correta**  
6. Clicar no botão **Login**  
7. Verificar se **"Logged in as _username_"** está visível  
8. Adicionar produtos ao carrinho  
9. Clicar no botão **Cart**  
10. Verificar se a página do carrinho é exibida  
11. Clicar em **Proceed To Checkout**  
12. Verificar os detalhes do endereço e revisar o pedido  
13. Inserir comentário no campo **Description**  
14. Clicar em **Place Order**  
15. Preencher os dados de pagamento:
    - Name on Card  
    - Card Number  
    - CVC  
    - Expiration Date  
16. Clicar em **Pay and Confirm Order**  
17. Verificar se a mensagem **"Your order has been placed successfully!"** está visível  
18. Clicar no botão **Delete Account**  
19. Verificar se **"ACCOUNT DELETED!"** está visível  
20. Clicar em **Continue**

### Resultado Esperado

- O login é realizado com sucesso  
- O checkout é concluído corretamente  
- A mensagem de confirmação do pedido é exibida  
- A conta é excluída corretamente ao final do teste  




## Test Case 17 — Remove Products From Cart

Este cenário valida a funcionalidade de remoção de produtos do carrinho de compras, garantindo que o item seja excluído corretamente da lista e que o carrinho seja atualizado.

### Objectivo

Validar o processo de **remoção de produto do carrinho**, garantindo:

- Adição prévia de produto ao carrinho  
- Acesso correto à página do carrinho  
- Remoção do item selecionado  
- Atualização correta da lista de produtos no carrinho  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- Deve existir pelo menos um produto disponível  
- Um produto deve ser previamente adicionado ao carrinho  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products**  
5. Adicionar um produto ao carrinho  
6. Clicar em **View Cart**  
7. Verificar se o produto está listado no carrinho  
8. Localizar o ícone de remoção (ícone "X") correspondente ao produto  
9. Clicar no ícone de remoção  
10. Verificar se o produto é removido da lista  
11. Confirmar que o carrinho é atualizado corretamente  
12. Confirmar que não há erros durante o processo  

### Resultado Esperado

- O produto é removido com sucesso do carrinho  
- O item não aparece mais na lista  
- O carrinho é atualizado corretamente  
- Nenhum erro é exibido durante a remoção  



## Test Case 18 — View Category Products

Este cenário valida a navegação por categorias de produtos, garantindo que os produtos sejam filtrados corretamente conforme a categoria selecionada.

### Objectivo

Validar a funcionalidade de **visualização de produtos por categoria**, garantindo:

- Exibição da seção de categorias na Página Inicial  
- Expansão das categorias  
- Redirecionamento correto para página da categoria selecionada  
- Exibição apenas dos produtos da categoria escolhida  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A seção **Category** deve estar visível na lateral esquerda  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Localizar a seção **Category** na lateral esquerda  
5. Verificar se as categorias estão visíveis (Women, Men, Kids)  
6. Clicar na categoria **Women**  
7. Selecionar qualquer subcategoria (por exemplo: Dress)  
8. Verificar se o sistema redireciona para a página da categoria selecionada  
9. Confirmar que o título da página corresponde à categoria escolhida  
10. Verificar se os produtos exibidos pertencem à categoria selecionada  
11. Clicar em outra categoria (por exemplo: Men)  
12. Selecionar qualquer subcategoria (por exemplo: T-Shirts)  
13. Verificar se o sistema redireciona corretamente  
14. Confirmar que os produtos exibidos pertencem à nova categoria  

### Resultado Esperado

- As categorias são exibidas corretamente  
- O clique em uma categoria redireciona corretamente  
- O título da página corresponde à categoria selecionada  
- Apenas produtos da categoria escolhida são exibidos  
- Nenhum erro ocorre durante a navegação  




## Test Case 19 — View & Cart Brand Products

Este cenário valida a visualização de produtos por marca e a navegação entre diferentes marcas, garantindo que os produtos sejam filtrados corretamente conforme a marca selecionada.

### Objectivo

Validar a funcionalidade de **visualização de produtos por marca**, garantindo:

- Exibição da seção de marcas  
- Redirecionamento correto ao selecionar uma marca  
- Exibição apenas dos produtos da marca escolhida  
- Navegação correta entre diferentes marcas  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página **Products** deve estar acessível  
- A seção **Brands** deve estar visível na lateral esquerda  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products** no menu superior  
5. Verificar se o sistema redireciona para a página **All Products**  
6. Localizar a seção **Brands** na lateral esquerda  
7. Verificar se as marcas estão visíveis  
8. Clicar em qualquer marca (por exemplo: Polo)  
9. Verificar se o sistema redireciona para a página da marca selecionada  
10. Confirmar que o título da página corresponde à marca escolhida  
11. Verificar se os produtos exibidos pertencem à marca selecionada  
12. Clicar em outra marca (por exemplo: H&M)  
13. Verificar se o sistema redireciona corretamente  
14. Confirmar que os produtos exibidos pertencem à nova marca selecionada  

### Resultado Esperado

- A seção **Brands** é exibida corretamente  
- O clique em uma marca redireciona corretamente  
- O título da página corresponde à marca selecionada  
- Apenas produtos da marca escolhida são exibidos  
- A navegação entre marcas funciona corretamente  
- Nenhum erro ocorre durante o processo  




## Test Case 20 — Search Products and Verify Cart After Login

Este cenário valida se os produtos adicionados ao carrinho antes do login permanecem no carrinho após o usuário realizar autenticação no sistema.

### Objectivo

Validar a persistência do **carrinho após login**, garantindo:

- Busca de produto  
- Adição de produto ao carrinho antes do login  
- Login bem-sucedido  
- Manutenção dos produtos no carrinho após autenticação  

### Pré-condição

- O usuário deve estar previamente cadastrado  
- O usuário não deve estar autenticado no início do teste  
- Deve existir pelo menos um produto correspondente ao termo pesquisado  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products**  
5. Verificar se a página **All Products** é exibida  
6. Informar um nome de produto no campo de busca  
7. Clicar no botão **Search**  
8. Verificar se a seção **"SEARCHED PRODUCTS"** está visível  
9. Adicionar os produtos exibidos ao carrinho  
10. Clicar em **View Cart**  
11. Verificar se os produtos estão listados no carrinho  
12. Clicar em **Signup / Login**  
13. Informar **Endereço de E-mail válido** e **Senha correta**  
14. Clicar no botão **Login**  
15. Verificar se **"Logged in as _username_"** está visível  
16. Clicar novamente em **Cart**  
17. Verificar se os produtos adicionados anteriormente ainda estão presentes no carrinho  

### Resultado Esperado

- Os produtos são adicionados ao carrinho antes do login  
- O login é realizado com sucesso  
- Os produtos permanecem no carrinho após autenticação  
- Nenhum item é removido ou perdido durante o processo  
- Nenhum erro ocorre durante o teste  



## Test Case 21 — Add Review on Product

Este cenário valida a funcionalidade de envio de avaliação (review) em um produto, garantindo que o formulário esteja disponível e que a submissão funcione corretamente.

### Objectivo

Validar o processo de **adição de review em produto**, garantindo:

- Acesso à página de detalhes do produto  
- Visualização da seção de avaliação  
- Preenchimento correto do formulário  
- Envio bem-sucedido da review  
- Exibição da mensagem de confirmação  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- Deve existir pelo menos um produto disponível  
- Um e-mail válido deve estar disponível para preenchimento  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar no botão **Products**  
5. Verificar se a página **All Products** é exibida  
6. Clicar em **View Product** de qualquer produto  
7. Verificar se a página de detalhes do produto é exibida  
8. Rolar a página até a seção **Write Your Review**  
9. Verificar se os campos Name, Email e Review estão visíveis  
10. Informar um **Nome válido**  
11. Informar um **Endereço de E-mail válido**  
12. Informar um **Texto de avaliação válido** no campo Review  
13. Clicar no botão **Submit**  
14. Verificar se a mensagem **"Thank you for your review."** está visível  

### Resultado Esperado

- A seção de review está visível  
- O formulário é preenchido corretamente  
- A review é enviada com sucesso  
- A mensagem **"Thank you for your review."** é exibida  
- Nenhum erro ocorre durante o processo  




## Test Case 22 — Add to Cart from Recommended Items

Este cenário valida a funcionalidade de adicionar produtos ao carrinho diretamente da seção **Recommended Items**, localizada na parte inferior da Página Inicial.

### Objectivo

Validar a funcionalidade de **adição ao carrinho a partir da seção Recommended Items**, garantindo:

- Exibição da seção Recommended Items  
- Adição correta do produto ao carrinho  
- Redirecionamento para a página do carrinho  
- Exibição correta do produto adicionado  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A seção **Recommended Items** deve estar visível  
- Deve existir pelo menos um item recomendado disponível  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Rolar a página até o final  
5. Verificar se a seção **"RECOMMENDED ITEMS"** está visível  
6. Clicar em **Add To Cart** de qualquer produto recomendado  
7. Clicar no botão **View Cart**  
8. Verificar se o sistema redireciona para a página do carrinho  
9. Confirmar que o produto selecionado está listado no carrinho  
10. Confirmar que o nome, preço e quantidade estão corretos  

### Resultado Esperado

- A seção **RECOMMENDED ITEMS** é exibida corretamente  
- O produto é adicionado ao carrinho com sucesso  
- A página do carrinho é carregada corretamente  
- O produto aparece listado com as informações corretas  
- Nenhum erro ocorre durante o processo  




## Test Case 23 — Verify Address Details in Checkout Page

Este cenário valida se os detalhes de endereço (Delivery e Billing Address) exibidos na página de checkout correspondem exatamente às informações fornecidas durante o cadastro do usuário.

### Objectivo

Validar a exibição correta dos **detalhes de endereço no checkout**, garantindo:

- Registro completo do usuário  
- Login bem-sucedido  
- Adição de produto ao carrinho  
- Exibição correta de Delivery Address  
- Exibição correta de Billing Address  
- Correspondência exata com os dados informados no cadastro  

### Pré-condição

- O usuário não deve estar autenticado  
- Deve existir pelo menos um produto disponível  
- Dados válidos devem estar disponíveis para cadastro  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Clicar em **Signup / Login**  
5. Informar **Nome válido** e **E-mail válido não cadastrado**  
6. Clicar em **Signup**  
7. Verificar se **"ENTER ACCOUNT INFORMATION"** está visível  
8. Preencher todos os dados obrigatórios da conta  
9. Preencher todos os dados obrigatórios de endereço:
    - Primeiro Nome  
    - Sobrenome  
    - Empresa  
    - Endereço  
    - Endereço 2  
    - País  
    - Estado  
    - Cidade  
    - CEP  
    - Número de Celular  
10. Clicar em **Create Account**  
11. Verificar se **"ACCOUNT CREATED!"** está visível  
12. Clicar em **Continue**  
13. Verificar se **"Logged in as _username_"** está visível  
14. Adicionar um produto ao carrinho  
15. Clicar em **Cart**  
16. Clicar em **Proceed To Checkout**  
17. Verificar os detalhes exibidos em **Delivery Address**  
18. Verificar os detalhes exibidos em **Billing Address**  
19. Confirmar que todos os dados correspondem exatamente aos informados no cadastro  
20. Clicar em **Delete Account**  
21. Verificar se **"ACCOUNT DELETED!"** está visível  
22. Clicar em **Continue**

### Resultado Esperado

- Os dados de Delivery Address correspondem ao cadastro  
- Os dados de Billing Address correspondem ao cadastro  
- Nenhuma inconsistência é encontrada  
- A conta é excluída corretamente ao final do teste  




## Test Case 24 — Download Invoice After Purchase Order

Este cenário valida a funcionalidade de download da fatura (invoice) após a finalização de um pedido.

### Objectivo

Validar o processo de **download da fatura após a compra**, garantindo:

- Finalização bem-sucedida do pedido  
- Exibição da opção de download da invoice  
- Download correto do arquivo  
- Exclusão da conta ao final  

### Pré-condição

- O usuário não deve estar autenticado  
- Deve existir pelo menos um produto disponível para compra  
- Dados válidos devem estar disponíveis para cadastro e pagamento  
- O navegador deve permitir download de arquivos  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Adicionar produtos ao carrinho  
5. Clicar em **Cart**  
6. Clicar em **Proceed To Checkout**  
7. Clicar em **Register / Login**  
8. Preencher **Nome** e **Endereço de E-mail válido**  
9. Clicar em **Signup**  
10. Verificar se **"ENTER ACCOUNT INFORMATION"** está visível  
11. Preencher todos os dados obrigatórios da conta  
12. Clicar em **Create Account**  
13. Verificar se **"ACCOUNT CREATED!"** está visível  
14. Clicar em **Continue**  
15. Verificar se **"Logged in as _username_"** está visível  
16. Clicar em **Cart**  
17. Clicar em **Proceed To Checkout**  
18. Verificar os detalhes do pedido  
19. Inserir comentário no campo **Description**  
20. Clicar em **Place Order**  
21. Preencher os dados de pagamento:
    - Name on Card  
    - Card Number  
    - CVC  
    - Expiration Date  
22. Clicar em **Pay and Confirm Order**  
23. Verificar se a mensagem **"Your order has been placed successfully!"** está visível  
24. Clicar no botão **Download Invoice**  
25. Verificar se o arquivo é baixado com sucesso  
26. Clicar em **Continue**  
27. Clicar em **Delete Account**  
28. Verificar se **"ACCOUNT DELETED!"** está visível  
29. Clicar em **Continue**

### Resultado Esperado

- O pedido é finalizado com sucesso  
- A opção **Download Invoice** está disponível  
- A invoice é baixada corretamente  
- Nenhum erro ocorre durante o processo  
- A conta é excluída corretamente ao final do teste  



## Test Case 25 — Verify Scroll Up using 'Arrow' Button and Scroll Down Functionality

Este cenário valida a funcionalidade de rolagem da página utilizando o botão de seta (scroll up arrow) e o comportamento de rolagem manual até o rodapé.

### Objectivo

Validar a funcionalidade de **scroll down e scroll up utilizando o botão de seta**, garantindo:

- Rolagem correta até o rodapé  
- Exibição da seção Subscription  
- Exibição do botão de seta para subir  
- Rolagem automática até o topo ao clicar no botão  
- Exibição correta do conteúdo do topo da página  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página deve conter conteúdo suficiente para permitir rolagem  
- O botão de scroll up (seta) deve estar funcional  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Rolar a página até o final  
5. Verificar se a seção **"SUBSCRIPTION"** está visível no rodapé  
6. Verificar se o botão de seta (scroll up arrow) está visível no canto inferior direito  
7. Clicar no botão de seta para subir  
8. Verificar se a página rola automaticamente até o topo  
9. Confirmar que o conteúdo do topo da página está visível (por exemplo: seção principal ou banner inicial)  
10. Confirmar que não ocorre nenhum erro durante o processo  

### Resultado Esperado

- A rolagem até o rodapé funciona corretamente  
- A seção **SUBSCRIPTION** é exibida no final da página  
- O botão de scroll up aparece corretamente  
- Ao clicar na seta, a página retorna ao topo  
- O conteúdo superior da página é exibido corretamente  
- Nenhum erro ocorre durante o teste  




## Test Case 26 — Verify Scroll Up without 'Arrow' Button and Scroll Down Functionality

Este cenário valida a funcionalidade de rolagem manual da página utilizando a barra de rolagem do navegador, sem utilizar o botão de seta (scroll up arrow).

### Objectivo

Validar a funcionalidade de **scroll down e scroll up manual**, garantindo:

- Rolagem correta até o rodapé  
- Exibição da seção Subscription  
- Rolagem manual até o topo  
- Exibição correta do conteúdo superior da página  

### Pré-condição

- O usuário deve estar na Página Inicial do site  
- A página deve conter conteúdo suficiente para permitir rolagem  
- A barra de rolagem do navegador deve estar funcional  

### Passo a passo do test

1. Abrir o navegador  
2. Navegar para a URL: `http://automationexercise.com`  
3. Verificar se a **Página Inicial** é exibida com sucesso  
4. Rolar a página manualmente até o final utilizando a barra de rolagem  
5. Verificar se a seção **"SUBSCRIPTION"** está visível no rodapé  
6. Rolar a página manualmente de volta ao topo  
7. Verificar se o conteúdo principal da parte superior da página está visível  
8. Confirmar que não ocorre nenhum erro durante o processo  

### Resultado Esperado

- A rolagem manual até o rodapé funciona corretamente  
- A seção **SUBSCRIPTION** é exibida corretamente  
- A rolagem manual até o topo funciona corretamente  
- O conteúdo superior da página é exibido corretamente  
- Nenhum erro ocorre durante o teste  
