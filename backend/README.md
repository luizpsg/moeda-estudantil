# Sistema de Moeda Estudantil - Backend

Este é o backend do Sistema de Moeda Estudantil, uma plataforma que permite a gestão de uma moeda virtual para estudantes, onde professores podem conceder moedas aos alunos e estes podem resgatar vantagens oferecidas por empresas parceiras.

## Funcionalidades Principais

- Sistema de notificações por email
- Gestão de moedas estudantis
- Resgate de vantagens/cupons
- Integração com empresas parceiras
- Sistema de reenvio automático de notificações

## Tecnologias Utilizadas

- Java
- Spring Boot
- Spring Data JPA
- Spring Mail
- PostgreSQL (assumido baseado na estrutura do projeto)

## Estrutura do Projeto

```
src/main/java/br/com/moeda_estudantil/
├── controller/     # Controladores REST
├── model/         # Entidades do sistema
├── repository/    # Repositórios JPA
├── service/       # Lógica de negócio
└── dto/           # Objetos de transferência de dados
```

## Configuração

1. Clone o repositório
2. Configure as variáveis de ambiente necessárias (email, banco de dados, etc.)
3. Execute o projeto usando Maven ou sua IDE preferida

## Endpoints Principais

- `/api/alunos` - Gestão de alunos
- `/api/professores` - Gestão de professores
- `/api/empresas` - Gestão de empresas parceiras
- `/api/vantagens` - Gestão de vantagens disponíveis
- `/api/resgates` - Gestão de resgates de vantagens
- `/api/notificacoes` - Gestão de notificações

## Sistema de Notificações

O sistema possui um serviço robusto de notificações que:

- Envia emails automáticos para alunos e empresas
- Mantém histórico de todas as notificações
- Possui sistema de reenvio automático para notificações que falharam
- Notifica sobre:
  - Recebimento de moedas
  - Resgate de vantagens
  - Cupons gerados

## Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

## Licença

Este projeto está sob a licença [inserir licença aqui].
