<img width="662" height="86" alt="88cc8ab2409d8d9f1ad17f731f45af61" src="https://github.com/user-attachments/assets/02a2c184-6688-40f4-9f3b-4d1a0cfe1a91" />

 <img alt="Notebook" src="https://img.shields.io/badge/jupyter-notebook-E0234E?logo=jupyter&logoColor=white" /> <img alt="Python" src="https://img.shields.io/badge/python-3.x-3776AB?logo=python&logoColor=white" />


## Como funciona 
O agente representado pelo personagem *pacman* precisa descobrir o melhor caminho que está demonstrado pela a frutinha para conseguir passar da fase, esse método conhecido reinforcement learning (aprendizado por reforço)

<img width="400" height="250" alt="pac" src="https://github.com/user-attachments/assets/86424d2a-4a7a-4356-99b2-1db18be74bf0" />


-----------------------------------------------
- A: Action (ação). O que o agente decide fazer.
- R: Reward (recompensa). O sinal que diz se a ação foi boa ou ruim.
- S′: Next state. O estado seguinte, depois da ação.
- π: Policy (política). A regra que escolhe a ação em cada estado.
- γ: Discount factor. O peso do futuro, entre 0 e 1.
-----------------------------------------------

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
### Rode Ambiente
```bash
jupyter notebook 
```

