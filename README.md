# NBC · Cadastro de Atletas

### Gestão de cadastros para o Novo Basquete Carmo

Aplicação web para cadastrar e gerenciar informações de atletas, com atualização em tempo real via Cloud Firestore e exportação em PDF.

## Funcionalidades

- Cadastro, listagem, edição e exclusão de atletas.
- Campos de identificação, contato e informações esportivas.
- Máscaras para preenchimento de CPF, CEP e telefone.
- Cálculo de idade a partir da data de nascimento.
- Exportação da lista de atletas em PDF.

## Tecnologias

**React 19 · TypeScript · Vite · Tailwind CSS · Firebase / Firestore · jsPDF**

## Executar localmente

Pré-requisitos: Node.js compatível com Vite 7 (20.19+ ou 22.12+), npm e um projeto Firebase para desenvolvimento.

```bash
git clone https://github.com/JoaoMFserafim/MembrosCadasgtroNBC.git
cd MembrosCadasgtroNBC
npm ci
```

Antes de iniciar, configure `firebase.ts` com um projeto de desenvolvimento próprio e habilite o Cloud Firestore. O serviço de persistência usa a coleção `atletas`.

```bash
npm run dev
```

Abra o endereço informado pelo Vite.

| Comando | Finalidade |
| --- | --- |
| `npm run dev` | Desenvolvimento local |
| `npm run build` | Verificação TypeScript e build |
| `npm run preview` | Prévia do build |
| `npm run lint` | Análise estática |

## Organização

```text
src/
├── Pages/Cadastro/  # Interface de cadastro e listagem
├── Types/           # Tipos dos atletas
└── services/        # Integração com Firestore
firebase.ts          # Inicialização do Firebase
```

## Demonstração e dados

Para demonstrações de portfólio, utilize somente dados fictícios e um banco de desenvolvimento. O formulário contém campos pessoais; o acesso aos registros depende das regras e da configuração do Firestore.

---

Desenvolvido por [JoaoMFserafim](https://github.com/JoaoMFserafim).
