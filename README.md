# Chapada Diamantina — Guia de Campo (versão instalável)

App para usar no celular **sem internet** durante a travessia do Vale do Pati:

- relevo 3D com imagem de satélite, trilhas, rios, casas de apoio e lugares;
- **GPS ao vivo** (ponto azul), com rumo e distância até um destino e aviso quando você se afasta da trilha mapeada;
- **gravação do caminho de cada dia** (exporta em GPX);
- **fotos com localização** e **álbum da viagem**, organizado por dia (exporta como uma página HTML);
- guia com fotos de bichos, plantas e pedras, e o modo "percorrer" da trilha.

Tudo o que você gravar (fotos e caminhos) fica guardado **só no seu celular**.

## Publicar no GitHub Pages (uma vez, uns 5 minutos)

O GPS e o uso sem internet só funcionam com um endereço **https**. O GitHub Pages fornece esse endereço de graça.

1. Crie um repositório público no GitHub, por exemplo `pati`.
2. Envie **o conteúdo desta pasta** (não a pasta em si) para a branch `main`:
   ```bash
   cd pwa
   git init && git add . && git commit -m "Guia Chapada Diamantina"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/pati.git
   git push -u origin main
   ```
   Pelo site também dá: em **Add file → Upload files**, arraste todos os arquivos e pastas.
3. No repositório, abra **Settings → Pages**. Em *Source*, escolha **Deploy from a branch**, depois `main` e `/ (root)`, e salve.
4. Em 1 a 2 minutos o app estará em `https://SEU_USUARIO.github.io/pati/`.

## Instalar no celular (ainda com internet, antes da viagem)

1. Abra o endereço no **Safari** (iPhone) ou no **Chrome** (Android).
2. Espere aparecer, na tela inicial do app, **"✓ Pronto para usar sem internet"**. Ele baixa cerca de 12 MB.
3. Instale na tela inicial:
   - **iPhone:** Compartilhar ⬆ → **Adicionar à Tela de Início**.
   - **Android:** ⋮ → **Instalar app**.
4. Abra uma vez **pelo ícone instalado**, entre em *Mapa 3D → Vale do Pati* e toque no botão de GPS para liberar a localização.
5. Teste: ative o modo avião e abra o app. Tudo deve funcionar.

> No iPhone, o app instalado e o Safari guardam os dados separadamente. Use sempre **pelo ícone**, para as fotos e os caminhos ficarem juntos.

## Na trilha

- **Trecho de hoje** (na tarja do GPS): escolha o percurso do dia. O app mostra quanto falta (km, subida e tempo), qual o próximo ponto e avisa se você sair do trecho.
- **Pôr do sol** e **água mais perto** aparecem no painel do GPS, calculados sem internet.
- **🆘 Emergência:** mostra suas coordenadas em letra grande e prepara um SMS com a localização.

- **Botão de GPS** (alvo azul, no mapa): mostra onde você está. Toque de novo para o mapa seguir você.
- **Tarja escura no topo do mapa:** toque para escolher um destino (ex.: Prefeitura), ligar **Gravar meu caminho** e **Manter a tela ligada**.
- **Botão laranja de câmera:** tira a foto e já a coloca no mapa e no álbum. Escreva uma legenda na hora.
- Fotos tiradas com a câmera normal do celular entram depois, em **Álbum → Adicionar da galeria**. O app usa a localização da própria foto ou, se ela não tiver, a do caminho gravado no mesmo horário. Se nada disso existir, você toca no mapa para marcar o lugar.

### Usar o relógio para gravar o caminho
**Huawei (GT 6):** grave como *Caminhada ao ar livre*. No app Huawei Health, abra o treino → ícone de rota à direita do mapa → *Exportar rota* → GPX → Salvar em Arquivos. Teste antes da viagem.

**Levar a trilha para o relógio:** em **Trilhas**, cada trecho tem **⌚ Levar para o relógio**. Salve o GPX e importe no Huawei Health (Eu → Minhas rotas → Importar rota → Enviar para o relógio). No relógio, a trilha aparece em Exercício → Caminhada ao ar livre → Rotas, e funciona sem celular.

O relógio grava o dia inteiro com a tela do celular apagada e gasta menos bateria. Ao fim do dia, ou na volta, exporte a atividade em **GPX ou TCX** (pelo Garmin Connect, pelo Strava, ou pelo HealthFit no caso do Apple Watch) e toque em **Álbum → ⌚ Importar caminho do relógio**. O app separa os pontos por dia, usa o caminho do relógio no lugar do gravado pelo celular e posiciona sozinho as fotos sem localização, comparando os horários.

### Limites que é bom saber
- O navegador **só grava o caminho com o app aberto e a tela ligada**. Para gravar o dia inteiro com a tela apagada, use junto um app de trilha (Organic Maps, Wikiloc ou Strava). Depois é só importar as fotos da galeria: o app as posiciona pela localização gravada na foto.
- O iPhone às vezes remove a localização das fotos escolhidas pela galeria. As fotos tiradas **pelo botão do app** usam o GPS do momento e não têm esse problema.
- Os dados ficam no navegador do celular. **Exporte o álbum e o GPX ao fim de cada dia ou da viagem** para não correr o risco de perder nada se o navegador limpar o armazenamento.
- Traçados e distâncias são aproximados. Não substituem o guia credenciado.

## Localização do grupo (aba Grupo)
1. **Antes de sair, com internet, todos juntos:** uma pessoa toca em **Grupo → Criar grupo** e aparece um QR na tela. Os outros abrem o app → **Grupo → 📷 Escanear o QR**, apontam para a tela e digitam o nome. Pronto, sem código.
2. **Família:** toque em **Link para a família**. A pessoa aponta a câmera do celular para o QR, ou você manda o link pelo WhatsApp. Ela vê no mapa 3D o último local de cada um, os recados e um alerta vermelho se alguém pedir ajuda.
3. Daí para frente é automático: a posição, o caminho, o **trecho do dia** escolhido no GPS e o **caminho do relógio** importado no álbum vão sozinhos para o grupo.

Como funciona sem sinal: o celular guarda o caminho e os recados e **envia tudo sozinho quando pegar internet** (na saída do vale, numa cidade, num Wi-Fi). Só envia com o app aberto. Andando com internet, manda a posição a cada 3 minutos; parado, uma vez por hora.

- **📍 Mandar minha posição:** abre o WhatsApp, SMS ou iMessage com a sua posição e um link. Quem abrir o link com internet vê você no mapa 3D e, se estiver no grupo, repassa a posição para todos. É assim que o **Vivo Satélite** (Starlink) ajuda: ele libera só apps de mensagem e mapas, não o navegador.
- **Satélite do iPhone** (SOS e Buscar via satélite): ainda não funciona no Brasil.
- Para se acharem dentro do vale sem internet nenhuma: rádios comunicadores ou aparelhos Meshtastic (LoRa, 915 MHz).
- Privacidade: tudo sai do celular criptografado com o código do grupo e passa pelo serviço gratuito ntfy.sh, que guarda por até 12 h. O serviço aceita cerca de 250 envios por dia por internet; num Wi-Fi dividido com muita gente pode bater o limite, e o app avisa e tenta de novo depois.

Se eu gerar uma versão nova, substitua os arquivos no repositório. O app se atualiza sozinho na próxima vez que abrir com internet. Fotos e caminhos já gravados são mantidos.

## Créditos dos dados
Relevo Copernicus GLO-30 (© DLR e.V. / Airbus, fornecido pela UE/ESA); imagem Sentinel-2 cloudless 2020 da EOX; trilhas, rios e lugares © colaboradores do OpenStreetMap (ODbL); geologia e hidrogeologia do Serviço Geológico do Brasil; fotos do Wikimedia Commons e do iNaturalist (autores e licenças no botão "Créditos" do app).
