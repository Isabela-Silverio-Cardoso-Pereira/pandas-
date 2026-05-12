# pandas-

**Series**
 Uma Series é um objeto unidimensional semelhante a um array que pode conter qualquer tipo de dado, como inteiros, strings ou floats. 

 //CODE
import pandas as pd
data = [10, 20, 30, 40, 50]
s = pd.Series(data)
print(s)

**Acessando elemento na series pelo indice**


import pandas as pd
data = [10, 20, 30, 40, 50]
s = pd.Series(data)
print("The full Series:")
print(s)
print("\nFirst element:", s[0])
print("\nElements from index 1 to 2:")
print(s[1:3])

**imprimir o tipo de dados dentro de uma seires**

import pandas as pd
data = [10, 20, 30, 40, 50]
s = pd.Series(data)
print("\nData type:", s.dtype)
print("Shape:", s.shape)


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
