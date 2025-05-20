# Exercícios OpenGL 3.3+ — README

Este projeto contém três exercícios práticos para aprender a criar e manipular geometria básica com OpenGL moderna (3.3+), utilizando GLFW, GLAD e GLM.

## Pré-requisitos

- **GLFW** (https://www.glfw.org/)
- **GLAD** (https://glad.dav1d.de/)
- **GLM** (https://github.com/g-truc/glm)
- Compilador C++ (g++, MinGW recomendado no Windows)

Certifique-se de que os diretórios de include e lib de cada biblioteca estejam corretamente configurados no comando de compilação.

---

## Exercício 1 — `createTriangle.cpp`

Cria uma função `createTriangle` que recebe as coordenadas dos vértices de um triângulo e retorna o VAO correspondente. O programa exibe um único triângulo na tela.

### Compilar:
```sh
g++ createTriangle.cpp C:\libs\glad\src\glad.c -o createTriangle.exe -I"C:\libs\glad\include" -I"C:\libs\glfw\glfw-3.4.bin.WIN64\include" -L"C:\libs\glfw\glfw-3.4.bin.WIN64\lib-mingw-w64" -lglfw3 -lopengl32 -lgdi32
```

---

## Exercício 2 — `fiveTriangles.cpp`

Utiliza a função do exercício 1 para instanciar e desenhar 5 triângulos em posições diferentes na tela.

### Compilar:
```sh
g++ fiveTriangles.cpp C:\libs\glad\src\glad.c -o fiveTriangles.exe -I"C:\libs\glad\include" -I"C:\libs\glfw\glfw-3.4.bin.WIN64\include" -L"C:\libs\glfw\glfw-3.4.bin.WIN64\lib-mingw-w64" -lglfw3 -lopengl32 -lgdi32
```

---

## Exercício 3 — `trianglesWithStruct.cpp`

Define uma struct `Triangle` com posição e cor. Ao clicar na janela, um novo triângulo é criado na posição do mouse, com cor aleatória. Todos os triângulos são desenhados usando o mesmo VAO e transformações via GLM.

### Compilar:
```sh
g++ trianglesWithStruct.cpp C:\libs\glad\src\glad.c -o trianglesWithStruct.exe -I"C:\libs\glad\include" -I"C:\libs\glfw\glfw-3.4.bin.WIN64\include" -I"C:\libs\glm" -L"C:\libs\glfw\glfw-3.4.bin.WIN64\lib-mingw-w64" -lglfw3 -lopengl32 -lgdi32
```

---

## Observações

- Se não quiser que uma janela de console apareça ao executar o `.exe`, adicione `-mwindows` ao comando de compilação.
- Certifique-se de que os caminhos para as bibliotecas e includes estejam corretos para o seu ambiente.
- Para dúvidas sobre instalação das bibliotecas, consulte a documentação oficial de cada uma.

---
