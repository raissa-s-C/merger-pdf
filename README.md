# Merger PDF

Este script em Python automatiza a junção de vários arquivos PDF em um único documento, eliminando a necessidade de recorrer a sites externos e garantindo total controle e privacidade sobre os seus arquivos.

---

## Como Funciona a Lógica

O processo de automação segue os seguintes passos:

1. **Preparação**: Utiliza a biblioteca `PyPDF2` para a manipulação dos documentos e o módulo nativo `os` para interagir com o sistema de arquivos.
2. **Identificação**: O script lê o conteúdo de uma pasta específica e cria uma lista com todos os arquivos presentes.
3. **Ordenação**: Os arquivos são organizados (através do método `.sort()`) para garantir que a mesclagem ocorre na sequência correta.
4. **Processamento**: O código percorre a lista item a item, valida se a extensão é estritamente `.pdf` e os adiciona ao objeto `PdfMerger`.
5. **Salvamento**: Por fim, o script gera, consolida e salva o novo arquivo final no diretório desejado.

---

## Pré-requisitos

Certifique-se de que tem o **Python** instalado em seu computador. Você precisará instalar a dependência oficial do projeto executando o seguinte comando no terminal:

```bash
pip install PyPDF2
