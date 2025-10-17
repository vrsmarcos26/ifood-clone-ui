<div align="center">
  <h1>
    Clone da Interface do iFood (Tela Inicial)
  </h1>
</div>

<p align="center">
  <img alt="Tecnologia Principal" src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white">
  <img alt="Linguagem do Layout" src="https://img.shields.io/badge/XML-d9534f?style=for-the-badge&logo=android-studio&logoColor=white">
  <img alt="Licença" src="https://img.shields.io/github/license/vrsmarcos26/ifood-clone-ui?style=for-the-badge&color=blue">
</p>

<p align="center">
  Recriação da tela inicial do iFood, um desafio de UI para Android focado em componentes como CardViews, rolagem horizontal e vertical.
</p>

<p align="center">
  <a href="#-sobre-o-projeto">Sobre</a> •
  <a href="#-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-como-usar">Como Usar</a> •
  <a href="#-demonstração">Demonstração</a> •
  <a href="#-licença">Licença</a>
</p>

---

### 🎯 Sobre o Projeto

Este projeto é uma réplica da tela inicial do iFood, desenvolvido como um exercício prático para aprimorar minhas habilidades em design de interfaces no Android. O foco foi estruturar um layout complexo que combina diferentes tipos de visualização de dados, como banners, listas de categorias e cards de restaurantes, dentro de um `ScrollView` principal. Foi um projeto acadêmico que serve como uma excelente peça para meu portfólio de desenvolvimento mobile.

---

### 🛠️ Tecnologias Utilizadas

A interface foi construída utilizando as ferramentas padrão do desenvolvimento Android nativo.

<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/Android_Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white" alt="Android Studio"></a>
  <a href="#"><img src="https://img.shields.io/badge/XML-d9534f?style=for-the-badge&logo=android-studio&logoColor=white" alt="XML"></a>
  <a href="#"><img src="https://img.shields.io/badge/CardView-FF5722?style=for-the-badge" alt="CardView"></a>
</p>

---

### ⚙️ Como Usar

Para visualizar este layout:
1.  Crie um novo projeto no Android Studio.
2.  Copie o conteúdo do arquivo `ifood.xml` para o seu arquivo de layout principal (ex: `res/layout/activity_main.xml`).
3.  Na sua `MainActivity.kt` ou `MainActivity.java`, certifique-se de que o layout está sendo carregado: `setContentView(R.layout.activity_main)`.
4.  Execute o aplicativo em um emulador ou dispositivo físico.

---

### 🎬 Demonstração

<p align="center">
  <img src="print.png" alt="Print da interface do Spotify" width="600">
</p>

<summary><strong>💡 Análise da Estrutura do Layout (Write-up)</strong></summary>
<br>

A complexidade da tela inicial do iFood foi abordada com uma combinação estratégica de layouts para garantir a performance e a fidelidade visual:

1.  **Layout Raiz (`ScrollView`)**: Como a tela possui mais conteúdo do que cabe na vertical, um `ScrollView` foi usado como contêiner principal, permitindo a rolagem de toda a página. Dentro dele, um `ConstraintLayout` organiza as seções.

2.  **Barra Superior (Header)**: Fixada no topo, contém o endereço do usuário, um ícone de dropdown e o ícone de perfil. O `ConstraintLayout` facilita o alinhamento desses elementos.

3.  **Barra de Busca (`EditText`)**: Estilizada com cantos arredondados e um ícone para se assemelhar ao componente nativo do app.

4.  **Categorias (`HorizontalScrollView`)**: Uma lista de categorias rolável horizontalmente foi implementada com um `HorizontalScrollView` contendo `CardViews` ou `Buttons` para cada item (Restaurantes, Mercado, etc.).

5.  **Conteúdo Principal**:
    -   **Banners Promocionais**: Implementados com `CardView` para dar o efeito de elevação e cantos arredondados, contendo uma `ImageView`.
    -   **Cards de Restaurantes**: O elemento mais complexo. Cada restaurante é um `CardView` que agrupa vários `TextViews` (nome, avaliação, categoria, tempo, frete) e uma `ImageView` (logo). O `ConstraintLayout` dentro do card é ideal para posicionar esses múltiplos elementos de forma eficiente e responsiva.

6.  **Barra de Navegação Inferior (`LinearLayout`)**: Fixada na parte inferior, utiliza um `LinearLayout` horizontal com `layout_weight` para garantir que os itens (Início, Busca, Pedidos, Perfil) ocupem o mesmo espaço.


---

### 📝 Licença

Este projeto está sob a licença MIT.

<hr>

<p align="center">
  Desenvolvido por <b>Marcos Vinícius Rocha Silva</b>
</p>
