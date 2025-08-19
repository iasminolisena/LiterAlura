# Challenge Literalura 📚

Aplicação em **Spring Boot + JPA + banco relacional** que permite buscar, salvar e listar livros e autores utilizando a API do **Project Gutenberg** e persistência local via repositório.

---

## 🚀 Funcionalidades
- Buscar livro pelo título (API do Project Gutenberg + salvar no banco)  
- Listar livros registrados  
- Listar autores registrados  
- Listar autores vivos em um ano específico  
- Listar livros por idioma (pt, en, es, fr)  
- Exibir Top 10 livros mais baixados  
- Encerrar a aplicação  

---

## 🛠️ Tecnologias
- Java 17+  
- Spring Boot  
- Hibernate / JPA  
- PostgreSQL  
- Maven  
- API: Project [Gutenberg](https://gutendex.com/)  

---

## ⚙️ Configuração e Execução

1. Clone o repositório:  
   ```bash
   git clone https://github.com/cristiellesreis/projeto-literAlura.git
   cd projeto-literAlura
   ```
2. Configure o banco de dados no arquivo src/main/resources/application.properties:
  ```
  spring.datasource.url=jdbc:postgresql://${DB_HOST}/literalura_db
  spring.datasource.username=${DB_USERNAME}
  spring.datasource.password=${DB_PASSWORD}
  spring.jpa.hibernate.ddl-auto=update
  ```
3. Execute a aplicação:
  ```bash
  ./mvnw spring-boot:run
  ```
4. Use o menu interativo no terminal:
  ```
  ***** Literalura *****
  
  1 - Buscar livro pelo título
  2 - Listar livros registrados
  3 - Listar autores registrados
  4 - Listar autores vivos em um ano específico
  5 - Listar livros por idioma
  6 - Top 10 livros mais baixados
  7 - Sair
  ```
## 📁 Estrutura do Projeto
  ```
src/
 ├─ main/
 │   ├─ java/br/com/alura/literalura/
 │   │    ├─ modelos/       → Entidades JPA (Livro, Autor)
 │   │    ├─ dto/           → DTOs para transferência de dados
 │   │    ├─ repositorio/   → Repositórios Spring Data
 │   │    ├─ servico/       → Lógica de negócios (API, conversões)
 │   │    └─ principal/     → Classe de entrada e menu interativo
 │   └─ resources/          → Configurações (application.properties)
```
## 📚 Créditos
Projeto desenvolvido como desafio pelo programa:

- Oracle Next Education
- Alura - Cursos de tecnologia

## ⚖️ Licença
Projeto de uso educacional, livre para estudos e modificações.

👩‍💻 Desenvolvido com ☕ por Iasmin Oliveira
