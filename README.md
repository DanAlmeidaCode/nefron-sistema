# Nefron Sistema

Sistema interno da **Clínica Néfron** (Dra. Macelle Rangel), clínica veterinária especializada em nefrologia e hemodiálise, em Vitória da Conquista - BA.

## Módulos

| Módulo | Status |
|---|---|
| [Prontuário](modulos/prontuario/) | ✅ Pronto e funcional |
| [Calculadora de precificação de consulta](modulos/calculadora-precificacao/) | ⏳ Pendente de definição |
| [Almoxarifado](modulos/almoxarifado/) | ⏳ Pendente de definição |
| [Passagem de plantão](modulos/passagem-plantao/) | ⏳ Pendente de definição |

Os módulos pendentes dependem de respostas da Dra. Macelle a um levantamento de requisitos em aberto. Ver detalhes no README de cada pasta.

### Prontuário

Formulário de internamento (dados do paciente, medicamentos com Oxigênio e Transfusão pré-carregados, máscara de telefone brasileiro) que gera um PDF client-side no layout da Clínica Néfron.

## Stack

- HTML/CSS/JS puro, sem framework, sem build step.
- PDF gerado no navegador com [html2canvas](https://html2canvas.hertzen.com/) + [jsPDF](https://github.com/parallax/jsPDF) (carregados via CDN).

## Como rodar localmente

Cada módulo é autocontido. Para o módulo de prontuário:

- Abra diretamente `modulos/prontuario/index.html` no navegador, ou
- Sirva a pasta com um servidor estático:

```bash
cd modulos/prontuario
python3 -m http.server
```

Depois acesse `http://localhost:8000`.
