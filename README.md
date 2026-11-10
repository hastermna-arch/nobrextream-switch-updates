# Nobrextream Switch — atualizações oficiais

Este repositório público distribui **somente versões aprovadas** do Nobrextream para Nintendo Switch desbloqueado. O desenvolvimento permanece em um repositório privado separado.

## Como funcionam as atualizações

O aplicativo consulta o arquivo `latest.json` na branch `main` por HTTPS. Para cada versão publicada, a página de **Releases** oferece:

- `nobrextream.nro` — aplicativo homebrew;
- `SHA256SUMS.txt` — hash de integridade do binário;
- `nobrextream-corresponding-source.tar.gz` — código-fonte correspondente, conforme GPL-3.0.

O arquivo `latest.json` é publicado **somente depois** da compilação e da verificação automática do pacote. O aplicativo compara a versão, solicita sua confirmação, baixa o NRO, valida tamanho e SHA-256 e mantém uma cópia anterior como `nobrextream.nro.previous` antes da substituição.

**O canal só estará ativo quando houver um Release e o respectivo `latest.json`.** A simples criação deste repositório não ativa as atualizações.

## Instalação inicial e recuperação

Copie o `nobrextream.nro` aprovado para `/switch/nobrextream/nobrextream.nro` pelo seu método habitual. Após instalar uma versão com atualizador, use **Configurações → Ferramentas → Atualizações do Nobrextream** no próprio aplicativo.

Caso uma atualização impeça a abertura do programa, restaure manualmente `nobrextream.nro.previous` pelo DBI ou pelo leitor de cartão. A interface do Switch utiliza português brasileiro; A confirma e B volta.

## Privacidade e licença

Este repositório **não hospeda** listas M3U, contas Xtream, PINs, senhas, tokens pessoais ou conteúdos audiovisuais. Utilize somente fontes de mídia autorizadas.

O aplicativo deriva de [IPTV Player](https://github.com/murat303/iptv-player), licenciado sob GPL-3.0, com adaptações para Nobrextream Switch. Os pacotes distribuídos devem acompanhar o código-fonte correspondente e as informações de licença.
