# Simulação de Ataque Ransomware em Python

Este projeto contém dois scripts em Python, `criptografia.py` e `decrypte.py`, que simulam um ataque ransomware para criptografar e descriptografar arquivos utilizando o algoritmo AES (Advanced Encryption Standard) por meio da biblioteca `pyaes`.

## Códigos:

### `criptografia.py` (Criptografar)

Este script é responsável por criptografar arquivos, simulando um ataque ransomware. Aqui está uma visão geral do processo:

1. **Abrir o Arquivo Original:**
   - O script lê o conteúdo do arquivo especificado.

2. **Remover o Arquivo Original:**
   - O arquivo original é removido após a leitura do conteúdo.

3. **Chave de Criptografia:**
   - Uma chave de criptografia (exemplo: `b'testeransowares'`) é definida no script.

4. **Criptografar o Arquivo:**
   - O conteúdo do arquivo é criptografado usando o AES e salvo em um novo arquivo com a extensão `.ransowaretroll`.

### `decrypte.py` (Descriptografar)

Este script é responsável por descriptografar os arquivos criptografados pelo script `criptografia.py`. Aqui está uma visão geral do processo:

1. **Abrir o Arquivo Criptografado:**
   - O script lê o conteúdo do arquivo criptografado especificado.

2. **Chave de Descriptografia:**
   - Uma chave de descriptografia (exemplo: `b'testeransowareds'`) é definida no script.

3. **Descriptografar o Arquivo:**
   - O conteúdo do arquivo criptografado é descriptografado usando a chave de descriptografia.

4. **Remover o Arquivo Criptografado:**
   - O arquivo criptografado é removido após a descriptografia.

5. **Criar Novo Arquivo Descriptografado:**
   - Um novo arquivo descriptografado é criado com o nome original.

## Como Usar:

1. **Instalação de Dependências:**
   Certifique-se de que a biblioteca `pyaes` está instalada. Caso não tenha, você pode instalá-la usando o seguinte comando:
   ```bash
   pip install pyaes
