# techconsult-aula3-dinamicaBD
em desenvolvimento
A partir das regras da ECHCONSULT, podemos montar o MER (Modelo Entidade-Relacionamento) identificando as entidades, seus atributos e os relacionamentos com suas respectivas cardinalidades.

próxima alteração na lição será com foco nas 
      Entidades

    DEPARTAMENTO
        id_departamento (PK)
        nome

    FUNCIONARIO
        id_funcionario (PK)
        nome
        cargo
        email
        telefone
        id_departamento (FK)

    CLIENTE
        id_cliente (PK)
        nome
        cpf_cnpj
        email
        telefone
        endereco

    PROJETO
        id_projeto (PK)
        nome
        descricao
        data_inicio
        data_fim
        id_cliente (FK)

    CONSULTOR
        id_consultor (PK)
        nome
        especialidade
        email
        telefone

    LOCACAO
        id_locacao (PK)
        data_locacao
        data_inicio
        data_fim
        valor
        id_cliente (FK)
        id_funcionario (FK)

    ALOCACAO
        id_projeto (PK/FK)
        id_consultor (PK/FK)
        horas
        funcao

A entidade ALOCACAO é necessária porque existe um relacionamento N:N entre Projeto e Consultor e, além disso, esse relacionamento possui os atributos horas e funcao.
