<p align="center">
  <img src="assets/banner.png" alt="WCS Gold Set" width="100%">
</p>

<p align="center">
  <a href="https://github.com/LeoDG20/wcs-gold-set-releases/releases/latest"><img alt="Versão" src="https://img.shields.io/github/v/release/LeoDG20/wcs-gold-set-releases?label=vers%C3%A3o&color=F59E0B&style=flat-square"></a>
  <a href="https://github.com/LeoDG20/wcs-gold-set-releases/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/LeoDG20/wcs-gold-set-releases/total?label=downloads&color=F59E0B&style=flat-square"></a>
  <img alt="Windows 10 e 11" src="https://img.shields.io/badge/Windows-10%20%7C%2011-1f2937?style=flat-square">
  <img alt="Assinatura Ed25519" src="https://img.shields.io/badge/atualiza%C3%A7%C3%A3o-assinada%20Ed25519-1f2937?style=flat-square">
</p>

<p align="center">
  <a href="https://github.com/LeoDG20/wcs-gold-set-releases/releases/latest"><b>⬇&nbsp; Baixar a versão mais recente</b></a>
</p>

Mede a **concordância entre versões de segmentação** do [Whisper Corpus Studio](https://github.com/LeoDG20/whisper-corpus-studio-releases/releases/latest): cada pessoa segmenta os mesmos áudios, manda sua versão (TextGrids do Praat) e o programa mostra, sem planilha, onde as versões concordam e onde divergem.

## Recursos

- **Versões:** importe um `.zip` exportado pelo WCS, uma pasta de TextGrids ou arquivos soltos.
- **Concordância:** nota de 0 a 100, erro médio das fronteiras (ms), acerto dentro da tolerância, viés e rótulos iguais.
- **Detalhamento:** por áudio, por fronteira e por transição de fonemas; com três ou mais versões, todas contra todas.
- **Exportação:** relatório em Markdown, CSV e JSON, e um pacote de TextGrids para importar de volta no WCS.

## Instalação

1. Em [Releases](https://github.com/LeoDG20/wcs-gold-set-releases/releases/latest), baixe **`WCS-Gold-Set-Setup-<versão>.exe`**.
2. Execute o instalador. Requer Windows 10 ou 11 (64 bits); não precisa de administrador.
3. Se aparecer *“O Windows protegeu o computador”*, clique em **Mais informações → Executar assim mesmo** (veja a pergunta abaixo).

## Atualização automática e segurança

O programa instalado verifica este repositório e se atualiza sozinho, baixando apenas o que mudou. Antes de aplicar qualquer arquivo ele confere a **assinatura Ed25519** contra a chave pública embutida nele; arquivo sem assinatura válida é recusado. A chave privada fica apenas com o autor e nunca é publicada.

## Perguntas frequentes

<details>
<summary><b>Por que o Windows mostra um aviso ao instalar?</b></summary>

O instalador não usa certificado comercial de editor, então o SmartScreen avisa para qualquer programa novo. A autenticidade é garantida pela assinatura Ed25519 descrita acima. Clique em **Mais informações → Executar assim mesmo**.

</details>

<details>
<summary><b>Os parâmetros calibrados aqui chegam ao WCS?</b></summary>

Sim: o autor os publica como pacote assinado no canal de parâmetros do WCS, que os aplica ao auto-segmentar.

</details>

<details>
<summary><b>Como desinstalo?</b></summary>

Em **Configurações do Windows → Aplicativos → Aplicativos instalados**.

</details>

<details>
<summary><b>Para que servem os outros arquivos de cada release?</b></summary>

Só o instalador (`Setup.exe`) interessa a quem instala. `manifest.json`, `package.zip`, `patch.zip` e os arquivos `.sig` são usados pela atualização automática e pela verificação de assinatura.

</details>

## Programas da família

| Programa | Função | Download |
| --- | --- | --- |
| Whisper Corpus Studio | Curadoria do corpus: segmentar, revisar e exportar o dataset. | [Baixar](https://github.com/LeoDG20/whisper-corpus-studio-releases/releases/latest) |
| WCS-Net Trainer | Treino das redes neurais a partir do dataset exportado pelo WCS. | [Baixar](https://github.com/LeoDG20/wcs-net-trainer-releases/releases/latest) |
| **WCS Gold Set** | Concordância entre versões de segmentação (você, orientador, colegas). | [Baixar](https://github.com/LeoDG20/wcs-gold-set-releases/releases/latest) |

---

<sub>Repositório de distribuição: o código-fonte é privado. Dúvidas ou problemas: abra uma <a href="https://github.com/LeoDG20/wcs-gold-set-releases/issues">issue</a>.<br>
© 2026 Leo Gobbi · uso acadêmico (TCC/IC).</sub>
