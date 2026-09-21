# Técnico Persianas — Site (redesign)

Site institucional de uma página para a Técnico Persianas (fábrica de persianas e cortinas), em HTML5, CSS3 e JavaScript puro — sem frameworks, pronto para hospedagem estática (GitHub Pages, Netlify, Vercel etc.).

## Estrutura

```
tecnico-persianas/
├── index.html
├── css/
│   └── style.css
├── js/
│   └── main.js          # abre/fecha o menu no mobile
├── assets/
│   ├── logo/
│   │   └── logo.png     # logo enviado pelo cliente
│   └── images/
│       └── *.jpg        # fotos dos 8 modelos de persiana rolô
└── README.md
```

## Ver localmente

Não precisa de build nem de servidor — basta abrir o `index.html` no navegador.
Se preferir um servidor local (recomendado para testar os caminhos de imagem):

```bash
cd tecnico-persianas
python3 -m http.server 8000
# depois abra http://localhost:8000
```

## Publicar no GitHub Pages

1. Crie um repositório novo e suba esta pasta (o conteúdo, não a pasta em si, deve ficar na raiz ou em `/docs`).
2. No GitHub: **Settings → Pages → Source**, selecione a branch (ex. `main`) e a pasta (`/root` ou `/docs`).
3. O site fica disponível em `https://<usuario>.github.io/<repositorio>/`.

## Conteúdo já confirmado

- Identidade visual: preto + dourado, a partir do logo enviado pelo cliente.
- Serviços, horário de atendimento, WhatsApp e Instagram: extraídos do site atual (tecnicopersianas.com.br).
- Fotos dos 8 modelos de persiana rolô: enviadas pelo cliente.
- Fotos de 6 projetos/instalações reais, na seção **Projetos realizados**: enviadas pelo cliente; as legendas (cômodo + tipo de persiana) foram escritas a partir do que aparece em cada foto.

## Ainda pendente de confirmação com o cliente

- O depoimento da seção **Depoimentos** está resumido nas palavras da equipe — confirmar se pode ir na íntegra ou se o resumo atual está aprovado.
- Não há endereço físico no site atual; se a empresa quiser exibir um, falta esse dado.
- Favicon usa o logo enviado; se o cliente tiver um ícone quadrado dedicado, pode substituir `assets/logo/logo.png`.

## Personalização rápida

- Cores: variáveis no topo de `css/style.css` (`--gold`, `--bg`, `--surface` etc.).
- Textos: direto no `index.html`, por seção.
- WhatsApp: número está fixo em `https://api.whatsapp.com/send?phone=5511970940242` em três lugares (header, hero, contato e botão flutuante) — buscar e substituir se mudar.
