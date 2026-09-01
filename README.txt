GENPOP SIM — PROTÓTIPO 0.1

O que há nesta versão
- Deriva genética (Wright–Fisher) com N, p0, gerações, réplicas/loci, fixação/perda e tempo até o evento.
- Seleção natural dialélica com WAA, WAa e Waa, seis frequências iniciais, frequências genotípicas e fitness médio.
- Estrutura populacional e migração com demes, N por deme, m, HS, HT e FST ao longo das gerações.
- Comparação N x m para o desenho do estudo dirigido.
- Seleção + deriva, com várias réplicas e matriz N x força de seleção.
- Seleção multialélica (A, B, C) com seis valores adaptativos.
- Exportação CSV.
- Presets dos estudos dirigidos.
- Sem bibliotecas externas e sem coleta de dados.

TESTE IMEDIATO NO COMPUTADOR
1. Extraia o ZIP.
2. Abra index.html no navegador.
3. Todas as simulações funcionam mesmo sem internet.

INSTALAÇÃO COMO APP (PWA) EM ANDROID / iOS
Para o sistema oferecer "Instalar" / "Adicionar à Tela de Início", os arquivos precisam ser abertos a partir de um endereço HTTPS (ou localhost durante desenvolvimento). Isso é uma exigência dos navegadores para PWA; não é uma dependência do simulador.

Depois de instalada e de o cache ser criado, esta versão funciona offline.

Android (Chrome/Edge): menu do navegador > Instalar aplicativo / Adicionar à tela inicial.
iPhone/iPad (Safari): Compartilhar > Adicionar à Tela de Início.

IMPORTANTE
Este ZIP é uma PWA e não é um APK nem um IPA assinado. A geração de APK/IPA nativos exige empacotamento e, no caso do iOS, assinatura/certificado Apple. O protótipo foi entregue primeiro como PWA para permitir testar a lógica e solicitar alterações antes de gerar uma versão de distribuição.

MODELOS
- Deriva: amostragem binomial de 2N cópias gênicas por geração.
- Seleção: seleção por viabilidade sob acasalamento aleatório.
- Estrutura: modelo-ilha com migração simétrica, seguida por deriva em cada deme.
- FST: (HT-HS)/HT a partir das frequências alélicas entre demes.
- Seleção + deriva: seleção por viabilidade, seguida por amostragem Wright–Fisher.
