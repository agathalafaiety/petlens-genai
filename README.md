# PetLens

**PetLens é uma ferramenta experimental que explora o uso da Inteligência Artificial Generativa do Google para fornecer soluções inovadoras para donos de pets.** 🐾

<br>

<p align="center">
  <img src="dogia.jpg" alt="PetLens - Cão Robótico com Interface Tecnológica" width="300">
   <img src="gatoia.jpg" alt="PetLens - Gato Robótico com Interface Tecnológica" width="300">
</p>
</p>
<p align="center">
  <em>Imagem gerada por inteligência artificial, representando a integração de tecnologia no cuidado pet.</em>
</p>

<br>

## O PetLens busca oferecer soluções para os seguintes desafios:

* **Diagnóstico Auxiliado por IA:** A preocupação com os primeiros sinais de doença é frequente. O PetLens propõe um sistema onde os tutores podem descrever os sintomas iniciais de seus pets (como tosse, falta de apetite, manchas na pele) e receber possíveis diagnósticos diferenciais gerados pelo Gemini. É crucial ressaltar que esta funcionalidade tem como objetivo fornecer uma primeira orientação e **não substituir a consulta com um veterinário**, mas sim ajudar o dono a entender a urgência da situação.

* **Personalização de Cuidados Preventivos:** Cada pet possui necessidades únicas. O PetLens visa criar um sistema que, baseado em informações específicas como raça, idade, histórico médico e até mesmo localização geográfica (considerando riscos de doenças regionais), possa gerar um plano de cuidados preventivos personalizado, incluindo sugestões de vacinação, vermifugação e exames específicos.

* **Enriquecimento Ambiental Personalizado:** Promover o bem-estar mental e físico dos pets é essencial. O PetLens ambiciona utilizar dados como raça, idade, nível de energia e histórico de comportamento para sugerir ideias criativas de enriquecimento ambiental, como brinquedos, atividades interativas e adaptações no ambiente doméstico.

* **Localização Inteligente de Serviços Pet-Friendly:** Encontrar serviços adequados para as necessidades específicas de um pet pode ser desafiador. O PetLens propõe um sistema que compreenda as necessidades detalhadas do usuário (por exemplo, "veterinário com atendimento de emergência para gatos perto de mim" ou "parque que permite cachorros grandes com área de agility") e forneça resultados relevantes com informações adicionais como horários de funcionamento e avaliações de outros usuários.

##

### Iniciativa do projeto

O projeto foi criado como entrega do desafio proposto durante a imersão de IA com o Google Gemini promovida pela Alura e pelo Google.

<p align="center">
  <img src="alura.png" alt="alura" width="300">
</p>

### Ferramentas ultilizadas 

* Google AI Studio
* Google Gemini
* Google Colab

# PetLens - Guia de Uso

Siga estes passos para configurar e executar o projeto utilizando o Google Colab:

**1. Obter Chave de API do Google Gemini:**

* Acesse o [Google AI Studio](https://makersuite.google.com/app/apikey).
* Crie ou selecione um projeto e gere uma chave de API.
* Copie e guarde esta chave de forma segura. **Importante:** Não compartilhe sua chave de API publicamente.

**2. Configurar o Ambiente no Google Colab:**

* Abra um novo notebook no [Google Colab](https://colab.research.google.com/).
* Você precisará instalar a biblioteca do Google Generative AI. Execute a seguinte célula de código no seu notebook:

    ```python
    !pip -q install google-genai
    ```

* Após a instalação, você precisará configurar sua chave de API. Execute a seguinte célula, **substituindo `"SUA_CHAVE_DE_API"` pela chave que você obteve no Google AI Studio:**

    ```python
    import os
    from google.colab import userdata

    os.environ["GOOGLE_API_KEY"] = userdata.get('GOOGLE_API_KEY')

    ```

    **Nota:** Mantenha sua chave de API em segredo. Uma prática comum é armazená-la como uma variável de ambiente, mas para simplicidade neste guia inicial no Colab, a configuração direta é mostrada. Para projetos mais robustos, explore métodos mais seguros de gerenciamento de chaves.

