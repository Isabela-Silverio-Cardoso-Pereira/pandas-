# pandas-


**Criar um dataframe a partir de um dicionário**


//CODE
import pandas as pd

student_data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 92, 78]
}
df = pd.DataFrame(student_data)
print(df)
//END CODE

**Escolhendo a ordem das colunas**

//CODE
import pandas as pd
student_data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 92, 78]
}
df = pd.DataFrame(student_data, columns=['Score', 'Name'])
print(df)
//END CODE

**Adicionar nome aos ids**

import pandas as pd
student_data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 92, 78]
}
index_labels = ['ID1', 'ID2', 'ID3']
df = pd.DataFrame(student_data, index=index_labels)
print(df)

**Acessando a coluna de um dataframe pelo nome**

import pandas as pd
student_data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 92, 78]
}
df = pd.DataFrame(student_data)
print(df.Name)

**Vendo um resumo do dataframe usando info**

import pandas as pd
student_data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Score': [85, 92, 78]
}
df = pd.DataFrame(student_data)
df.info()
