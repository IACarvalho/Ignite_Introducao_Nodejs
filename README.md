# Anotações Introdução ao NodeJS
## Métodos de rotas
- **GET** -> Buscar informação no servidor
- **POST** -> Inserir informação no servidor
- **PUT** -> Alterar uma informação no servidor
- **PATH** -> Alterar uma informação específica
- **DELETE** -> Ecluir uma informação no servidor

## Tipos de parâmetros
- **Route params** -> São parâmetros passando dentro da rota, e são parâmetros obrigatórios. Sevem para identificar, buscar, modificar ou deletar um recurso.
	- O nome do parâmetro é o mesmo da assinatura da rota
	- Para recuperar o calor de um route param ´usado: request.params.
- **Query params** -> Assim como os route params é passado na rota, mas difere no fato de não se tornar uma parte obrigatória da rota (não causa erro caso não seja passado).
	- Servem para paginação e filtro
	- Os query params são passados ao acessar uma rota, não estão na assinatura da rota. é passado após um sinalk de interrogação (?) nome do parâmetro e o valor. Ex: localhost:3333/rota?page=1
	- Para passar mais de um parâmetro basta "concatenar" usando um & entre os parâmetros.
	- Para recuperar o valor basta usar: request.query
- **Body params** -> São parâmetros usados normalmente em formulários, cadastrar um usuário, livro, produto, etc. Pega as informações direto do corpo do projeto.
	- Para recuperar as informações usa: request.body
	