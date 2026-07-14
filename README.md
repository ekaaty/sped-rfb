# SPED-RFB
---

Este projeto tem como finalidade empacotar para distribuição para os diversos 
sistemas GNU/Linux os programas fornecidos pela Receita Federal do Brasil (RFB).

## Sistema Público de Escrituração Digital - SPED

O SPED, abreviação de **Sistema Público de Escrituração Digital** tem como 
objetivo unificar a recepção, validação, armazenamento e autenticação de livros
e documentos integrantes das escriturações contábil e fiscal das 
[pessoas jurídicas](
    https://pt.wikipedia.org/wiki/Pessoas_jur%C3%ADdicas "Pessoas jurídicas"
), através de um fluxo computadorizado de informações. O SPED também visa 
facilitar a fiscalização, integrando informações de interesse dos governos 
federal e estadual.

O projeto SPED é composto pelas seguintes escriturações:

- EFD – Escrituração Fiscal Digital;
    - [EFD ICMS/IPI](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/efd-icms-ipi);
    - [EFD PIS/COFINS (Contribuições)](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/efd-contribuicoes);
    - [EFD-Reinf](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/efd-reinf);
- [ECD – Escrituração Contábil Digital](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/ecd);
- [ECF – Escrituração Contábil Fiscal](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/ecf);
- [e-Financeira](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/e-financeira)
- [eSocial](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/esocial);
- [Central de Balanços](https://www.gov.br/sped/pt-br/assuntos/escrituracoes-digitais/central-de-balancos);

Acesse o [Portal do SPED no gov.br](https://www.gov.br/sped/pt-br) para mais
informações.

A Receita Federal do Brasil fornece aplicativos para a geração e validação de 
arquivos de transferência eletrônica para as escriturações do SPED de acordo com
a tabela a seguir:

|Componente               |Descrição                                    |
|-------------------------|---------------------------------------------|
|Sped EFD (Fiscal)        |Gerador de EFD ICMS/IPI                      |
|Sped EFD (Contribuições) |Gerador de EFD PIS/COFINS                    |
|Sped ECD (Contábil)      |Validador de ECD                             |
|Sped ECF (Contábil)      |Validador de ECF                             |

## Pré-requisitos

Antes de começar, verifique se o seu computador atende aos seguintes requisitos:
* Possui uma versão 64 bits do GNU/Linux instalada: `x86_64, amd64`. Para saber 
qual a sua arquitetura execute o seguinte comando:
    ```
    uname -a
    ```
* O seu sistema possui uma interface gráfica instalada: `KDE Plasma, Gnome, XFCE, etc.` 
* O seu sistema GNU/Linux está executando uma distribuição compatível:
    * [Fedora](https://getfedora.org)
    * [Ekaaty](https://ekaaty.com)
<!--
    * [Rocky Linux](https://rockylinux.org)(ainda não suportado)
    * [Alma Linux](https://almalinux.org)(ainda não suportado)
    * [Oracle Linux (OL)](https://www.oracle.com/br/linux/)(ainda não suportado)
    * [Amazon Linux (AL)](https://aws.amazon.com/amazon-linux/)(ainda não suportado)
-->

## Instalando os aplicativos SPED
Para instalar os aplicativos do SPED em sua máquina com GNU/Linux, siga estas etapas:

### Fedora e Ekaaty (usando DNF):
Execute os seguintes comandos em seu terminal para habilitar o repositório 
Copr e instalar as aplicações:

```bash
sudo dnf copr enable ekaaty/sped-rfb
sudo dnf install --refresh sped-*
```

