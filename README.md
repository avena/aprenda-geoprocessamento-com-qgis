Material do [Aprenda geoprocessamento com QGIS](https://www.udemy.com/course/aprenda-geoprocessamento-com-qgis/)

## Simbologia Categorizada

Utilizada para classificar dados em categorias individuais. Funciona tanto com textos quanto com números, criando uma cor ou símbolo distinto para cada valor único encontrado no campo.

- Agrupa por valores únicos. Aceita campos de texto ou numéricos.

Na Camada, clicar com o botão direito > Propriedades > Simbologia > Selecionar "Categorizada" no menu suspenso > Escolher o campo desejado > Clicar em "Classificar" > Ajustar cores e símbolos conforme necessário > Clicar em "OK" para aplicar.

## Simbologia Graduada

Ideal para representar grandezas. Para utilizá-la, o atributo do campo deve ser obrigatoriamente do tipo numérico, permitindo a criação de classes baseadas em intervalos (como mapas de calor ou densidade).

- Representa intervalos de valores. Exige campo numérico.

Na Camada, clicar com o botão direito > Propriedades > Simbologia > Graduada no menu suspenso

- Selecionar o campo numérico desejado > Escolher o método de classificação (Cor ou Tamanho) > Definir o modo de classes (Desvio Padrão, Escala Logarítmica, Igual Contagem (Quartil), Intervalo Igual, Quebra Natural (Jenks), Quebras Suaves) > Pode mudar a quantidade classes > Clicar em "Classificar" > Ajustar cores e símbolos conforme necessário > Clicar em "OK" para aplicar.

Assim no mapa, Valores maiores e menores pode ter cores ou tamanhos diferentes, facilitando a visualização de variações na grandeza representada.

## Simbologia Baseado em Regra

Permite a criação de regras personalizadas para a simbologia, utilizando expressões lógicas para definir como os dados serão representados. Isso é útil quando se deseja aplicar estilos específicos com base em múltiplas condições.

- Usa expressões lógicas para definir regras de simbologia.
  Na Camada, clicar com o botão direito > Propriedades > Simbologia > Selecionar "Regras" no menu suspenso > Definir um nome para o Rótulo > Clicar em "+" para adicionar uma nova regra > Definir a expressão lógica para a regra > Escolher o símbolo e cor desejados > Repetir para outras regras conforme necessário > Clicar em "OK" para aplicar.

  Algumas expressões comuns incluem:

  - "campo" = 'valor' (para texto)
  - "campo" > valor (para números)
  - "campo" < valor (para números)
  - "campo" BETWEEN valor1 AND valor2 (para intervalos numéricos)
  - "campo" IS NULL (para valores nulos)
  - "campo" IS NOT NULL (para valores não nulos)
  - Combinações usando AND, OR, NOT para criar condições mais complexas.  
    Exemplo: "população" > 1000 AND "área" < 50
