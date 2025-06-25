# 🛒 Lista de Compras (React Native) 🚀

![Badge](https://img.shields.io/badge/React_Native-blue?style=flat-square\&logo=react)
![Badge](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square\&logo=typescript)
![Badge](https://img.shields.io/badge/Expo-000020?style=flat-square\&logo=expo)
![Badge](https://img.shields.io/badge/AsyncStorage-32CD32?style=flat-square\&logo=android)

Bem-vindo ao seu novo ajudante de compras! 📝 Este aplicativo super prático foi criado na formação React Native da Rocketseat.

## 🎉 Funcionalidades Incríveis

* ✅ **Adicione Itens:** Nunca mais esqueça de comprar algo!
* 🎯 **Marque como Comprado:** Aquele prazer de completar sua lista!
* ❌ **Remova Itens:** Algo a mais ou errado? Sem problemas!
* 🔄 **Filtre Itens:** Veja rapidamente o que falta e o que já comprou.
* 💾 **Salve Automaticamente:** Seus itens estão seguros com AsyncStorage.

## 📹 Demonstração

![Lista de Compras - Demonstração](comprar.mp4)

## 📁 Estrutura do Projeto

```plaintext
src
├── app
│   └── Home
├── assets
│   ├── logo.png
│   ├── logo@2x.png
│   └── logo@3x.png
├── components
│   ├── Button
│   ├── Filter
│   ├── Input
│   ├── Item
│   └── StatusIcon
├── storage
│   └── itemsStorage.ts
└── types
    └── FilterStatus.ts
```

## 🛠️ Instalação Rápida

Clone o projeto:

```bash
git clone <URL_DO_REPOSITORIO>
cd lista-compras-react-native
```

Instale tudo:

```bash
npm install
```

Inicie o App:

```bash
npm run start
# ou
expo start
```

## 📚 Estrutura de Dados

```typescript
type ItemsStorage = {
  id: string;
  status: FilterStatus;
  description: string;
};

enum FilterStatus {
  PENDING = 'pending',
  DONE = 'done',
}
```

## 💾 Persistência

Guarda os dados localmente no seu celular usando AsyncStorage.

## 📖 Conceitos Aplicados

### ⚛️ React Native

Framework para desenvolvimento de aplicativos móveis usando JavaScript e React. Permite criar apps nativos para Android e iOS a partir de uma única base de código.

**Exemplo:** Criar componentes visuais, como botões e listas, usando elementos do React Native como `TouchableOpacity`, `FlatList` e `TextInput`.

### 📘 TypeScript

É um superconjunto do JavaScript que adiciona tipagem estática e interfaces claras ao código, facilitando a manutenção e a detecção de erros antes da execução.

**Exemplo:**

```typescript
type ItemsStorage = {
  id: string;
  status: FilterStatus;
  description: string;
};
```

### 🚀 Expo

Ferramenta e plataforma que facilita o desenvolvimento de aplicativos React Native ao fornecer uma série de funcionalidades integradas, facilitando testes, build e deploy.

**Exemplo:** Executar o aplicativo rapidamente usando `expo start`.

### 💾 AsyncStorage

É uma solução de armazenamento persistente local para aplicativos React Native. Armazena dados no dispositivo do usuário.

**Exemplo:**

```typescript
await AsyncStorage.setItem("@comprar:items", JSON.stringify(items));
const items = await AsyncStorage.getItem("@comprar:items");
```

Estes conceitos tornam a aplicação prática, fácil de manter e altamente escalável.
