## [1.8.0] - 27-07-2022
- Melhoria: Alteraçõa de nomenclarura (erroCallbackListener) para (documentCallbackListener)
- Melhoria: Retornar erros e sucesso via call back (documentCallbackListener)
- Melhoria: Adicionado tipoDeCaptura no retorno do documentCallbackListener
- Melhoria: flag (capturaManual) para habilitar processo de captura manual.
- Melhoria: flag (orientacaoCaptura) para habilitar a mudança na orientação do layout de captura entre a forma "portrait" e "landscape"
- Melhoria: Alteraçõa de nomenclarura da cores (brscan_background_captura, brscan_default_captura e brscan_highlight_captura) por (brscan_documento_background_captura, brscan_documento_default_captura e brscan_documento_highlight_captura) respectivamente.
- Melhoria: Alteraçõa de cores padrão (
    brscan_documento_highlight_captura = #00AF7D,
    brscan_documento_default_captura = #FFFFFF,
    brscan_documento_background_captura = #B2000000,
    brscan_documento_icone_captura_botao_fechar = #FFFFFF e
    brscan_documento_box_texto_orientacao = #00000000)
- Melhoria: Alteraçõa do tamanho da fonte de brscan_documento_tamanho_texto_orientacao para 16px

## [1.7.1] - 20-07-2022
- Correção(hotfix): Atualizar MLKit para versão 2.6.0.

## [1.7.0] - 11-07-2022
- Melhoria: Retornar erros via call back(erroCallbackListener).
- Melhoria: Alterar o tamanho da imagem para envio ao type document.
- Melhoria: Realizar a captura do documento com o device estabilizado.
- Melhoria: Atualizar MLKit para versão 2.6.0.

## [1.6.1] - 29-06-2022
- Correção(hotfix): Atualizar retorno das imagens capturadas.

## [1.6.0] - 27-06-2022
- Melhoria: Adicionado o envio de metadados para análise e processamento.

## [1.5.1] - 02-06-2022
- Correção: Processo com delay 0 e tempo de captura do documento fixo.
- Melhoria: Modificado flag (tempoDelayMensagem) para 0ms como default.
- Melhoria: Mudança flag (tempoDelayMensagem) depreciada.
- Melhoria: Adicionado flag (tokenTentativa) define quantos tokens extra podem ser usados(0 default)

## [1.5.0] - 17-05-2022
- Correção(hotfix): Atualizar URL do SSL Pinning.

## [1.4.9] - 10-05-2022
- Melhoria(hotfix): Atualizar cor dos boxes de texto de oritencão e lado do documento.
- Melhoria: Incluído possibilidade de utilização de opacidade nas cores hexadecimais.

## [1.4.8] - 06-05-2022
- Melhoria(hotfix): Modificar propriedades para receber o json de resposta da URL.

## [1.4.7] - 05-05-2022
- Melhoria: Atualizar endpoint de validação da chave
- Melhoria: Impedir a execução em emuladores

## [1.4.6] - 26-04-2022
- Melhoria: Melhorar o tempo de captura com delay

## [1.4.5] - 25-04-2022
- Melhoria: Adicionado flag (tempoDelayMensagem) define o tempo de exibição entre as mensagem de processo(2000ms default).
- Melhoria: Adicionado flag (acessibilidade) que habilita recurso de acessibilidade A+
- Melhoria: Incluído customização(via plist) de cores texto e caixa de orientações na tela de captura.
- Melhoria: Incluído customização(via plist) de tamanho texto de orientações na tela de captura.

## [1.4.4] - 14-04-2022
- Melhoria: remover meta do base64

## [1.4.3] - 13-04-2022
- Melhoria: Adicionado flag verificarLuminosidae
- Melhoria: Adicionado Label (RG, CNH ou documento) e o lado (Frente, Verso e Aberto) quando informado
- Melhoria: Mudança do nome de arquivo de configuracoes.plist para configuracoes_documento.plist
- Melhoria: Cliente poderá incluir o arquivo de configurações direto no app e editá-lo.

## [1.4.2] - 04-04-2022
- Melhoria: Adicionado flag (scoreMinimo) para receber o valor de score mínimo aceito (0 a 100 default 60)
- Melhoria: Incluído meta do retorno de tipo "base64" data:image/jpeg;base64,.
- Melhoria: No retorno com erro será retornado o Código do erro, a Descrição do erro e o iD da analise 
- Melhoria: Incluído parametrização da cor do background do frame de loading
- Melhoria: Incluído parametrização da cor do botão dos frames.
- Melhoria: Incluído parametrização da cor do Check das instruções.
- Melhoria: Retornando apenas um delegate de sucesso e um delegate no carro de erro

## [1.4.1] - 28-03-2022
- Melhoria: Adicionado flag (retornarErros) que retona todos os erros para aplicação cliente.
- Melhoria: Mudança de flag (segurancaExtra) depreciada.
- Melhoria: Adicionado flag (segurancaExtraRootCheck) para validar se o dispositivo está no modo root.
- Melhoria: Adicionado flag (segurancaExtraSslPinning) para validar ssl pinning.
- Correção: botão de captura pegando a cor Secondary

## [1.4.0] - 17-03-2022
- Melhoria: Alteração apontamento para novo serviço document.brscan.com.br/v1/.
- Melhoria: Adicionado botão de fechar na tela inicial (quando wizard for true) que possibilita sair do sdk.
- Melhoria: Alteração no botão de fechar da tela de captura para um "X" da cor preta.
- Melhoria: Remoção de validação por score e Depreciação da flag (scoreMinimo).
- Melhoria: Possibilidade de alteração do shape do botão de captura manual por uma imagem
- Melhoria: Adicionando no objeto de retorno o id da captura.

## [1.3.3] - 23-02-2022
- Melhoria: Adicionar flag "scoreMinimo" para permitir o cliente passar o valor desejado.

## [1.3.2] - 16-02-2022
- Melhoria: Corrigir texto quebrado na tela de preview
- Melhoria: Remover logs da aplicação

## [1.3.1] - 11-02-2022
- Melhoria: Modificar nome do objeto de personalização do layout

## [1.3.0] - 10-02-2022
- Melhoria: Adicionado flag (swiper) para habilitar/desabilitar telas de instruções para captura com iconografia.
- Melhoria: Adicionado flag (telaSelecaoDocumento) para habilitar/desabilitar tela de escolha do tipo de documento.
- Melhoria: Adicionado imagem cropada na tela de confirmação do documento.
- Melhoria: Retorno de imagens em base64 em baixa resolução.
- Melhoria: Retorno de boundingbox da imagem.
- Melhoria: Adicionado flag (resolucao) para informar o tipo de resolução(low, hd e original) da imagem a ser salva.
- Melhoria: Adicionado flag (ladoDocumentoAceito) para capturar apenas um lado específico.
- Melhoria: Remoção de imagens capturadas anteriormente pela lib.
- Melhoria: Adicionado tela de erro de conexão com opções de enviar novamente ou cancelar o processo.
- Melhoria: Adicionado flag (telaPreview) para habilitar/desabilitar telas de Preview
- Melhoria: Adicionado flag (tipoRetorno) para escolher entre base64 ou path do arquivo
- Melhoria: Não salva imagem quando o tipo de retorno é base64
- Melhoria: Mudança no objeto de retorno (removendo campos path e base64 e adicionando campo imagem)
- Melhoria: Adicionado flag (configuracaoTexto) para receber os textos de customização

## [1.2.6] - 13-12-2021
- Melhoria: Atualizar SSL Pinning.

## [1.2.5] - 30-11-2021
- Melhoria: Corrgir layout de captura e subir nova versão para o Cocoapods.

## [1.2.4] - 30-11-2021
- Melhoria: Subir nova versão para o Cocoapods.

## [1.2.3] - 25-11-2021
- Melhoria: Refatorar lógica da captura manual.
- Melhoria: Customização do texto de solicitação de mudança de lado no e da confirmação (IOS).
- Melhoria: Alterar retorno do caminho das imagens no delegate.

## [1.2.2] - 23-11-2021
- Melhoria: Corrigir divergência da tela de informação na captura do doc.
- Melhoria: Atualizar repositório de demonstração do componente default com o lado AB liberado.
- Melhoria: Adicionado tela de preview e confirmação de captura.

## [1.2.1] - 17-11-2021
- Melhoria: Customização de fonte.
- Melhoria: Customização da tela de captura. 



