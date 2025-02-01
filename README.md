# Automacao com PyAutoGUI

## Descricao
Este projeto utiliza a biblioteca `pyautogui` para automatizar interacoes na tela, localizando e clicando em imagens predefinidas.

## Requisitos
Certifique-se de ter instalado o Python e as bibliotecas necessarias antes de executar o script.

### Instalacao das dependencias
```bash
pip install pyautogui
```

## Como funciona
O script busca por imagens especificas na tela e realiza cliques automaticamente quando elas sao encontradas. Ele tambem inclui um loop principal que permite a execucao continua ate que o usuario interrompa o processo manualmente.

### Fluxo do Script
1. O script espera um tempo determinado entre cada iteracao.
2. Ele tenta localizar e clicar nas imagens conforme a logica definida.
3. Se uma imagem for encontrada, o clique e realizado.
4. Se a imagem nao for encontrada, o script continua a procurar.
5. O loop continua ate que o usuario interrompa a execucao (Ctrl + C).

## Como usar
1. Substitua os arquivos de imagem (`claim.png`, `fechar.png`, `farmar.png`) pelos que deseja utilizar.
2. Execute o script com:
   ```bash
   python nome_do_arquivo.py
   ```
3. O script rodara em loop, verificando e clicando nas imagens conforme necessario.

## Personalizacao
- Modifique os nomes dos arquivos de imagem para refletirem os elementos corretos da interface que deseja automatizar.
- Ajuste os tempos de espera (`time.sleep(x)`) conforme necessario.
- Altere o parametro `confidence` para melhorar a precisao na deteccao das imagens.

## Observacoes
- Certifique-se de que as imagens utilizadas estao bem definidas e visiveis para evitar erros de deteccao.
- O script pode falhar caso a interface mude ou a resolucao da tela seja alterada.

## Interrupcao
Para interromper a execucao do script, pressione `Ctrl + C` no terminal.

