# Simulador SMK-37 Pro

Simulador de treino em navegador para o teclado controlador M-VAVE SMK-37 Pro. O projeto é uma página HTML autônoma: não usa framework, instalação de pacotes ou serviço remoto para carregar a interface.

## Estado do projeto

Protótipo em desenvolvimento. A interface permite tocar notas por mouse/toque e teclado do computador, produzir som demonstrativo com Web Audio, gravar áudio do microfone no navegador, usar MIDI Web quando suportado, praticar escalas/acordes e experimentar arpejador e sequenciador.

A síntese FM é ilustrativa e não reproduz o motor interno do instrumento. Não foram confirmados nem extraídos do firmware original os menus, a tabela de patches, algoritmos FM ou mapa detalhado dos controles. Não use o simulador como documentação oficial do SMK-37 Pro.

## Executar

1. Baixe ou clone o repositório.
2. Abra `index.html` em um navegador moderno.
3. Pressione **Ativar áudio** antes de tocar.
4. Para gravar o microfone, escolha **Gravar microfone** e permita o acesso quando o navegador perguntar. A gravação permanece no navegador até baixar o arquivo.
5. Para usar Web MIDI, conecte o dispositivo e escolha **Conectar MIDI USB**. O suporte depende do navegador e das permissões disponíveis.

Se o navegador bloquear microfone ou MIDI ao abrir o arquivo diretamente, sirva a pasta por `localhost` ou HTTPS. Não há etapa de build.

## Tecnologias

- HTML, CSS e JavaScript sem bibliotecas externas.
- Web Audio API para som demonstrativo.
- MediaDevices e MediaRecorder para gravação local do microfone.
- Web MIDI API quando disponível.

## Contribuir

Leia [CONTRIBUTING.md](CONTRIBUTING.md) antes de abrir uma issue ou pull request. Relatos de segurança devem seguir [SECURITY.md](SECURITY.md).

## Licença e materiais visuais

A licença ainda aguarda aprovação do mantenedor. O painel incorpora arte vetorial fornecida durante o desenvolvimento; os direitos de redistribuição dessa arte precisam ser confirmados antes de uma publicação pública. O nome e a marca M-VAVE pertencem aos seus respectivos titulares.
