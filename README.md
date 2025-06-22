# 🐍 Python - Os Primeiros Passos

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

**Projeto de aprendizado dos fundamentos da linguagem Python**

[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Python Version](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge)](https://python.org)

</div>

---

## 📖 Descrição

Este repositório contém meus primeiros passos na linguagem Python, incluindo exercícios práticos, projetos básicos e conceitos fundamentais aprendidos durante minha jornada de aprendizado. Cada arquivo representa um conceito específico ou exercício prático.

## 🎯 Objetivos do Projeto

- ✅ Aprender os fundamentos da linguagem Python
- ✅ Praticar conceitos básicos de programação
- ✅ Desenvolver lógica de programação
- ✅ Criar projetos práticos e funcionais
- ✅ Documentar o processo de aprendizado

## 📚 Conteúdo do Repositório

### 🐍 Conceitos Básicos
- **Variáveis e Tipos de Dados**
- **Operadores Aritméticos**
- **Estruturas Condicionais**
- **Estruturas de Repetição**
- **Funções**
- **Listas e Dicionários**

### 🎮 Projetos Práticos
- **Calculadora Simples**
- **Jogo da Adivinhação**
- **Sistema de Notas**
- **Conversor de Temperatura**
- **Lista de Tarefas**

## 🛠️ Tecnologias Utilizadas

### Linguagem
- **Python 3.8+** - Linguagem principal

### Ferramentas
- **VS Code** - Editor de código
- **Jupyter Notebook** - Para experimentos
- **Git** - Controle de versão

### Bibliotecas
- **Built-in libraries** - Bibliotecas padrão do Python
- **Math** - Operações matemáticas
- **Random** - Geração de números aleatórios
- **Datetime** - Manipulação de datas

## 🚀 Como Executar

### Pré-requisitos
- Python 3.8 ou superior
- Editor de código (VS Code recomendado)

### Instalação

1. **Clone o repositório**
```bash
git clone https://github.com/juanrodrip/python-os-primeiros-passos.git
cd python-os-primeiros-passos
```

2. **Verifique a instalação do Python**
```bash
python --version
# ou
python3 --version
```

3. **Execute os arquivos**
```bash
# Exemplo de execução
python nome_do_arquivo.py
```

## 📁 Estrutura do Projeto

```
python-os-primeiros-passos/
├── 01_variaveis.py           # Variáveis e tipos
├── 02_operadores.py          # Operadores aritméticos
├── 03_condicionais.py        # Estruturas if/else
├── 04_loops.py              # Estruturas de repetição
├── 05_funcoes.py            # Definição de funções
├── 06_listas.py             # Manipulação de listas
├── 07_dicionarios.py        # Trabalhando com dicionários
├── projetos/
│   ├── calculadora.py       # Calculadora simples
│   ├── adivinhacao.py       # Jogo da adivinhação
│   └── notas.py             # Sistema de notas
├── README.md                # Documentação
└── requirements.txt         # Dependências (se houver)
```

## 🎮 Exemplos de Código

### Calculadora Simples
```python
def calculadora():
    print("=== Calculadora Simples ===")
    num1 = float(input("Digite o primeiro número: "))
    num2 = float(input("Digite o segundo número: "))
    operacao = input("Digite a operação (+,-,*,/): ")
    
    if operacao == '+':
        resultado = num1 + num2
    elif operacao == '-':
        resultado = num1 - num2
    elif operacao == '*':
        resultado = num1 * num2
    elif operacao == '/':
        resultado = num1 / num2 if num2 != 0 else "Erro: Divisão por zero"
    else:
        resultado = "Operação inválida"
    
    print(f"Resultado: {resultado}")

if __name__ == "__main__":
    calculadora()
```

### Jogo da Adivinhação
```python
import random

def jogo_adivinhacao():
    numero_secreto = random.randint(1, 100)
    tentativas = 0
    max_tentativas = 10
    
    print("=== Jogo da Adivinhação ===")
    print(f"Tente adivinhar o número entre 1 e 100. Você tem {max_tentativas} tentativas.")
    
    while tentativas < max_tentativas:
        try:
            palpite = int(input("Digite seu palpite: "))
            tentativas += 1
            
            if palpite < numero_secreto:
                print("Muito baixo! Tente um número maior.")
            elif palpite > numero_secreto:
                print("Muito alto! Tente um número menor.")
            else:
                print(f"Parabéns! Você acertou em {tentativas} tentativas!")
                return
                
        except ValueError:
            print("Por favor, digite um número válido.")
    
    print(f"Game Over! O número era {numero_secreto}.")

if __name__ == "__main__":
    jogo_adivinhacao()
```

## 📊 Progresso de Aprendizado

### ✅ Conceitos Dominados
- [x] Variáveis e tipos de dados
- [x] Operadores aritméticos e lógicos
- [x] Estruturas condicionais (if/else)
- [x] Estruturas de repetição (for/while)
- [x] Funções e parâmetros
- [x] Listas e manipulação
- [x] Dicionários
- [x] Tratamento de exceções

### 🎯 Próximos Passos
- [ ] Programação orientada a objetos
- [ ] Módulos e pacotes
- [ ] Manipulação de arquivos
- [ ] APIs e requisições HTTP
- [ ] Frameworks web (Flask/Django)
- [ ] Análise de dados (Pandas)
- [ ] Automação web (Selenium)

## 🧪 Testes

### Como Testar
```bash
# Execute cada arquivo individualmente
python 01_variaveis.py
python 02_operadores.py
python 03_condicionais.py
# ... e assim por diante
```

### Verificação de Sintaxe
```bash
# Verificar se não há erros de sintaxe
python -m py_compile nome_do_arquivo.py
```

## 📈 Métricas do Projeto

- **Arquivos Python**: 10+
- **Linhas de Código**: ~500
- **Projetos Práticos**: 5
- **Conceitos Aplicados**: 15+
- **Tempo de Desenvolvimento**: 3 semanas

## 🤝 Contribuição

Este é um projeto de aprendizado pessoal, mas sugestões e melhorias são sempre bem-vindas!

### Como Contribuir
1. **Fork** o projeto
2. **Crie** uma branch para sua feature
3. **Commit** suas mudanças
4. **Push** para a branch
5. **Abra** um Pull Request

## 📚 Recursos de Aprendizado

### Cursos e Tutoriais
- [Curso em Vídeo - Python](https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6)
- [Documentação Oficial Python](https://docs.python.org/pt-br/3/)
- [W3Schools Python](https://www.w3schools.com/python/)

### Livros Recomendados
- "Python para Iniciantes" - Mark Lutz
- "Automate the Boring Stuff with Python" - Al Sweigart
- "Python Crash Course" - Eric Matthes

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Juan Rodriguez**

- GitHub: [@juanrodrip](https://github.com/juanrodrip)
- LinkedIn: [Juan Rodriguez](https://linkedin.com/in/juanrodrip)
- Portfolio: [juanrodrip.github.io](https://juanrodrip.github.io)

## 🙏 Agradecimentos

- **Gustavo Guanabara** pelo curso excelente
- **Comunidade Python** pelo suporte
- **Stack Overflow** pelas soluções
- **GitHub** pela plataforma

## 🎯 Próximos Objetivos

- [ ] **Projeto Web** - Criar uma aplicação web com Flask
- [ ] **Automação** - Scripts para automação de tarefas
- [ ] **Análise de Dados** - Projetos com Pandas e Matplotlib
- [ ] **API REST** - Desenvolver APIs com FastAPI
- [ ] **Machine Learning** - Introdução ao scikit-learn

---

<div align="center">

**🐍 Python é incrível! Continue aprendendo! 🐍**

[![GitHub stars](https://img.shields.io/github/stars/juanrodrip/python-os-primeiros-passos?style=social)](https://github.com/juanrodrip/python-os-primeiros-passos/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/juanrodrip/python-os-primeiros-passos?style=social)](https://github.com/juanrodrip/python-os-primeiros-passos/network)

</div>
