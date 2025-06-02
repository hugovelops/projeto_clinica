<b>Banco de Dados de uma Clínica:</b></br>
Projeto para a disciplina Programação Web na faculdade.
Para funcionar é necessário ter o Bootstrap instalado na mesma pasta com os arquivos como visto na imagem a seguir:


![image](https://github.com/user-attachments/assets/ac686e77-376c-4b21-9bce-5f3cb6f6cbb5)


<b>Diagrama de classes</b>
```mermaid
classDiagram
    class consulta {
        + Integer id_consulta
        + Integer paciente_id_paciente
        + Integer medico_id_medico
        + Date data_consulta
        + Time hora_consulta
        + Text descricao_consulta
    }

    class medico {
        + Integer id_medico
        + String nome_medico
        + String crm_medico
        + String especialidade_medico
    }

    class paciente {
        + Integer id_paciente
        + String nome_paciente
        + String cpf_paciente
        + Date data_nasc_paciente
        + Char sexo_paciente
        + String fone_paciente
        + String email_paciente
        + String endereco_paciente
    }

    consulta "1" *-- "1" medico : medico_id_medico
    consulta "1" *-- "1" paciente : paciente_id_paciente


```
<b>Dependências:</b></br>
<b>Bootstrap</b>- use o link abaixo ou pesquise no seu navegador-
https://getbootstrap.com .</br>
<b>SQL</b> feito pelo <b>DBDesigner</b>.

<b>Atenção:</b></br>
Para usar o projeto, lembre-se de alterar o diretório no começo dos códigos e verifique o nome colocado nas tabelas.