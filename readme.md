<img width="662" height="86" alt="88cc8ab2409d8d9f1ad17f731f45af61" src="https://github.com/user-attachments/assets/02a2c184-6688-40f4-9f3b-4d1a0cfe1a91" />

 <img alt="Notebook" src="https://img.shields.io/badge/jupyter-notebook-E0234E?logo=jupyter&logoColor=white" /> <img alt="Python" src="https://img.shields.io/badge/python-3.x-3776AB?logo=python&logoColor=white" />


## Como funciona
O agente representado por personagem de jogo 2d **pac-man**, precisa achar um caminho no labirinto,  usando método aprendizado por reforço(reinforcement learning) 
a cada passo ele recebe -1 porém, +1 ponto cada bolinha adquirida. Caso esbarre em fantasma o total de pontos são de 100 falhando e realizando outra tentativa. a saída representada por cereja
representa +100 com isso  considera que ganhou

<img width="400" height="250" alt="pac" src="https://github.com/user-attachments/assets/86424d2a-4a7a-4356-99b2-1db18be74bf0" />





- A: Action (ação). O que o agente decide fazer.
- R: Reward (recompensa). O sinal que diz se a ação foi boa ou ruim.
- S′: Next state. O estado seguinte, depois da ação.
- π: Policy (política). A regra que escolhe a ação em cada estado.
- γ: Discount factor. O peso do futuro, entre 0 e 1.

## Tabela 

| Situação | Recompensa |
|---|---|
| Passo normal | -1 |
| Parede ou borda | -5 |
| Bolinha (só na 1ª vez no episódio) | +2 |
| Fantasma | -100 (fim) |
| Cereja | +100 (fim) |

## Parâmetros principais

| Parâmetro | Valor | Significado |
|---|---|---|
| `alpha` | 0.2 | taxa de aprendizado |
| `gamma` | 0.5 | peso do futuro |
| `epsilon` / `epsilon_min` | 1.0 / 0.001 | exploração inicial / mínima |
| `decay` | 0.998 | quanto o epsilon diminui por episódio |
| `N_EPISODES` | 3000 | tentativas de treino |
| `MAX_STEPS` | 400 | limite de passos por tentativa |
| `PELLET_BONUS` | 3 | bônus ao comer bolinha |

## Como rodar

### Crie ambiente
```bash
python -m venv venv
```
### Ative ambiente
```bash
source venv/bin/activate
```
### Instale pacotes
```bash
pip install -r requirements.txt
```
### Rode notebook
```bash
jupyter notebook 
```

