# Hospital Defense

## Curso Técnico de Desenvolvimento de Sistemas — Senai Itapeva

**Hospital Defense** é um jogo educativo de Cyber Defense ambientado em uma unidade hospitalar. O jogador inspeciona dispositivos IoT conectados, compara as configurações observadas com padrões recomendados, identifica vulnerabilidades e aplica correções.

O cenário e as falhas são simulados para fins didáticos. O jogo não se conecta a equipamentos ou redes hospitalares reais.

---

## Demonstração

O jogo apresenta uma UTI modelada em 3D, com equipamentos médicos identificados por marcadores destacados. O ambiente pode ser girado em 360° e explorado com zoom.

Ao selecionar um dispositivo, a inspeção abre em tela cheia. O modelo ampliado aparece ao lado da referência recomendada e do desafio interativo daquele equipamento. A comparação mostra a leitura atual e o padrão seguro correspondente.

---

## Funcionalidade Principal: Inspeção e Proteção de Dispositivos IoT

### Objetivo

Inspecionar os sete dispositivos conectados à UTI, concluir o desafio específico de cada aparelho, identificar os três vulneráveis e corrigir suas falhas.

### Dispositivos simulados

- **Monitor cardíaco:** análise de tráfego criptografado.
- **Bomba de infusão INF-02:** inspeção da versão do firmware.
- **Ventilador pulmonar:** seleção do segmento de rede adequado.
- **Bomba de infusão PMP-04:** auditoria de credenciais padrão.
- **Gateway IoT:** identificação da porta de diagnóstico exposta.
- **Tablet clínico:** verificação da criptografia do armazenamento.
- **Sensor ambiental:** validação de assinatura digital.

Três equipamentos já estão protegidos. Os outros três apresentam falhas simuladas de firmware, credenciais ou exposição de serviço. O jogador precisa analisar as informações antes de classificar cada dispositivo.

### Fluxo de jogo

1. Selecione um equipamento no mapa 3D ou no inventário.
2. Gire e aproxime o modelo para inspecionar o aparelho.
3. Compare a leitura observada com o padrão recomendado.
4. Resolva o minijogo específico e identifique o estado do dispositivo.
5. Isole e corrija os dispositivos vulneráveis.

---

## Funcionalidades

1. **Hospital 3D interativo**
   - Cenário de UTI com dispositivos IoT e equipamentos médicos.
   - Rotação do ambiente e controle de zoom.
   - Marcadores clicáveis para identificar os nós da rede.

2. **Modo de inspeção em tela cheia**
   - Centraliza o dispositivo selecionado.
   - Exibe o modelo 3D ao lado da referência segura.
   - Apresenta a leitura observada e a configuração recomendada.
   - Permite retornar ao mapa ou sair com a tecla **Esc**.

3. **Minijogos de análise**
   - Cada dispositivo tem um desafio relacionado à sua função e ao controle de segurança analisado.
   - Os desafios abordam tráfego TLS, firmware, segmentação de rede, credenciais, portas de serviço, criptografia e assinaturas digitais.

4. **Resposta a incidentes**
   - Painel de inventário e indicadores de ameaças, correções e integridade da rede.
   - Ação para isolar e corrigir os dispositivos vulneráveis.
   - Opção para reiniciar a simulação.

---

## Tecnologias Utilizadas

- **HTML5** — estrutura da aplicação.
- **Tailwind CSS** — estilos e componentes visuais, carregado via CDN.
- **JavaScript ES Modules** — lógica do jogo e interações.
- **Three.js** — renderização do hospital e dos aparelhos em 3D.
- **OrbitControls** — rotação e zoom do cenário e dos dispositivos.
- **CSS2DRenderer** — marcadores interativos sobre o mapa 3D.
- **SVG** — ilustrações de referência geradas pela aplicação.

---

## Estrutura de Arquivos

```text
Hospital-Defense/
|-- index.html   # Jogo completo: interface, estilos, modelos e lógica
|-- README.md    # Documentação do projeto
```

---

## Como Executar

### Pré-requisitos

- Navegador moderno, como Google Chrome, Microsoft Edge ou Mozilla Firefox.
- Conexão com a internet para carregar Tailwind CSS e Three.js via CDN.

### Execução local

1. Abra a pasta do projeto no Visual Studio Code.
2. Inicie um servidor local, por exemplo, usando a extensão **Live Server**.
3. Abra o endereço local indicado pelo servidor.

Também é possível iniciar um servidor estático com Python a partir da pasta do projeto:

```bash
python -m http.server 8000
```

Depois, acesse `http://localhost:8000` no navegador. Um servidor local é recomendado porque a página utiliza módulos JavaScript ES Modules.

---

## Competências Desenvolvidas

- Conceitos de segurança cibernética aplicados a ambientes IoT.
- Identificação de configurações inseguras e comparação com padrões recomendados.
- Noções de firmware, criptografia, segmentação de rede, credenciais e assinaturas digitais.
- Desenvolvimento de interfaces interativas com HTML, CSS e JavaScript.
- Criação de ambientes e interações 3D com Three.js.
- Design de experiências educativas baseadas em desafios.

---

## Autoras

Projeto desenvolvido por:

- **Lorena Rinaldo Moreira** — [LinkedIn](https://www.linkedin.com/in/lorena-rinaldo01/)
- **Isabelly Ferreira de Lima** — [LinkedIn](https://www.linkedin.com/in/isabelly-ferreira-42a54837b/)

**Instituição:** Curso Técnico de Desenvolvimento de Sistemas — **Senai Itapeva**
