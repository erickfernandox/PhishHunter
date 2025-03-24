# DPhishHunter

### Ferramenta de Geração Combinatoria e Verificação de Possiveis Domínios para Detecção Preventiva de Phishing

### Funcionalidades
- Geração automática de domínios suspeitos usando combinações de palavras.
- Verificação de registro WHOIS para detectar domínios recentemente criados.
- Testes de conectividade para determinar se os domínios estão online.
- Verificação automática de subdomínios relevantes.
- Extração do título da página para identificação visual rápida.

### Requisitos
Para utilizar o **DPhishHunter**, você precisa ter instalado:
- Python 3.x
- Pacotes necessários:
  ```bash
  pip install requests beautifulsoup4 whois dns.resolver colorama
  ```

### Instalação
```bash
git clone https://github.com/seu-usuario/DPhishHunter.git
cd DPhishHunter
pip install -r requirements.txt
```

### Como Usar
Para rodar o script, utilize o seguinte comando:
```bash
python phishhunter.py -p inscricoes,concurso,2025,cadastro
```
Ou utilizando um arquivo de lista de palavras:
```bash
python phishhunter.py -l wordlist.txt
```

### Exemplo de Saída
```bash
[REGISTRED/OFFLINE] inscricoesconcurso2025.com
      [Subdominio Found] cadastro.inscricoesconcurso2025.com - Title: "Página Oficial"
```

