# AutomationExerciseDotCom
Automatizar o site playground de e-commerce: https://automationexercise.com/

## Checklist — Automation Exercise

- [x] Test Case 1: Register User
- [ ] Test Case 2: Login User with correct email and password
- [x] Test Case 3: Login User with incorrect email and password
- [x] Test Case 4: Logout User
- [x] Test Case 5: Register User with existing email
- [ ] Test Case 6: Contact Us Form
- [x] Test Case 7: Verify Test Cases Page
- [ ] Test Case 8: Verify All Products and product detail page
- [ ] Test Case 9: Search Product
- [ ] Test Case 10: Verify Subscription in home page
- [ ] Test Case 11: Verify Subscription in Cart page
- [ ] Test Case 12: Add Products in Cart
- [ ] Test Case 13: Verify Product quantity in Cart
- [ ] Test Case 14: Place Order — Register while Checkout
- [ ] Test Case 15: Place Order — Register before Checkout
- [ ] Test Case 16: Place Order — Login before Checkout
- [ ] Test Case 17: Remove Products From Cart
- [ ] Test Case 18: View Category Products
- [ ] Test Case 19: View & Cart Brand Products
- [ ] Test Case 20: Search Products and Verify Cart After Login
- [ ] Test Case 21: Add review on product
- [ ] Test Case 22: Add to cart from Recommended items
- [ ] Test Case 23: Verify address details in checkout page
- [ ] Test Case 24: Download Invoice after purchase order
- [ ] Test Case 25: Verify Scroll Up using 'Arrow' button and Scroll Down functionality
- [ ] Test Case 26: Verify Scroll Up without 'Arrow' button and Scroll Down functionality

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

